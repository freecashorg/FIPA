```
FIPA4: CoinDays
Version: 1
Language: en-US
Author: Deisler-JJ_Sboy
Status: draft
Created date: 2021-03-08
LastModifiedDate：2021-03-08
File hash: "unknown"
TXid: 
```

# FIPA4_CoinDays(en-US)

## Contents

[Introduction](#introduction)

[General rules of FEIP type protocols](#general-rules-of-feip-type-protocols)

[Rules specific to this protocol](#rules-specific-to-this-protocol)

[CoinDays of an UTXO](#CoinDays-of-an-UTXO)

[CoinDays of an CID](#CoinDays-of-an-CID)


## Introduction

```

ProtocolType: FIPA
SerialNumber: 4
ProtocolName: CoinDays
VersionNumber: 1
Description : CoinDays is an indicator for FCH holders.
Author: Deisler-JJ_Sboy
Language: en-US
Tags: FIPA, CoinDays
PreVersionHash:"unknown"

```

## General rules of FEIP FIPA protocols



## Rules specific to this protocol

1. CoinDays can be simply understood as: (quantity of coins) multiplied by (holding time).
2. Exact calculation. <br>
  The precision of FCH is 0.00000001FCH, or 1 Satoshi. 

```python
    # e.g. : 987654321 Satoshi = 9.87 Coins
    Coins = (floor(Satoshi of UTXO / 1000000)) /100.0
```

  The Timestamp in the blockhead is seconds from Unix Epoch, and we need to format it to Days. We define the calculation as follows:
    
```
    Days =  (generatedTimestamp - spentTimestamp) / (24 * 3600)
    generatedTimestamp = Timestamp of blockHead when UTXO is generated
    spentTimestamp = Timestamp of blockHead when the UTXO is spent
```

## CoinDays of a UTXO

## CoinDays of an CID
