# Cen API
Dedicated Api for Cen providing User, Transaction & Analytical Data.

Development Repo https://github.com/dylanheath/cen-server

### General Usage


All usage must be server side, abiding by the CORS policy.

#### EndPoints

### Transactions
```
GET mainnet.cen.network/.netlify/functions/api/transactions/getall
GET mainnet.cen.network/.netlify/functions/api/transactions/getsent{address, name, email or phone number}
GET mainnet.cen.network/.netlify/functions/api/transactions/getreceived{address, name, email or phone number}
```
### Users
```
GET mainnet.cen.network/.netlify/functions/api/user/{address, name, email or phone number}
```

### Analytics
```
GET mainnet.cen.network/.netlify/functions/api/transactions/totaltransactions
GET mainnet.cen.network/.netlify/functions/api/transactions/totalamount
```

### Status

```
GET mainnet.cen.network/.netlify/functions/api/status
```

#### Response Times & Timeouts

Expect Cold starts while Cen is growing, 200+ ms responses 

Expect higher response times outside San Francisco (Netlify AWS lambda functions)
