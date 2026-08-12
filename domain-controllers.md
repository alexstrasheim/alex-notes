# Domain Controllers

## Domain controller IPs

Connect to VPN, then RDP

```
10.151.150.252
10.151.150.253
10.151.150.254
```

## Sync

To Sync changes across Domain Controllers (DC)
```
repadmin /syncall /Aedpq
```
To Sync with Azure immediately
```
Invoke-Command wdc-005-prod {start-adsyncsynccycle -policytype delta}
```