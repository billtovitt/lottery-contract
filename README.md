# lottery_smart_contract


# Things used in the project :-

1. Solidity programming language.
2. Ethereum.
3. Remix IDE.




# Architecture of the project :-

Global Variables :- 
1. Owner -> The real owner who deployed the contract ( type address ).
2. Players -> All the players address will be stored in this dynamic array ( type address[] ).
3. lotteryNo -> keep track of total lotteries done.
4. winners -> key value pair to keep track of  lottery winners history.


Functions  :- 
1. Enter Lottery
2. Pick winner
3. Get random number.
4. get balance.
5. get players
6. get winners by lottery id.




# How It works :-

1. The lottery starts accepting transactions, anyone having an ethereum wallet can send a minimum amount of 0.001 Ether.

2. The Player send Ether directly to the contract address and after that their ethereum address is registered. A user can send more transactions and we don't impose the maximum amount allowed to be sent.

3. There will be a manager, The owner who will deploy the contract. 

4. At some point, randomly chosen by the manager, he'll pick a random winner from the player list. Only the manager is allowed to see the contract balance and randomly select the winner.

5. The contract will transfer the entire balance to the winner address and the lottery is reset and ready for the next round.

