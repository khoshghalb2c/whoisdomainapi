# WhoisDomainAPI
Query domains using this API.

[![Donate](DonateIDPay.svg)](https://idpay.ir/khoshghalb2c/)
## Getting Started
Read the description below to get started with `whoisdomainAPI`.

## How to use?
You need to send 2 parameters to the server and wait for the response.
**The values to send are as follows:**
1. `domain`; Your DomainName for query.
2. `APIKEY`; Your Api-Key for identification.

## What is the API response?
If there is no problem with the values you sent, Api return below fields:
1. Result code; with the name `result`
2. The DomainName you submitted; with the name `domain`
3. Query from that domain's nic server; with the name `query`
4. Mondified DateTime in Tehran Time; with name `datetime`
5. Time method; with name `time`
6. Your IP; with name `ip`

## What is the code and meaning of the errors?
If the API give error, it is definitely one of the following values:
1. APIKEY is incorrect <sub>code: **101**</sub>
2. APIKEY is empty <sub>code: **102**</sub>
3. APIKEY don't send <sub>code: **103**</sub>
4. DomainName is invalid <sub>code: **104**</sub>
5. DomainName is empty <sub>code: **105**</sub>
6. DomainName don't send <sub>code: **106**</sub>
7. The Domain's nic server, not found in the list. <sub>code: **301**</sub>
8. Could not connect to that domain's nic server <sub>code: **302**</sub>
9. An unknown error has occurred. Make sure the DomainName is correct  <sub>code: **303**</sub>

## Attentions!
- In case of an error, the name of the returned values is `error_code` and `error_text`.
- One of the response fields is ResultCode. ResultCode is usually 200.
- Contact me to get `APIKEY`.
- You must be send your fields to `https://khoshghalb2c.ir/api/whois/index.php` with **`POST`** method.
- See example in [here](example.html).
- You are can whois from your domain in [this](https://khoshghalb2c.ir/whois) link without Api.

## Licence
```
Copyright © 2023 Khoshghalb2c.ir. All Rights Reserved.
```
