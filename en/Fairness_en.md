## 1. Fair random number algorithm ##

All games on the TRON Go platform are based on smart contracts deployed on TRON. We can't interfere with the generating of random numbers, this ensures the fairness of the game. The algorithm of random number  is as follows.

**Slot:<br>**
randomNum = sha256(sign(address + bet_amount + bet_count + randNonce + timestamp)<br>
randNonce++<br>
randomNum = sha256(sign(randNonce + randomNum + timestamp) Mod 24<br>

**Dice:<br>**
randomNum = sha256(sign(address + bet_amount + bet_count + randNonce + timestamp)<br>
randNonce++<br>
randomNum = sha256(sign(randNonce + randomNum + timestamp) Mod 100<br>

## 2. Verifying Transactions ##

Users' betting records generated in all games on the TRON Go platform will be displayed below games. We have placed the entrance for users to view transaction of any record on the chain. And users can click and jump to the TRON explorer to verify transaction details.