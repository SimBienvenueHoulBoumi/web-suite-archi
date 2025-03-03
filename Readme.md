```bash
docker logs -f webtoon-suite-api # voir les log

#faire une migration avant d'accéder au site
docker exec -it webtoon-suite-api sh
npx prisma migrate deploy

url: http://host.docker.internal:[PORT]/api#/

## supprimer tout
docker system  prune -a

## lancer le programme
docker-compose --env-file .env up -d


```
