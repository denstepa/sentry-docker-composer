# sentry-docker-composer

### Install

1. docker-compose up -d redis postgres
2. docker run --rm sentry generate-secret-key
3. insert generated key into ```SENTRY_SECRET_KEY``` var
4. docker-compose up -d redis postgres sentry
5. docker exec -it compose-sentry sentry upgrade
6. set default user and password
7. docker-compose up -d
