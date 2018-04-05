## Preparation of block chain competition meeting

---

* **Bitcoin transaction:**

  * Alice: $p_a$,$s_a$

  * Bob: $p_b$,$s_b$

  * Alice prepare the following message

    ```python

        Detail= "pa sends 1 bitcoin to pb"
        Signature=Sign(Detail,sa)   
    	
        Transaction={Detail,Signature}
        
    ```

  * The community(miners) verifies if Alice's transaction is valid

    ```py
    	if Verify(Transaction,pa)==True:
    		Include this Transaction into the current block
    	else:
    		Reject the Transaction
    ```

  ---

  ​

* **Blocks, or transaction ledgers, are blocks of transactions.** It is nothing but a data structure in CS language.

  ​

* **3 essential properties of a block chain.**

  * i. Append only (A singly link list)
  * ii. Not possible to revise a block ( this heavily uses the Universal Hash Functions )
  * iii. Global  (Network broadcasting)

* The insight of these 3 properties: 

  * So it serves as a perfect **<u>time-proof</u>** data structure.
  * Time-proof: Data structure grows in the same direction of time flow, and it is improbable to modify the history. 
  * In use cases like money transaction, stock trading, logistic record tracing, contract enforcement,  **<u>where people needs a proof to achieve unanimous consensus upon history</u>**,  a block chain is handy.

---

* **More use cases**

  * Online wallet, contiguous payment, money exchange, casino.
  * Auctions.
  * Anonymous file storage, secure cloud data services.
  * Contract enforcement.
  * Retailing, safe payment (escrow method).
  * IOT related, like firmware update.
  * Supply chain record.
  * Internal trading between enterprises.
  * Anything else that you can modeled as transactions and transaction ledgers.

  ​

* Possible paths of variations to discover

  * Different transaction format and transaction policy.
  * Different block minting methods (for bitcoin proof of work, for etherum proof of stake)
  * Anonymity in transaction (zerocash, monero)
  * Centralized block chain ( internal trading, efficient central bank )
  * More efficient network and book keeping.