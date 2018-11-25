# EdxToken
Token contracts for edx


## detailedBalance
* use detailedBalance to retrieve vested
* param:

  1.account: which account

  2.mtype:  
  * 0/1 all tokens  returns (all tokens, transferrable tokens)
  * 2 basestone Invest info   (all invested, locked)
  * 3 pe Invest info   (all invested, locked)
  * 4 team Invest info   (all invested, locked)

## 	grantRole(address account,uint8 mtype,uint256 amount)

* use grantRole to set authorization
* param:

  1.account: which account to author

  2.mtype:  

  * 2 as basestone
  * 3 as pe Invest
  * 4 as team Invest info
  * others clear account's rights

  3.amount  
  how many tokens can be used

  ##    roleInfo(uint8 mtype)  returns(address,uint256)

   check for bs/pe/tm roleInfo

  ** param:**

    1.mtype:  

    * 2 as basestone
    * 3 as pe Invest
    * 4 as team Invest info

  ** returns **

   (address,value) address is master account for bs/pe/tm and value mean how many coins can be assigned
