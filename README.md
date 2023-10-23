# DockerCompose-PostgreSQL-PGAdmin
#Instructions
1. Create docker compose file and begin adding setup to it

   ``
   touch docker-compose.yml; code docker-compose.yml
   ``

2. Create another file to hold psql data for the table to be created and data inserted into table
  
   ``
   touch psql; code psql
   ``

3. Run `` docker-compose up -d `` to get your containers running
4. Run `` docker ps `` to see running containers. Grab container id for the container named 'pgadmin'
5. ``docker inspect container_id`` and search for Gateway: IP address. This will be for connected to the server
6. Open up a browser and type localhost:5050 then sign in with pgadmin credentials created in compose file
7. Add server and input username, password, host address then connect
8. Click query tool then add sql code

#References 

https://www.pgadmin.org/docs/pgadmin4/latest/container_deployment.html

https://hub.docker.com/_/postgres
