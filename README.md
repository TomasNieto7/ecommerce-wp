# Instrucciones para levantar el entorno Docker de ecommerce-wp

## 1. Requisitos previos
- Tener instalado Docker Desktop y asegurarse de que esté corriendo.

## 2. Levantar los contenedores

Abre una terminal en la raíz del proyecto y ejecuta:

```powershell
docker-compose up -d
```

Esto descargará y levantará los contenedores necesarios en segundo plano.

## 3. Acceder a WordPress

Una vez que los contenedores estén arriba, accede a WordPress desde tu navegador en:

- [http://localhost:8080](http://localhost:8080)

## 4. Acceder a la base de datos (phpMyAdmin)

Puedes gestionar la base de datos MySQL usando phpMyAdmin en:

- [http://localhost:8081](http://localhost:8081)

### Credenciales por defecto
- **Usuario:** wordpress
- **Contraseña:** wordpress
- **Host:** db

## 5. Importar la base de datos 

Una ves dentro de phpMyAdmin importa la base de datos que se encuentra en:

- [https://drive.google.com/drive/folders/155GJJh5Hw2Xaz9w2XAdcU49Ab_GvuPs-?usp=sharing](https://drive.google.com/drive/folders/155GJJh5Hw2Xaz9w2XAdcU49Ab_GvuPs-?usp=sharing)

## 6. Detener los contenedores

Para detener los contenedores, ejecuta:

```powershell
docker-compose down
```

---

Si tienes problemas, asegúrate de que Docker Desktop esté corriendo y revisa los logs con:

```powershell
docker-compose logs
```
