# Mediul de dezvoltare

## Cerințe

- Docker Desktop (cu Docker Compose) sau Docker Engine și pluginul Compose
- Git
- Un browser modern (Chrome, Firefox sau Edge)

Node.js v24.22.1 și Yarn v4.18.1 sunt furnizate de containerul `app`; nu le
instala și nu rula comenzi `node` sau `yarn` pe gazdă.

## Pornire

Din rădăcina proiectului, construiește imaginea și pornește containerul:

```sh
docker compose up --build -d
```

Portul 5173 este publicat la adresa http://localhost:5173. Aplicația este încă
în lucru și `package.json` nu definește încă un script de server; pagina va fi
disponibilă când serverul aplicației va porni în container pe portul 5173.

## Comenzi Yarn

Rulează comenzile Yarn numai în containerul pornit:

```sh
docker compose exec app yarn install
docker compose exec app yarn --version
docker compose exec app yarn <comandă>
```

Prima comandă instalează dependențele declarate în manifestul Yarn.
De exemplu, verificarea proiectului din `bin/check` rulează
`docker compose exec -T app yarn build`.

## Oprire

Oprește și elimină containerul proiectului:

```sh
docker compose down
```
