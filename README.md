#Ejecutar los comandos, en orden:
pm2 start src/index.js --name front --watch
#Corre el front en localhost

pm2 start src/index.js --name api8082 --watch -- --port 8082
pm2 start src/index.js --name api8083 --watch -- --port 8083
pm2 start src/index.js --name api8084 --watch -- --port 8084
pm2 start src/index.js --name api8085 --watch -- --port 8085
#Arrancan la api en los puertos que se pasan como argumento

sudo service nginx start
#Corre nginx