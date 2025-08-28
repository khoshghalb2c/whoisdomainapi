# WhoisDomainAPI
Query domains using this API.

## Getting Started
Read the description below to get started with **whoisdomainAPI**.

## How to use?
You need to send 2 parameters to the server and wait for the response.
**The values to send are as follows:**
1. `domain`; Your DomainName for query.
2. `APIKEY`; Your Api-Key for identification.

## What is the API response?
If there is no problem with the values you sent, Api return below fields:
1. Result code; named `result`
2. The DomainName you submitted; named `domain`
3. Query from that domain's nic server; named `query`
4. Mondified DateTime in Tehran Time; named `datetime`
5. _time()_ method in php; named `time`
6. Your IP; named `ip`
> [!TIP]
> When your <ins>non-IR</ins> domain query is successful, the `result` is **200**. <br/>
> When your <ins>IR</ins> domain query is successful, the `result` will be one of either **201**, **202**, or **203**.

## What is the code and meaning of the errors?
If the API give error, it is definitely one of the following values:
1. APIKEY expired <sub>code: **100**</sub>
2. APIKEY is incorrect <sub>code: **101**</sub>
3. APIKEY is empty <sub>code: **102**</sub>
4. APIKEY don't send <sub>code: **103**</sub>
5. DomainName is invalid <sub>code: **104**</sub>
6. DomainName is empty <sub>code: **105**</sub>
7. DomainName don't send <sub>code: **106**</sub>
8. APIKEY limit is over <sub>code: **107**</sub>
9. The Domain's nic server, not found in the list. <sub>code: **301**</sub>
10. Could not connect to that domain's nic server <sub>code: **302**</sub>
11. An unknown error has occurred. Make sure the DomainName is correct  <sub>code: **303**</sub>
> [!NOTE]
> If an error occurs, the return values ​​are named `error_code` and `error_text`.

## Attentions!
- Contact me to get `APIKEY`.
- You must be send your fields to `https://khoshghalb2c.ir/api/whois/index.php` with **`POST`** method.
- See example in [here](example.html).

## Licence
```
Copyright © 2022-2025 Khoshghalb2c.ir. All Rights Reserved.
```
