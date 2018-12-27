# NET Core Command-Line Interface (CLI) Kata - Cheat Sheet

mkdir dotnet-cli-kata
new mvc -lang C# -n "MyProject.WebApps"
dotnet new classlib -lang C# -n "MyProject.Core"
dotnet new mstest -lang C# -n "MyProject.Core.Tests"
dotnet new sln -n all
dotnet sln add .\MyProject.Core\
dotnet sln add .\MyProject.Core.Tests\
dotnet sln add .\MyProject.WebApp\
dotnet sln list
dotnet add .\MyProject.Core.Tests\ reference .\MyProject.Core
dotnet add .\MyProject.WebApp\ reference .\MyProject.Core
dotnet add .\MyProject.Core.Tests\ package Moq
dotnet add .\MyProject.WebApps\ package Microsoft.EntityFrameworkCore --version 2.2.0
dotnet build all.sln
dotnet test .\MyProject.Core.Tests\
dotnet publish .\MyProject.WebApps\ -o .\out -c Release