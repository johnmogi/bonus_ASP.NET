# bonus_ASP.NET

In this bonus section I've studied ASP.NET and how to use it to create a simple web application.

## Part 1: Create and build a website

[] Created “ASP.NET Core Web App” project using visual studio.
[] by adding “Newtonsoft.Json" nuget package-
csproj content modified:

`<ItemGroup> <PackageReference Include="Newtonsoft.Json" Version="13.0.1" /> </ItemGroup>`

Compile (rebuild) your project
Which files and folders were created?

mostly everything you see in this repo, but publish added release and debug folders.
actual project files are in the release - publish folder.

## Part 2: Create website on your Microsoft machine

- Add IIS to your windows server:

using rdp, added feaures - IIS.

- Does it works? If not, make it work

finally, adding json URL 5100 - got a crash because both IIS and dotnet aplication dll ran on the same port (socket)
resolved by stopping IIS and running dotnet command.

![screenshot from within the server](/win.jpg)
