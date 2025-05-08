# FE-PusdatinATRBPN

# PlacesFrontend

A simple ASP.NET Core MVC frontend to consume a RESTful API for managing Places.
This project includes CRUD operations and displays the data using Bootstrap 5.

## Features

* List all places
* View details of a place
* Create a new place
* Edit existing place
* Delete a place
* Client-side and server-side validation
* Bootstrap 5 integration for UI

## Tech Stack

* ASP.NET Core MVC (.NET 8)
* Bootstrap 5 (via CDN)
* HttpClient for API communication
* Model validation with Data Annotations

## Requirements

* .NET 8 SDK
* Visual Studio 2022 or later (optional)
* A running REST API backend (e.g., [https://localhost:5001/api/places](https://localhost:5001/api/places))

## Getting Started

1. **Clone this repository**

   ```bash
   git clone https://github.com/your-username/PlacesFrontend.git
   cd PlacesFrontend
   ```

2. **Configure the API URL**

   In `Services/PlaceService.cs`, update the `_apiUrl` to point to your API backend:

   ```csharp
   private readonly string _apiUrl = "https://localhost:5001/api/places";
   ```

3. **Run the project**

   ```bash
   dotnet run
   ```

   Or open the `.csproj` file in Visual Studio and press **F5**.

4. **Browse the App**
   Go to `https://localhost:5001` or the port shown in your terminal.

## Folder Structure

```
PlacesFrontend/
│
├── Controllers/           # MVC Controllers
├── Models/                # Data models
├── Services/              # HTTP client to consume API
├── Views/                 # Razor views (UI)
│   └── Places/            # Views for Places controller
├── wwwroot/               # Static files (optional)
├── Program.cs             # App startup and configuration
└── README.md              # This file
```

## Notes

* Ensure the backend API supports CORS or is hosted on the same domain for smooth interaction.
* No login or authentication is implemented. The app assumes open access to the API.

## License

This project is licensed under the MIT License.
