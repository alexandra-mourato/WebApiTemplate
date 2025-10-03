# How to create a Custom Web API Template

1. Create your base project with your structure (ex: folders, projects, readme, gitignore, etc)
   - _dotnet new webapi -n MyCustomApiBase_

3. In the project root, create a folder _.template.config_ with a _template.json_ file:
   
       {
          "$schema": "http://json.schemastore.org/template",
          "author": "Your Name",
          "classifications": [ "Web", "API" ],
          "identity": "MyCompany.Templates.WebApi",
          "name": "Custom Web API Template",
          "shortName": "mycustomapi",
          "sourceName": "MyCustomApiBase",
          "preferNameDirectory": true
        }
4. Pack the template into a NuGet package (.nupkg)
    - _dotnet new install ./_

7. Test the template
    - _dotnet new mycustomapi -n MyNewProject_
