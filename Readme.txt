Iniciar el proyecto
    npm init

Agregar dependencias:
    npm i body-parser cookie-parser cors express helmet mongoose morgan

Agregar dependencias desarrollo:
    npm i -D nodemon @types/body-parser @types/cookie-parser @types/cors @types/express @types/helmet @types/mongoose @types/morgan

Agregar typescript 
    npm i -D tsc

Convertir de types a javaScript
    npm run build
    npm run start

Iniciar servidor de mongoose
    cd C:\Program Files\MongoDB\Server\3.6\bin
    mongod.exe --dbpath D:\mongodb\data\db
    
    Abrir shell mongo
        cd C:\Program Files\MongoDB\Server\3.6\bin
        mongo
        crear base de datos:
            use dbnodemonapi
        insertar datos:
            db.dbnodemonapi.insert({"title": 'mi primer post',"content": 'mi primer post content'}) 
        ver datos insertados:
            db.dbnodemonapi.find()

Convertir el codigo
    C:\xampp\htdocs\angular\NodeMonApi>tsc

Iniciar el app
    node ./build/server.js

//Descargar complemento visual studiocode 
    Click en Extencions, REST Client
    //enviar peticion:
        GET http://localhost:3000/api/posts HTTP/1.1
    //Separar peticion
        ###
        //enviar datos para grabar
                POST http://localhost:3000/api/posts HTTP/1.1
                content-type: application/json
                {
                    "title": "mi primer post",
                    "content": "mi primer post content"
                }

    //Ver request.http
