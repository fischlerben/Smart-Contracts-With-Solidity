# Smart Contracts With Solidity
![BlockchainPic](https://columbia.bootcampcontent.com/columbia-bootcamp/cu-nyc-fin-pt-09-2020-u-c/-/raw/master/Homework/20-Solidity/Instructions/Images/smart-contract.png)

This blockchain example creates an Ethereum-based Smart Contract which accepts Ether and divides it evenly among a hypothetical group of employees. This would allow a Human Resources department to pay employees quickly and efficiently.

## Contract Set-Up / Deployment:
First thing to make sure of is that both Ganache and MetaMask are running on your computer, and that your MetaMask is connected to your localhost.

This Solidity code was compiled in the Remix IDE:

![compiled_code](/Screenshots/compiled_code.png?raw=true)

Now, we are ready to deploy the contract to our local Ganache chain by connecting to the Injected Web3 environment.  The "Account" is my first address listed in Ganache - the 3 addresses listed under "Deploy" are the next 3 addresses listed in my Ganache:

![deploy_setup](/Screenshots/deploy_setup.png?raw=true)

![mm_pre_transfer](/Screenshots/mm_pre_transfer.png?raw=true)

Then, deploy your contract:

![metamask_ganache](/Screenshots/metamask_ganache.gif?raw=true)

After you send those transactions, you should notice that your MetaMask ETH balance declined:

![mm_post_transfer](/Screenshots/mm_post_transfer.png?raw=true)

You should also see the balances in your Ganache chain increase as well, depending on how much wei/Ether was sent.  In this particular example, only 101 wei was transferred (there is 10^18 wei in 1 Ether) so my accounts that received those transactions did not increase in ETH - however, we can confirm these transactions went through by navigating to the "Transactions" tab of Ganache:

![gan_transactions](/Screenshots/gan_transactions.png?raw=true)