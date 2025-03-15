# Blazor Web App with Tailwind CSS

![GitHub Repo stars](https://img.shields.io/github/stars/guanhaowu/BlazorServerWebshop?style=flat-square)
![GitHub forks](https://img.shields.io/github/forks/guanhaowu/BlazorServerWebshop?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/guanhaowu/BlazorServerWebshop?style=flat-square)
![GitHub pull requests](https://img.shields.io/github/issues-pr/guanhaowu/BlazorServerWebshop?style=flat-square)
![GitHub](https://img.shields.io/github/license/guanhaowu/BlazorServerWebshop?style=flat-square)


## 📌 Project Overview
This is a **Blazor Web App** built with **.NET 9** and integrated with **Tailwind CSS v4** for styling. The project includes automated build scripts for **development, production, and testing**, ensuring an efficient and optimized workflow.

## 🚀 Features
- **Blazor Web App** (C# .NET 9)
- **Tailwind CSS v4** for modern UI styling
- **Live-reload development** with `dotnet watch` and `tailwindcss --watch`
- **Production-ready builds** with minified Tailwind CSS and optimized .NET output
- **Automated testing and formatting** for cleaner code

## 📂 Project Structure
```
📦 Project Root
 ┣ 📂 Components # Contains UI layout, components and pages
 ┃ ┗ 📂 Layout
 ┃ ┗ 📂 Pages
 ┃ ┗ 📂 Shared
 ┃ ┗ 📜 _Imports.razor
 ┃ ┗ 📜 App.razor
 ┃ ┗ 📜 Routes.razor
 ┣ 📂 Properties # Contains launch settings
 ┃ ┗ 📜 launchSettings.json # Configuration for debugging and hosting
 ┣ 📂 wwwroot
 ┃ ┣ 📂 css
 ┃ ┃ ┗ 📜 tailwind.css  # Compiled Tailwind output
 ┃ ┗ 📜 app.css  # Tailwind input file
 ┣ 📜 appsettings.json  # Global configuration settings
 ┣ 📜 appsettings.Development.json  # Development-specific settings
 ┣ 📜 Program.cs
 ┣ 📜 package.json
 ┣ 📜 package-lock.json  # Locks dependencies to ensure consistency
 ┣ 📜 .csproj
 ┣ 📜 README.md
```

## 🛠️ Requirements
Before running this project, ensure you have the following installed:

1. **.NET 9 SDK** - Download from [dotnet.microsoft.com](https://dotnet.microsoft.com/)
2. **Node.js (LTS version)** - Download from [nodejs.org](https://nodejs.org/)
3. **npm (comes with Node.js)** - Used for managing dependencies and scripts.

## 🛠️ Setup & Installation
### **1. Install Dependencies**
```sh
npm install
```

### **2. Restore .NET Dependencies**
```sh
dotnet restore
```

## 🔧 Development
Run the following command to start the Blazor Web App **with live Tailwind updates**:
```sh
npm run start
```
This will:
- Start `dotnet watch` to automatically reload Blazor.
- Start `tailwindcss --watch` to automatically compile styles.

## 🎯 Production Build
To generate an optimized **production build**:
```sh
npm run build:prod
```
This will:
- **Minify Tailwind CSS**.
- **Publish the Blazor app** with **trimming and compression**.

## ✅ Testing & Formatting
### **Run Tests**
```sh
npm run test
```
### **Format C# Code**
```sh
npm run format
```

## 📜 Scripts Reference
| Command                  | Description                                     |
|--------------------------|-------------------------------------------------|
| `npm run restore`        | Restores .NET dependencies.                     |
| `npm run build`          | Rebuilds the project in Debug mode.             |
| `npm run build:prod`     | Builds and minifies for production.             |
| `npm run tailwind:watch` | Runs Tailwind CSS in watch mode.                |
| `npm run tailwind:build` | Builds and minifies Tailwind CSS.               |
| `npm run dev`            | Runs Blazor in watch mode.                      |
| `npm run start`          | Runs Blazor & Tailwind watch mode concurrently. |
| `npm run test`           | Runs Blazor unit tests.                         |
| `npm run format`         | Formats C# code using `dotnet format`.          |
