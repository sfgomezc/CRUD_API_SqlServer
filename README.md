# CRUD_API_SqlServer

Proyecto API en .NET 5 que permite manejo de contacto mediante un CRUD b�sico en una sola tabla, con almacenamiento en base de datos Azure SQL.

Requiere del paquete:
```
Microsoft.EntityFrameworkCore.SqlServer v3.1.28
Microsoft.EntityFrameworkCore.Tools v3.1.28
```

Comandos para migraci�n. El primero genera el modelo con las tablas y campos, el segundo comando actualiza la base de datos:
```
Add-Migration "mensaje de migracion"
Update-Database
```

![alt text](https://github.com/sfgomezc/CRUD_API_InMemory/blob/master/Img_API.png?raw=true)

POST  
https://crud-api-sqlserver.azurewebsites.net/api/contacts
```
{
  "fullName": "Steven Gomez",
  "email": "steven.gomez@gmail.com",
  "phone": 3011234567,
  "address": "Calle 181 # 19-41"
}
```

GET  
https://crud-api-sqlserver.azurewebsites.net/api/contacts

GET ```{id}```  
https://crud-api-sqlserver.azurewebsites.net/api/contacts/1eb1149f-7a1e-4c87-8560-88d4fc0e1114

PUT  
https://crud-api-sqlserver.azurewebsites.net/api/contacts/c7d062dc-2456-40a4-9a5f-3c4fc8e780af
```
{
  "fullName": "Steven Gomez C",
  "email": "steven.gomez.c@gmail.com",
  "phone": 3011230000,
  "address": "Calle 180 # 11-55"
}
```

DELETE  
https://crud-api-sqlserver.azurewebsites.net/api/contacts/c7d062dc-2456-40a4-9a5f-3c4fc8e780af

