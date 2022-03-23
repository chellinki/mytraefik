# mytraefik v2
### Before starting the traefik v2 please follow the below steps:

##### 1) Create an empty acme.json file and provide the read and write permission only to user
```
touch acme.json
```
```
chmod 600 acme.json
```

##### 2) Create a logs directory and within it create an access.log file with 644 permissions
```
mkdir logs
```
```
touch logs/access.log
```
```
chmod 644 logs/access.log
```

##### 3) Update the details in docker-compose.yml file for mailid, domains, basicauth 
> For htpassword generation use below link: (add an extra `$` symbol for each `$` symbol)

https://www.web2generators.com/apache-tools/htpasswd-generator

##### 4) Start the `Traefik`
```
docker-compose up -d
```
