
# Common commands for Clean Architecture (.NET) project

## Build project
```sh
# Build the entire solution
dotnet build CleanArchitecture.sln
# Or build a specific project
dotnet build src/Web.Api/Web.Api.csproj
```

## Run project
```sh
# Run the Web API
dotnet run --project src/Web.Api/Web.Api.csproj
```

## Watch run (auto-reload on code changes)
```sh
dotnet watch run --project src/Web.Api/Web.Api.csproj
```

## Check code format according to .editorconfig
```sh
# Check the entire solution, will fail if any file does not match the format
dotnet format --verify-no-changes CleanArchitecture.sln
```

- If there are formatting issues, fix them with:
```sh
dotnet format CleanArchitecture.sln
```

- You can replace CleanArchitecture.sln with the path to a .csproj file if you want to check only a specific project.
