"# bonus_ASP.NET" 

In this bonus section I've built an “ASP.NET Core Web App” project using visual studio.

### steps and requirements:

## part 1- local work in visual studio:
- by adding “Newtonsoft.Json" nuget package-
csproj content has been added:

```
<pre>
  <ItemGroup>
    <PackageReference Include="Newtonsoft.Json" Version="13.0.1" />
  </ItemGroup>
</pre>
```

- nuget package has been restored.

- project has been reCompiled.

# Which files and folders were created?
mostly everything you see in this repo, but publish added release and debug folders inside the bin folder.
actual project files are in the release - publish folder.

- the project has been published to the local folder.

## part 2 - transfer site to windows machine:

- added IIS and dotnet core to the windows machine.

- created a new IIS app pool.

- used port 5100 for the IIS app pool.

- copied the published site to the windows machine.

- added   "Urls": "http://localhost:5100/", to appsettings.json file.

- ran dotnet command to start the site - had a port conflict (on the same port as IIS), so i turned IIS down and ran dotnet again.

