# Run project locally via docker

1. Clone repository from githab;
2. Open project in your IDE;
3. Run command '***docker compose up db***'.

## Load the database backup

4. For upload db backup in the DB container ***contact with admin for obtain database dump. Arter, execute the following command in the terminal:***

>`docker compose exec -T db pg_restore -U wikiuser -d wiki --no-owner --no-privileges < wiki_backup.dump`

## Setup other services
5. Wait untill backup loaded.
6. Execure command in the terminal: 
>`docker compose up`

##### NOTE:
If you have any troubles with setup please contact to project admin or official docs for Wiki.js and Docker.