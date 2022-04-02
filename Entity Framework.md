## 1. Database first approach: scaffold DBContext from database, selecting the tables to scaffold

`Scaffold-DbContext 'Data Source=(localdb)\MSSQLLocalDB;Initial Catalog=Northwind;Integrated Security=True;Connect Timeout=30;Encrypt=False;TrustServerCertificate=False;ApplicationIntent=ReadWrite;MultiSubnetFailover=False' Microsoft.EntityFrameworkCore.SqlServer -Tables Suppliers, Products, Categories`

## 2. Code First Approach: Migration of Model from DBContext to Database

- `dotnet ef migrations add InitialCreate`
- `dotnet ef database update`

## 3. Code First Approach: Alter a table

- Make Changes in your model
- add a migration with `dotnet ef migrations add ChangedInspectionType.InspectionNameToString`
- a migration file with `up` and `down` is created. `up` is run when you apply the migration. `down` is run if you ever decide to revert it
- `dotnet ef database update`
