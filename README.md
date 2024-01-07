<p align="center">
  <img src="https://1000logos.net/wp-content/uploads/2021/11/Docker-Logo-2013.png" width="800px" height="600" alt="Docker Logo">
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

