# .NET Core Command-Line Interface (CLI) Kata

This kata trains usage of the .NET Core CLI to create projects.

Version: 1.0 (2018-12-27)  
Target duration: 5 minutes  
Required tools: [.NET Core 2.2 SDK](https://dotnet.microsoft.com/download)

## Specification

1. Create a folder called dotnet-cli-kata and navigate to it.
2. Create a ASP.NET Core Web App (MVC, C#) project called **MyProject.WebApp**.
3. Create a Class library project (C#) called **MyProject.Core**.
4. Create a unit test project (C#, MSTest) called **MyProject.Core.Tests**.
5. Create a solution file all.sln and add all 3 project to it.
6. List all projects in the all.sln and verify that all project have been added.
7. Add project reference in **MyProject.Core.Tests** to **MyProject.Core**
8. Add project reference in **MyProject.WebApp** to **MyProject.Core**
9. Add package **Moq** to **MyProject.Core.Tests**
10. Add package **Microsoft.EntityFrameworkCore** version 2.2.0 to **MyProject.WebApp**
11. Build all.sln
12. Run tests for **MyProject.Core.Tests**.
13. Publish **MyProject.WebApp** in folder "out" in *Release* configuration