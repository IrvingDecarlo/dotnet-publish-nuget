dotnet-publish-nuget, a GitHub Action by Irving Decarlo

# What is the Action for?

dotnet-publish-nuget is an action that builds, packs and publishes .csproj files as .nupkg to NuGet.

## How to use

It can be used freely by any workflow. It has 3 parameters:
1. `files-csproj`: A comma-separated list of .csproj files to pack and publish:
```
files-csproj: "Example/Example.csproj,Test/Test.csproj"
```
2. `nuget-key`: The NuGet.org API token to use for publishing the packages. Register it as a secret in your repository:
```
nuget-key: ${{ secrets.NUGET_API_KEY }}
```
3. `restore-workloads`: "Restore the projects' workloads? Accepts 'true' or 'false'. Defaults to 'false' if not specified."
```
restore-workloads: 'true'
```

It has no outputs.

> [!IMPORTANT]
> .Net must be set up prior to using this action or else it will not work.

## How can I contribute

Feel free to give me any suggestions that you believe will improve the Action. Additionally, you may make your own Action that is based on this one.

Thank you!
