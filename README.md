# Роутинг
## v2rayng
```
[{"enabled":true,"ip":["geoip:custom-blocked"],"locked":false,"outboundTag":"proxy","remarks":"Заблокированные IP в прокси"},{"domain":["geosite:custom-blocked"],"enabled":true,"locked":false,"outboundTag":"proxy","remarks":"Заблокированные сайты в прокси"},{"enabled":true,"locked":false,"outboundTag":"direct","port":"0-65535","remarks":"Остальное напрямую"},{"enabled":false,"locked":false,"outboundTag":"proxy","port":"0-65535","remarks":"Остальное в прокси"}]
```

# Роутинг c (geosite/geoip)-whitelist.dat
## v2rayng
```
[{"enabled":true,"ip":["geoip:custom-blocked"],"locked":false,"outboundTag":"proxy","remarks":"Заблокированные IP в прокси"},{"domain":["geosite:custom-blocked"],"enabled":true,"locked":false,"outboundTag":"proxy","remarks":"Заблокированные сайты в прокси"},{"enabled":true,"ip":["geoip:custom-whitelist"],"locked":false,"outboundTag":"direct","remarks":"РУ IP напрямую"},{"domain":["geosite:custom-whitelist"],"enabled":true,"locked":false,"outboundTag":"direct","remarks":"РУ сайты напрямую"},{"enabled":true,"locked":false,"outboundTag":"direct","port":"0-65535","remarks":"Остальное напрямую"},{"enabled":false,"locked":false,"outboundTag":"proxy","port":"0-65535","remarks":"Остальное в прокси"}]
```
