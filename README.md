# Роутинг "Проксировать только заблокированное"
## [v2rayng](https://github.com/2dust/v2rayNG/releases), [Exclave](https://f-droid.org/packages/com.github.dyhkwong.sagernet/)
__Geodat файлы добавлять под названием geoip.dat/geofile.dat, чтобы они заменили собой дефолтные:__
  - geoip.dat - <https://github.com/vacuumbeef/geodat/releases/latest/download/geoip.dat>
  - geosite.dat - <https://github.com/vacuumbeef/geodat/releases/latest/download/geosite.dat>

__Доменная стратегия: IPIfNonMatch__

__Роутинг:__
```
[{"enabled":true,"ip":["geoip:custom-blocked"],"locked":false,"outboundTag":"proxy","remarks":"Заблокированные IP в прокси"},{"domain":["geosite:custom-blocked"],"enabled":true,"locked":false,"outboundTag":"proxy","remarks":"Заблокированные сайты в прокси"},{"enabled":true,"locked":false,"outboundTag":"direct","port":"0-65535","remarks":"Остальное напрямую"},{"enabled":false,"locked":false,"outboundTag":"proxy","port":"0-65535","remarks":"Остальное в прокси"}]
```

## Happ
```
happ://routing/add/eyJibG9ja2lwIjpbXSwiYmxvY2tzaXRlcyI6W10sImRpcmVjdGlwIjpbIjEwLjAuMC4wLzgiLCIxNzIuMTYuMC4wLzEyIiwiMTkyLjE2OC4wLjAvMTYiLCIxNjkuMjU0LjAuMC8xNiIsIjIyNC4wLjAuMC80IiwiMjU1LjI1NS4yNTUuMjU1IiwiZ2VvaXA6cHJpdmF0ZSJdLCJkaXJlY3RzaXRlcyI6WyIucnUiXSwiZG5zaG9zdHMiOnsiY2xvdWRmbGFyZS1kbnMuY29tIjoiMS4xLjEuMSIsImRucy5nb29nbGUiOiI4LjguOC44In0sImRvbWFpbnN0cmF0ZWd5IjoiSVBJZk5vbk1hdGNoIiwiZG9tZXN0aWNkbnNkb21haW4iOiJodHRwczovL2Rucy5nb29nbGUvZG5zLXF1ZXJ5IiwiZG9tZXN0aWNkbnNpcCI6IjguOC44LjgiLCJkb21lc3RpY2Ruc3R5cGUiOiJEb0giLCJmYWtlZG5zIjpmYWxzZSwiZ2VvaXB1cmwiOiJodHRwczovL2dpdGh1Yi5jb20vdmFjdXVtYmVlZi9nZW9kYXQvcmVsZWFzZXMvbGF0ZXN0L2Rvd25sb2FkL2dlb2lwLmRhdCIsImdlb3NpdGV1cmwiOiJodHRwczovL2dpdGh1Yi5jb20vdmFjdXVtYmVlZi9nZW9kYXQvcmVsZWFzZXMvbGF0ZXN0L2Rvd25sb2FkL2dlb3NpdGUuZGF0IiwiZ2xvYmFscHJveHkiOmZhbHNlLCJsYXN0dXBkYXRlZCI6IjE3NzczOTk3NjYiLCJuYW1lIjoi0KLQvtC70YzQutC+INC30LDQsdC70L7QutC40YDQvtCy0LDQvdC90L7QtSIsInByb3h5aXAiOlsiZ2VvaXA6Y3VzdG9tLWJsb2NrZWQiXSwicHJveHlzaXRlcyI6WyJnZW9zaXRlOmN1c3RvbS1ibG9ja2VkIl0sInJlbW90ZWRuc2RvbWFpbiI6Imh0dHBzOi8vY2xvdWRmbGFyZS1kbnMuY29tL2Rucy1xdWVyeSIsInJlbW90ZWRuc2lwIjoiMS4xLjEuMSIsInJlbW90ZWRuc3R5cGUiOiJEb0giLCJyb3V0ZW9yZGVyIjoiYmxvY2stZGlyZWN0LXByb3h5In0=
```
