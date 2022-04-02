## 1. Database first approach: scaffold DBContext from database, selecting the tables to scaffold

Scaffold-DbContext 'Data Source=(localdb)\MSSQLLocalDB;Initial Catalog=Northwind;Integrated Security=True;Connect Timeout=30;Encrypt=False;TrustServerCertificate=False;ApplicationIntent=ReadWrite;MultiSubnetFailover=False' Microsoft.EntityFrameworkCore.SqlServer -Tables Suppliers, Products, Categories

## 2. Code First Approach: Migration of Model from DBContext to Database

- dotnet ef migrations add InitialCreate
- dotnet ef database update
- 

