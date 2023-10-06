# Curso Asp.Net Core

## Ambiente de trabajo
Ocuapomos instalar el dotnet sdk 3.1.201 y seteamos el dotnet con esta version 
```
dotnet new globaljson --sdk-version 3.1.201 --force
```

aparte ocupamos tener instalado el sql server express - https://www.microsoft.com/en-us/sql-server/sql-server-downloads 
al momento de instalarlo nos pedira instalar SSMS - https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16 

### Creamos la base de datos 
Creamos la base de datos con nombre "CursoOnline" y la tabla Curso

### Crea una solucion y proyecto ASP.NET core

creamos una carpeta en el disco local NetCore y accedemos mediante el cmd a esa carpeta
```
dotnet new sln 
```
### crea un proyecto 

creamos una carpeta "LeerData"
```
dotnet new console 
```

### Agregar LeerData.csproj a como parte de la solucion NetCore.sln

```
dotnet sln add LeerData/LeerData.csproj
```

### Para compilar el proyecto usando como intemediario la solucion

```
dotnet sln add LeerData/LeerData.csproj
```

### editamos la extension de C# y añadimos estas lineas 

```
    "omnisharp.monoPath": "",
    "omnisharp.sdkPath": "C:\\Program Files\\dotnet\\sdk",
    "omnisharp.path": "latest"
```