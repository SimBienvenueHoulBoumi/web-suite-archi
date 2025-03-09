```bash
docker logs -f webtoon-suite-api-dev # voir les log

#faire une migration avant d'accéder au site
docker exec -it webtoon-suite-api-dev sh
npx prisma migrate deploy

url: http://host.docker.internal:[PORT]/api#/

## supprimer tout
docker system  prune -a


## Quand le docker est lancé en mode dev les modifications sont prisent en compte automatiquement

```
