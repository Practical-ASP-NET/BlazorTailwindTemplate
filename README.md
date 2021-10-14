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
