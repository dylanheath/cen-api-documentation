# Cen API
Dedicated Api for Cen providing User, Transaction & Analytical Data.

Development Repo https://github.com/dylanheath/cen-server

### General Usage

All usage must be server side, abiding by the CORS policy.

### EndPoints

Transactions
```
GET mainnet.cen.network/.netlify/functions/api/transactions/getall
GET mainnet.cen.network/.netlify/functions/api/transactions/getsent{address, name, email or phone number}
GET mainnet.cen.network/.netlify/functions/api/transactions/getreceived{address, name, email or phone number}
GET mainnet.cen.network/.netlify/functions/api/transactions/totaltransactions
```
Users
```
GET mainnet.cen.network/.netlify/functions/api/user/{address, name, email or phone number}
```

Analytics
```
GET mainnet.cen.network/.netlify/functions/api/transactions/totaltransactions
```
#### Response Times & Timeouts

Responses may be slow because the functions will cold start leading to 150+ ms, only caused by minimal connections.

For those in *Australasia* expect higher response times, Netlify AWS Lambda is located in Sans Francisco
