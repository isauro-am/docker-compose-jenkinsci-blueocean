# Docker-compose-jenkinsci-blueocean

Requisitos
 - Docker
 - Docker-compose

Ejecutar

- docker build do-t jenkins/blueocean_ci --no-cache .
- docker-compose up

Principalmente ejecutamos unicamente el "up" para poder capturar la contraseña proporcionada para configurar nuestro acceso admin. 

```docker
*************************************************************
jenkings_container | *************************************************************
jenkings_container | *************************************************************
jenkings_container | 
jenkings_container | Jenkins initial setup is required. An admin user has been created and a password generated.
jenkings_container | Please use the following password to proceed to installation:
jenkings_container | 
jenkings_container | fdb101f773a44s7c6bs0b4dd4b29b9fe
jenkings_container | 
jenkings_container | This may also be found at: /var/jenkins_home/secrets/initialAdminPassword
jenkings_container | 
jenkings_container | *************************************************************
jenkings_container | *************************************************************
jenkings_container | *************************************************************
```
Ahora se puede acceder mediante 

http://localhost:8080