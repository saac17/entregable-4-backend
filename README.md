entregable 4 
integrantes: Juan Sebastian Cantor Vaca y Santiago Alejandro Alvarez Capera

1. Clona este repositorio
```
git clone https://github.com/saac17/entregable-4-backend
```
2. Abre tu editor de codigo y descarga las dependencias
~~~
    npm install
~~~
3. Con Thunder Client(extencion de VSC) o Postman genera las siguientes peticiones

# Metodo POST: 
- para crear nuevos usuarios, envia un JSON con todos los campos requeridos
> **localhost:9000/api/v1/users**

- prueba iniciar session, debes enviar el correo y contraseña del usuario
- si las credenciales estan correctas te generara un token
> **localhost:9000/api/v1/auth/login**

# Metodo PATCH:
- Trata de editar uno de los usuarios que creaste, adjunta en el body los datos modificados en formato  JSON
- recuerda enviar en el HEADER HTTP la propiedad **{Authorization: JWT tu_token}**
> **localhost:9000/api/v1/users/userId**

# Metodo DELETE:
- Intenta eliminar un usuario
- recuerda enviar en el HEADER HTTP la propiedad **{Authorization: JWT tu_token}**
> **localhost:9000/api/v1/users/userId**

# Rutas protegidas adicionales:
# Metodo POST:
- Visualiza datos del usuario logeado
- recuerda enviar en el HEADER HTTP la propiedad **{Authorization: JWT tu_token}**
> **localhost:9000/api/v1/users/me**
