Store secrets locally using User Secrets:
---
From Package Manager Console (replace with your actual values):
---
dotnet user-secrets set "Authentication:Google:ClientId" "YOUR_REAL_CLIENT_ID" --project "Login Trial App/Login Trial App.csproj"
dotnet user-secrets set "Authentication:Google:ClientSecret" "YOUR_REAL_CLIENT_SECRET" --project "Login Trial App/Login Trial App.csproj"
--.
---
Appsettings
---
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=;Database=GoogleLoginTrialDB;Trusted_Connection=True;MultipleActiveResultSets=True;TrustServerCertificate=True"
  },

  "Logging": {
    "LogLevel": {
      "Default": "Information",
      "Microsoft.AspNetCore": "Warning"
    }
  },
  "AllowedHosts": "*",

  "Authentication": {
    "Google": {
      "ClientId": "",
      "ClientSecret": ""
    }
  }

}
