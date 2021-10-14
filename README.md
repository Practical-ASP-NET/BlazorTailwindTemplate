# Blazor Tailwind Project Template for `dotnet new`

## Install template via nuget

``` bash
dotnet new --install PracticalDotNet.TailwindStarterProject::6.0.0-rc2.1
```

## Install template from source

Download the source then you can install template 'offline'.

```bash
cd content
dotnet new --install .
```

## Spin up a new project using the template

Once you have the template installed it will show up in the list of templates for `dotnet new`.

``` bash
dotnet new -l
```

Here's how it should appear in the list…

``` bash
Blazor WASM Tailwind Project Template         blazor-tailwind      [C#]
```

Here's how you can spin up a new project…

``` bash
dotnet new blazor-tailwind - o ExampleApp
cd ExampleApp
dotnet watch
```

This example creates the project in ExampleApp then launches it using `dotnet watch`.
