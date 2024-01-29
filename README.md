<p align="center">
  <img src="https://1000logos.net/wp-content/uploads/2021/11/Docker-Logo-2013.png"  height="350px" alt="Docker Logo">
</p>

# Ejercicios Docker

## Desarrollador
- Francisco José García Flores

## Contenedores

### 1. Kali Linux con escritorio accesible por navegador

Para crear y ejecutar el contenedor:

```bash
docker build -t kali-desktop:latest .
docker run -d -p 5901:5901 --name kali-container kali-desktop:latest
```
### 2. Instalación del CMS Strapi

```bash
docker build -t strapi-cms:latest .
docker run -d -p 1337:1337 --name strapi-container strapi-cms:latest
```
### 3. Instalación del paquete PHPMyAdmin

```bash
docker build -t phpmyadmin-xampp:latest .
docker run -d -p 8080:80 --name phpmyadmin-container phpmyadmin-xampp:latest
```

### 4. Instalación de Portainer mediante ficheros YML

  1. Creamos un nuevo volumen
      ```bash
      docker volume create Portainer_data
      ```

  2. Verificamos que el volumen existe
     ```bash
     docker volume ls
     ```
     
  3. Corremos y creamos el contenedor mediante docker compose
     ```bash
      docker-composer up -d
      ```
