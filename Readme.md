```bash
docker logs -f webtoon-suite-api-dev # voir les log

## ports
api -> 5200
web-app -> 4000

#faire une migration avant d'accéder au site
docker exec -it webtoon-suite-api-dev sh
npx prisma migrate deploy

url-api: http://localhost:[API-PORT]/api#/
url-web: http://localhost:[WAB-APP-PORT]#/

## supprimer tout
docker system  prune -a


## Quand le docker est lancé en mode dev les modifications sont prisent en compte automatiquement

```
