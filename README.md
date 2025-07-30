# hairsalonapp-api

ASP.NET Core API for handling email notifications for the Hair Salon App.

### Prerequisites

- .NET 9.0 SDK
- Visual Studio 2022 (17.12 or later) or Visual Studio Code
- Docker Desktop
- Email service configuration (e.g., SMTP settings for `blueskiessalon@gmail.com`)

### Setup

1. Clone or download the repository from GitHub.
2. Open `hairsalonapp-api.sln` in Visual Studio or VS Code.
3. Restore NuGet packages (e.g., `Microsoft.AspNetCore.Mvc`, `MailKit`).
4. Configure `appsettings.json` with your SMTP settings (use `appsettings.example.json` as a template).
5. Run the API:
   - Visual Studio: Set as startup project, run (Debug | Any CPU).
   - Docker:
     ```bash
     docker build -t hairsalonapp-api .
     docker run -d -p 8080:8080 hairsalonapp-api
