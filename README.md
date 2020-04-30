#Persist and retrieve relational data with Entity Framework Core

##Projekt fra https://docs.microsoft.com/en-us/learn/modules/persist-data-ef-core/

Kør følgende kommando fra en Powershell for at oprette tabeller i databasen

`dotnet ef database update --project /ContosoPets.DataAccess/ContosoPets.DataAccess.csproj --context ContosoPetsContext`

I Visual Studio kan du oprette en forbindelse til databasen via Server explorer. 

Database filen er 

C:\Users\**{dit brugernavn}**\ContosoPets.mdf

Kør AddData.sql scriptet fra ContosoPets.DataAccess projektet for at tilføje test data. 

Start ContosoPets.Api og lav et GET requetst til https://localhost:5001/Orders/2 med Postman eller anden api test tool for at teste om alt er oppe og køre.