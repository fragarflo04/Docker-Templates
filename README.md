<p align="center">
  <img src="docker-logo.png" alt="Docker Logo">
</p>

# Proyecto Docker

## Desarrollador
- [Tu Nombre]

## Contenedores

### 1. Kali Linux con escritorio accesible por navegador

Para crear y ejecutar el contenedor:

```bash
docker build -t kali-desktop:latest .
docker run -d -p 5901:5901 --name kali-container kali-desktop:latest
```
