# Portfolio — Blazor WebAssembly (.NET 10)

A personal portfolio website built with Blazor WebAssembly targeting .NET 10. The main client project lives in the `BlazorApp` folder and uses component-based architecture.

## Quick info
- Framework: Blazor WebAssembly
- Target: .NET 10
- Client project: `BlazorApp`
- CI/CD: `.github/workflows/deploy.yml` (example GitHub Actions workflow)

## Prerequisites
- .NET 10 SDK (https://dotnet.microsoft.com)
- Git
- A code editor with Blazor support (Visual Studio, VS Code)

## Run locally (CLI)
1. Restore packages:

   `dotnet restore`

2. Build:

   `dotnet build`

3. Run the Blazor WebAssembly project:

   `dotnet run --project BlazorApp`

Open the URL printed to the console (commonly `https://localhost:5001`).

You can also use `dotnet watch run --project BlazorApp` for live reload during development.

## Run in Visual Studio
- Open the solution, set `BlazorApp` as the startup project and press F5 or use "Start Debugging".

## Publish
Produce a production build for static hosting:

`dotnet publish -c Release --project BlazorApp -o ./publish`

Serve the contents of `publish/wwwroot` from a static host (Azure Static Web Apps, GitHub Pages, CDN, etc.).

## Project layout (important files)
- `BlazorApp/Program.cs` — app startup
- `BlazorApp/App.razor` — root component and router
- `BlazorApp/Pages` — pages
- `BlazorApp/Components` — reusable UI components
- `BlazorApp/Shared` — layout and shared components (NavMenu, Footer, MainLayout)
- `BlazorApp/wwwroot` — static assets (CSS, JS, index.html)

## Contributing
1. Fork and create a feature branch.
2. Open a PR with a clear description.

## License
Add a `LICENSE` file to declare the project license (e.g., MIT).

---
This README was created to provide a concise reference for developing and publishing the Blazor WebAssembly application in this repository.
