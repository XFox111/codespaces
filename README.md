# Codespaces repository
This repository is used as a startpoint for GitHub Codespaces

## Devcontainer configuration
- PowerShell CLI
- .NET 6.0.100 (LTS)
- Node.JS 16.13.0 (LTS)
- Microsoft SQL Server Express

## VS code extensions
- ms-dotnettools.csharp
- ms-mssql.mssql

## LocalDB substitution
Codespaces don't support LocalDB, so you have to use a local SQL server
To setup your project to work with SQL server replace your LocalDB connection string in `appsettings.Development.json` with this value:
```
Server=localhost;Database=TestDB;Persist Security Info=True;User ID=sa;Password=P@ssw0rd;MultipleActiveResultSets=True;
```
