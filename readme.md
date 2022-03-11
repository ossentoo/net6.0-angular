This is a .net 6.0 asp.net application with the Angular template as created by Visual Studio 2022


to publish and run this project:

- Open the project in VS Code
- Open a terminal window
- Navigate to the Project2 project directory (the same directory that the csproj file is located)
- run "dotnet project -c Release".  Notice how ng build --prod is executed as part of the public
- run the published project by typing:  "dotnet .\bin\Release\net6.0\publish\Project

The project should start running and output something similar to  the following:

info: Microsoft.Hosting.Lifetime[14]
      Now listening on: http://localhost:5000
info: Microsoft.Hosting.Lifetime[14]
      Now listening on: https://localhost:5001
info: Microsoft.Hosting.Lifetime[0]
      Application started. Press Ctrl+C to shut down.
info: Microsoft.Hosting.Lifetime[0]
      Hosting environment: Production
info: Microsoft.Hosting.Lifetime[0]

- Open a browser and navigate to https://localhost:5001.  Notice how the site responds with a 404 error.

Why is this happening and how can it be fixed?  This is important because when this project is published to an Azure App Service, the same 404 error occurs