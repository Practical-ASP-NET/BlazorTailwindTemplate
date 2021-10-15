# Blazor Tailwind Project Template for `dotnet new`

View on [Nuget.org](https://www.nuget.org/packages/PracticalDotNet.TailwindStarterProject/).

## Install template via nuget

From anywhere on your machine you can use this command to install the template directly from Nuget.

``` bash
dotnet new --install PracticalDotNet.TailwindStarterProject::6.0.0-rc2.1
```

## Install template from source

Alternatively, if you'd prefer, you can install it yourself from the source.

Download the source then change into the `content` folder.

From there you can install the template using `dotnet new --install`.

There's **no need to build anything first**. In fact, if you do build the project inside the content folder you might end up with extra folders (like bin, obj) being included in the template.

```bash
cd content
dotnet new --install .
```

In this example we instruct `dotnet` to look in the current folder (`.`) for any templates and install any it finds. 

It should find the `.template.config` folder which instructs it that this is a template for it to install.

## Spin up a new project using the template

Once you have the template installed it will show up in the list of templates for `dotnet new`.

``` bash
dotnet new -l
```

Here's how it should appear in the list…

``` bash
Blazor WASM Tailwind Project Template         blazor-tailwind      [C#]
```

From here you're now free to use the template to create your very own Blazor + Tailwind project!

``` bash
dotnet new blazor-tailwind - o ExampleApp
cd ExampleApp
dotnet watch
```

This example creates the project in an ExampleApp folder, then launches it using `dotnet watch`.

## Upgrading/downgrading the .NET version

When you create a new project using this template you'll discover that you new project references a specific version of .NET.

Taking the above example, if you looked at `ExampleApp\ExampleApp.csproj` you should see something like this...

``` xml
<PropertyGroup>
    <TargetFramework>net6.0</TargetFramework>
    <Nullable>enable</Nullable>
    <ImplicitUsings>enable</ImplicitUsings>
</PropertyGroup>

<ItemGroup>
    <PackageReference Include="Microsoft.AspNetCore.Components.WebAssembly" Version="6.0.0-rc.2.21480.10"/>
    <PackageReference Include="Microsoft.AspNetCore.Components.WebAssembly.DevServer" Version="6.0.0-rc.2.21480.10" PrivateAssets="all"/>
</ItemGroup>

...
```

If you wish to use a different version of .NET you will need to change the TargetFramework and Package References. There are a couple of ways to change the referenced package versions:

- Manually change the version numbers in the .csproj 
- Use the Nuget package manager in your IDE to downgrade the NuGet packages

You can also change the `TargetFramework` by manually updating the csproj or using your IDE to target a different version (for example net5.0).
