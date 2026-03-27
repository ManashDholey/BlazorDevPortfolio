# 🚀 BlazorDevPortfolio

A developer portfolio web application built with **Blazor WebAssembly** and **ASP.NET Core Web API**, showcasing projects, skills, and professional information.

![.NET 7](https://img.shields.io/badge/.NET-7.0-purple)
![Blazor WASM](https://img.shields.io/badge/Blazor-WebAssembly-blue)
![Bootstrap 5](https://img.shields.io/badge/Bootstrap-5.0.2-violet)
![PWA](https://img.shields.io/badge/PWA-Enabled-green)

---

## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Configuration](#configuration)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

---

## 📖 About

**BlazorDevPortfolio** is a personal developer portfolio website built using the Blazor WebAssembly (WASM) framework. It follows a clean client-server architecture with a shared library, making it easy to extend and maintain. The application is designed to present your projects, skills, and professional background in a modern, responsive interface.

---

## ✨ Features

- **Blazor WebAssembly** – Full client-side SPA running in the browser via WebAssembly
- **Progressive Web App (PWA)** – Installable with offline support via service workers
- **Responsive Design** – Built with Bootstrap 5 for a mobile-first, responsive layout
- **ASP.NET Core Web API** – Backend API server with Swagger/OpenAPI documentation
- **Clean Architecture** – Separated into Client, Server, and Shared projects
- **Custom Styling** – Tailored CSS with custom backgrounds and shadow effects

---

## 🛠️ Tech Stack

| Layer      | Technology                                   |
|------------|----------------------------------------------|
| Frontend   | Blazor WebAssembly (.NET 7)                  |
| Backend    | ASP.NET Core Web API (.NET 7)                |
| Styling    | Bootstrap 5, Custom CSS, Open Iconic Icons   |
| API Docs   | Swagger / Swashbuckle                        |
| PWA        | Service Workers                              |
| Language   | C#, HTML, CSS, JavaScript                    |

---

## 📁 Project Structure

```
BlazorDevPortfolio/
├── BlazorDevPortfolio.sln          # Solution file
│
├── DevPortfolioClient/             # Blazor WebAssembly Client
│   ├── App.razor                   # Root application component
│   ├── Program.cs                  # Client entry point & service configuration
│   ├── _Imports.razor              # Global Razor imports
│   ├── DevPortfolioClient.csproj   # Client project file
│   ├── Pages/
│   │   └── Public/
│   │       └── Index.razor         # Home / Landing page
│   ├── Shared/
│   │   ├── MainLayout.razor        # Main layout component
│   │   └── MainLayout.razor.css    # Scoped layout styles
│   ├── Properties/
│   └── wwwroot/
│       ├── index.html              # HTML host page
│       ├── manifest.json           # PWA manifest
│       ├── service-worker.js       # Service worker (dev)
│       ├── service-worker.published.js  # Service worker (prod)
│       ├── css/
│       │   ├── app.css             # Custom application styles
│       │   ├── bootstrap/          # Bootstrap CSS
│       │   └── open-iconic/        # Open Iconic icon set
│       ├── assets/                 # Static assets (images, etc.)
│       └── sample-data/            # Sample JSON data
│
├── DevPortfolioServer/             # ASP.NET Core Web API Server
│   ├── Program.cs                  # Server entry point & middleware config
│   ├── DevPortfolioServer.csproj   # Server project file
│   ├── Controllers/
│   │   └── WeatherForecastController.cs  # Sample API controller
│   ├── WeatherForecast.cs          # Weather forecast model
│   ├── Properties/
│   ├── appsettings.json            # App configuration
│   └── appsettings.Development.json # Dev environment config
│
└── DevPortfolioShared/             # Shared Class Library
    └── DevPortfolioShared.csproj   # Shared project file
```

---

## ⚙️ Prerequisites

- [.NET 7.0 SDK](https://dotnet.microsoft.com/download/dotnet/7.0) or later
- A code editor like [Visual Studio 2022](https://visualstudio.microsoft.com/) or [VS Code](https://code.visualstudio.com/)
- (Optional) A modern browser with WebAssembly support

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/ManashDholey/BlazorDevPortfolio.git
cd BlazorDevPortfolio
```

### 2. Restore dependencies

```bash
dotnet restore
```

### 3. Run the Server project

```bash
cd DevPortfolioServer
dotnet run
```

The API server will start and Swagger UI will be available at `https://localhost:<port>/swagger` in development mode.

### 4. Run the Client project

Open a new terminal:

```bash
cd DevPortfolioClient
dotnet run
```

Navigate to the URL shown in the terminal (typically `https://localhost:5001` or similar).

### Alternative: Run both using the solution

```bash
dotnet run --project DevPortfolioServer
```

Or open `BlazorDevPortfolio.sln` in Visual Studio and press **F5** to run with debugging.

---

## 🔧 Configuration

- **Server settings** are in `DevPortfolioServer/appsettings.json` and `appsettings.Development.json`.
- **Client base URL** is configured in `DevPortfolioClient/Program.cs` using `builder.HostEnvironment.BaseAddress`.
- **PWA manifest** can be customized in `DevPortfolioClient/wwwroot/manifest.json`.

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is open source. Feel free to use it as a template for your own portfolio.

---

## 👤 Author

**Manash Dholey** — [GitHub Profile](https://github.com/ManashDholey)

---

> *"I am a software developer that specializes in .NET and Azure web development. Solving problems with software is fun to me."*
