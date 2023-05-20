# Conexion a MongoDB

_Necesario tener instalado Node.js y una cuenta de MongoDB_

## Pasos a seguir

1. Vamos a dirigirnos al Atlas de MongoDB y crearemos un nuevo proyecto 

![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/12c33ec7-90ae-462b-8235-c5d94b6dc919)
![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/c4f2dac9-88e0-4f39-ba27-45785201af92)

2. Creamos una nueva base de datos 

![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/b41f828f-7ed5-426d-aed5-2420b60b8ae9)

3. Al crear un usuario, debemos guardar la contraseña (Podemos cambiar la contraseña por una más fácil de recordar)

![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/078619c2-db9e-4031-8a98-d53780fe4b4b)

4. En le apartado de agregar IP, colocaremos 0.0.0.0/0. Una vez hecho esto pulsamos Finish and Close

![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/d7abc3bb-30de-4c5f-b388-7009f436cfd2)

5. Entramos a la consola de VSCode e instalamos las dependencias necesarias para realizar la conexion

 - Nos posicionamos en la carpeta de nuestro proyecto, una vez posicionados, escribiremos npm init para inicializar nuestro proyecto, pulsamos enter en todas las opciones

 ![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/9e5c535f-9c70-4a8e-b73f-f0e22dfa90ec)

 - Procedemos a instalar las dependencias, en la consola vamos a escribir **npm i nodemon mongoose dotenv express** (Se pueden instalar todas las dependencias por separado, pero lo haremos de esta forma por comodidad)

![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/5f4b4d68-2819-4f10-a514-e48a4579bcff)

6. Luego de instalar las dependencias, nos dirigimos al archivo *package.json*, en la parte de scripts, vamos a agregar el script para iniciar nuestro servidor:

![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/14530cec-1dc4-4b3c-87b2-c89f2fb82734)

 - Colocamos una coma al final del script *test*, en la siguiente linea escribimos **"start": "nodemon index.js"** (Se puede colocar el nombre de tu preferencia, en este caso nuestro script se llama *start*)

![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/f9ce2aa8-b8b1-4351-9858-78551f72c6ea)

7. Volvemos a MongoDB, en nuestra base de datos entraremos en el apartado _connect_ 

![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/2fe57a8b-dcae-453e-940c-3cfc468c5ea6)

 - Dentro del menú, entraremos en _drivers_ 

![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/59a71a3a-56a6-4290-b9c5-44a59a7cf43f)
 
 - En la parte 3, copiaremos el código que nos es proporcionado 

![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/ea519c65-3deb-475c-9915-02a2ccbd783b)

8. De nuevo en VSCode, crearemos un archivo _.env_

![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/66beb935-94fb-4acb-aaeb-3b434826981a)
![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/af75281d-315f-4ce6-a5ee-95b4e01c3add)

9. Dentro del archivo, creamos una nueva variable de entorno, a la cual llamaremos __MONGO_URI_TEST__

![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/4876f05a-a7bd-4550-b4c3-a7d2a1b6e0f4)

 - Seguido, pegaremos el código que copiamos anteriormente, y en la parte que dice _password_ vamos a remplazarla por la contraseña de nuestro usuario (incluyendo los símbolos de mayor y menor que)
 
![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/6d3215b4-0e67-4d8a-9057-75b4c47301a6)
![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/4a395c9f-7a76-4ff4-87c3-5b687f9ee12b)

10. En la consola, vamos a escribir **npm run start** (Start es el nombre de nuestro script, en caso de que no hayas puesto ese nombre, remplazar _start_ por el nombre de nuestro script)
 
 ![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/fdfaed08-bbd8-4716-b25c-74644b6caf8f)
 
 11. Si todo ha ido bien, veremos en la consola lo siguiente: 
 
 ![image](https://github.com/ale2306dc/mongoConexion/assets/127338496/41d5557c-4e98-44a9-af0a-2dac185af3e1)

 Listo, ya estamos conectados a nuestro servidor!











