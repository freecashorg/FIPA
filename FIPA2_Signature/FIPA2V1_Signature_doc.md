```
FIPA2: Signature
Version: 1
Language: en-US
Author: 
Status: draft
Created date: 2021-04-24
LastModifiedDate：
File hash: "unknown"
TXid: 
```

# FIPA2_Signature(en-US)

## Contents

[Introduction](#introduction)




## Introduction

```

ProtocolType: FIPA
SerialNumber: 2
ProtocolName: Signature
VersionNumber: 1
Description : Defines the .
Author: 
Language: en-US
Tags: FIPA, Signature
PreVersionHash:"unknown"

```

## General rules of FIPA protocols



## Rules specific to this protocol
1.Message signature use ecdsa algorithm.

2.Signature format as below：<br/>
{ "msg":"xxxxx",//raw msg <br/>
  "address":"FKsiWy4KLHAArxy6bgjVx4QuAS8fS2FqBR",//fch address <br/>
  "signature":"H+B8xy6lwKIpSQ06kH8MyFUwqRnH1E2FEUrJDNYr+ZoFAHlFxlJ+zj4wFPNqi658PK63ARF vrJezoBrzzq9OLdA=",//signature <br/>
}


