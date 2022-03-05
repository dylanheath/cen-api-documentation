# Cen API
Dedicated Api for Cen providing User, Transaction & Analytical Data.

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
