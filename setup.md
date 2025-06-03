# Setup

## Prerequisites

- .NET 8 SDK or higher
- Git
- Optional: Visual Studio 2022 or Visual Studio Code

## Step-by-Step Instructions

1. **Clone the repository**
   ```powershell
   git clone <REPO-URL>
   cd projectDocumentation
   ```
2. **Restore dependencies**
   ```powershell
   dotnet restore
   ```
3. **Migrate the database (if required)**
   ```powershell
   dotnet ef database update
   ```
4. **Build the project**
   ```powershell
   dotnet build
   ```
5. **Run the project**
   ```powershell
   dotnet run
   ```
6. **Run tests**
   ```powershell
   dotnet test
   ```

## Environment Variables (Example)

If needed, set the following environment variables (e.g., in a `.env` file or project settings):

- `ConnectionStrings__DefaultConnection` – Connection string for SQLite
- `ASPNETCORE_ENVIRONMENT` – e.g., `Development` or `Production`

## Notes

- Data is stored in JSON, XML, and flat files in the `Data` directory.
- Log files are located at `Data/logs.txt`.
- Sample data can be generated via a seed script or on first run.
