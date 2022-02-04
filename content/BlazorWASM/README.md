# Tailwind JIT Mode

Tailwind (since V3) now runs in "JIT" mode.

This means it's designed to run in --watch mode during development, watching your markup/stylesheets and rebuilding its CSS file as you make changes.

The easiest way to make that work when working on a Blazor project which is not ASP.NET Hosted (standalone) is to manually launch the Tailwind CLI when you're working on your project.

To launch Tailwind JIT mode you can use this command (in the root of your project, wherever the `package.json` file is).

``` bash
npm run buildcss:watch
```

This will keep Tailwind running. Then you can launch your project as normal.