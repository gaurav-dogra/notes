# Thinks I want to know more about

## 1. CoVariance and Contravariance

- concept behind <in T> & <out T>

```C#
interface ISortable<in T>
interface ISortable<out T>
```

```Java
interface IPopable<? extends T>
interface IPopable<? super T>
```

## 2. (Visual Studio) How to move selected text left/right, just as Alt + Up/Down moves them up/down

## 3. Add the User Secrets and override the connection string

- Execute the following in Package Manager Console *(View > Other Windows > Package Manager Console).*
- [https://makolyte.com/ef-core-how-to-create-a-database-and-a-table/](https://makolyte.com/ef-core-how-to-create-a-database-and-a-table/)

```powershell
Install-Package Microsoft.Extensions.Configuration.UserSecrets

```

*Note: The UserSecrets package contains Microsoft.Extensions.Configuration.Json already, so you don’t need to add it separately.*

- Right-click on the project > click **Manage User Secrets**.
- This creates the secrets.json file and opens it.
- Now can you override the connection string from appsettings by putting it in secrets.json:

```json
{
  "ConnectionStrings": {
    "Default": "Server=SQL_SERVER_INSTANCE_NAME;Database=StreamingService;Integrated Security=true"
  }
}

```

4. Tag Helpers
5. User Authentication and authorization
