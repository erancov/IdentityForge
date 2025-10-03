# IdentityForge

**IdentityForge** is an **OpenIddict-powered Identity Server** with a built-in **Blazor Server Admin Dashboard**.  
It provides authentication, authorization, and management of applications, clients, scopes, roles, and users in a clean and modular architecture.

---

## ✨ Features

- 🔑 **OpenIddict Identity Server** – OAuth2 & OpenID Connect compliant
- 👤 **User & Role Management** – Create, update, assign roles
- 📦 **Application & Client Management** – Configure OAuth2/OIDC clients
- 🎯 **Scopes & Permissions** – Manage granular access scopes
- 📊 **Admin Dashboard** (Blazor) – Modern UI for managing identity resources
- 🧩 **Modular Architecture** – Separated into Domain, Application, Infrastructure, and Web layers

---

## 📂 Project Structure

```
src/
 ├── IdentityForge.Web/            # Blazor Admin Dashboard
 ├── IdentityForge.Application/    # Business logic (DTOs, Services)
 ├── IdentityForge.Domain/         # Core entities and enums
 └── IdentityForge.Infrastructure/ # EF Core, Repositories, OpenIddict integration
```

---

## 🚀 Getting Started

### 1. Clone the repo

bash
git clone https://github.com/erancov/IdentityForge.git
cd IdentityForge

### 2. Update connection string

Edit `appsettings.json` inside `IdentityForge.Web` to point to your database.

### 3. Run database migrations

bash
dotnet ef database update --project src/IdentityForge.Infrastructure

### 4. Launch the server

bash
dotnet run --project src/IdentityForge.Web

---

## 🛠️ Tech Stack

- **.NET 9** (Blazor Server, Web API)
- **OpenIddict** (OAuth2 / OpenID Connect)
- **Entity Framework Core**
- **ASP.NET Core Identity**
- **SQL Server / PostgreSQL (configurable)**

---

## 📜 License

This project is licensed under the MIT License.  
See [LICENSE](LICENSE) for more details.
