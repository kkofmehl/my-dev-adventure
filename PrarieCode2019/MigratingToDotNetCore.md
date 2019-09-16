# Migrating To .NET Core

## Speaker

Javier Lozano
javier@lozanotek.com

https://www.github.com/jglozano/migrate-net-core

## Notes:

- Look into gRPC for server => server communication as opposed to HTTP
    - Good for high through-put
    - Alternative to REST??

- Project File TidBits
    - `<AspNetCoreHostingModel>InProcess</AspNetCoreHostingModel>`

- !!! CsvHelper has a .NET Core version

- `IConfiguration` - Instead of .GetSection(), we can use `configuration["item.config"]`

- Any special directories that need to be created should be created (Project file code can do this)

- Look further into url compression within IIS (Web.config) settings

## Porting Process
- Can search Microsoft Docs: `Porting from .NET Framework`
- Identity Dependencies
- Target .NET Standard 2.0 (Plan A)
- Target .NET 4.7.2 ( OR HIGHER) and then move to .NET Standard 2.0 (Plan B)
- Use the .NET Portability Analyzer  (Visual Studio Ad-in)
    - Generates report of how portable our code is to .NET Core/Standard
- Use the .NET API Analyzer  (Console Application)
    - Find the gotchas for other platforms (linux, etc)
    - Cross-platform runtime support
- Try to avoid re-writes. If it can't be done, it can't be done. 

## Not in .NET Core
- AppDomains
- Remoting
    - Use System.IO.Pipes, Kestrel _(host, not the webserver)_, Sockets, gRPC
- Code Access Security
- System.EnterpriseServices

## ASP.NET MVC => ASP.NET Core (quick way)
- Create new ASP.NET Core project with the _same name_
- Copy/Paste all files
- Global.asax => Startup.cs
- Move content (js, css, img, etc.) to wwwroot
- Wire-up dependency injection
- Change namespace refs
- Handle `HttpContext` references
    - Can be tricky
- Delete files that are not needed



Questions:

Is there something similiar to AutoFac Modules in Microsoft's Dependency Injection library?