Prowl Monorepo to make development of prowl game engine and it's packages easier

Add to the `Prowl.Monorepo.sln`:

```
dotnet sln Prowl.Monorepo.sln add Prowl.Echo/**/*.csproj
```

To reference one project to another:

```xml
<!-- Prowl.Runtime.csproj -->

<Project Sdk="Microsoft.NET.Sdk">
  <!-- ... -->

  <ItemGroup>
    <ProjectReference Include="..\..\Prowl.Paper\Paper\Paper.csproj" />
  </ItemGroup>

  <!-- ... -->
</Project>
```