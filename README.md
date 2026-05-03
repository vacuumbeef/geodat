# Роутинг
## v2rayng, Exclave
#### Geodat файлы добавлять под названием geoip.dat/geofile.dat, чтобы они заменили собой дефолтные:
  - geoip.dat - <https://github.com/vacuumbeef/geodat/releases/latest/download/geoip.dat>
  - geosite.dat - <https://github.com/vacuumbeef/geodat/releases/latest/download/geosite.dat>

### Доменная стратегия: IPIfNonMatch
#### Роутинг:
```
[{"enabled":true,"ip":["geoip:custom-blocked"],"locked":false,"outboundTag":"proxy","remarks":"Заблокированные IP в прокси"},{"domain":["geosite:custom-blocked"],"enabled":true,"locked":false,"outboundTag":"proxy","remarks":"Заблокированные сайты в прокси"},{"enabled":true,"locked":false,"outboundTag":"direct","port":"0-65535","remarks":"Остальное напрямую"},{"enabled":false,"locked":false,"outboundTag":"proxy","port":"0-65535","remarks":"Остальное в прокси"}]
```

## Happ
```
happ://routing/add/eyJibG9ja2lwIjpbXSwiYmxvY2tzaXRlcyI6W10sImRpcmVjdGlwIjpbIjEwLjAuMC4wLzgiLCIxNzIuMTYuMC4wLzEyIiwiMTkyLjE2OC4wLjAvMTYiLCIxNjkuMjU0LjAuMC8xNiIsIjIyNC4wLjAuMC80IiwiMjU1LjI1NS4yNTUuMjU1IiwiZ2VvaXA6cHJpdmF0ZSJdLCJkaXJlY3RzaXRlcyI6W10sImRuc2hvc3RzIjp7ImNsb3VkZmxhcmUtZG5zLmNvbSI6IjEuMS4xLjEiLCJkbnMuZ29vZ2xlIjoiOC44LjguOCJ9LCJkb21haW5zdHJhdGVneSI6IklQSWZOb25NYXRjaCIsImRvbWVzdGljZG5zZG9tYWluIjoiaHR0cHM6Ly9kbnMuZ29vZ2xlL2Rucy1xdWVyeSIsImRvbWVzdGljZG5zaXAiOiI4LjguOC44IiwiZG9tZXN0aWNkbnN0eXBlIjoiRG9IIiwiZmFrZWRucyI6ZmFsc2UsImdlb2lwdXJsIjoiaHR0cHM6Ly9naXRodWIuY29tL3ZhY3V1bWJlZWYvZ2VvZGF0L3JlbGVhc2VzL2xhdGVzdC9kb3dubG9hZC9nZW9pcC5kYXQiLCJnZW9zaXRldXJsIjoiaHR0cHM6Ly9naXRodWIuY29tL3ZhY3V1bWJlZWYvZ2VvZGF0L3JlbGVhc2VzL2xhdGVzdC9kb3dubG9hZC9nZW9zaXRlLmRhdCIsImdsb2JhbHByb3h5IjpmYWxzZSwibGFzdHVwZGF0ZWQiOiIxNzc3Mzk5NzY2IiwibmFtZSI6ItCi0L7Qu9GM0LrQviDQt9Cw0LHQu9C+0LrQuNGA0L7QstCw0L3QvdC+0LUiLCJwcm94eWlwIjpbImdlb2lwOmN1c3RvbS1ibG9ja2VkIl0sInByb3h5c2l0ZXMiOlsiZ2Vvc2l0ZTpjdXN0b20tYmxvY2tlZCJdLCJyZW1vdGVkbnNkb21haW4iOiJodHRwczovL2Nsb3VkZmxhcmUtZG5zLmNvbS9kbnMtcXVlcnkiLCJyZW1vdGVkbnNpcCI6IjEuMS4xLjEiLCJyZW1vdGVkbnN0eXBlIjoiRG9IIiwicm91dGVvcmRlciI6ImJsb2NrLWRpcmVjdC1wcm94eSJ9
```


# Роутинг c (geosite/geoip)-whitelist.dat
## v2rayng
```
[{"enabled":true,"ip":["geoip:custom-blocked"],"locked":false,"outboundTag":"proxy","remarks":"Заблокированные IP в прокси"},{"domain":["geosite:custom-blocked"],"enabled":true,"locked":false,"outboundTag":"proxy","remarks":"Заблокированные сайты в прокси"},{"enabled":true,"ip":["geoip:custom-whitelist"],"locked":false,"outboundTag":"direct","remarks":"РУ IP напрямую"},{"domain":["geosite:custom-whitelist"],"enabled":true,"locked":false,"outboundTag":"direct","remarks":"РУ сайты напрямую"},{"enabled":true,"locked":false,"outboundTag":"direct","port":"0-65535","remarks":"Остальное напрямую"},{"enabled":false,"locked":false,"outboundTag":"proxy","port":"0-65535","remarks":"Остальное в прокси"}]
```
