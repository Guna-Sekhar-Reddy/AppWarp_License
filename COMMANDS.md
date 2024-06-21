Server:
In Server/DB folder execute the following command to start database server :

java -cp hsqldb-2.3.1.jar org.hsqldb.server.Server --database.0 file:mydb --dbname.0 testdb

In Server/ folder execute the following command to start the server :

java -cp ".;AppWarpS2Server\*" Hello

Client:
In Client/ execute the following to make a request to get all online users in zone "ab" on the server :

node client.js

k6 testing:

k6 run scriptFilename.js ------------->(for 1 virtual user or if virtual users are defined in script file)
k6 run --vus 10 --duration 30s scriptFilename.js ---------> ( for 10 virtual users)
