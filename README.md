# How to create a Custom Web API Template

1. Create your solution structure: folders, projects, readme, gitignore, ...

2. In the root of the project folder, create a folder named: .template.config 

3. Inside that folder, create a template.json file with your template configuration

4. Use the dotnet command to pack the template into a NuGet package (.nupkg)
    dotnet new install ./

5. Test the template
    dotnet new mycustomapi -n MyNewProject