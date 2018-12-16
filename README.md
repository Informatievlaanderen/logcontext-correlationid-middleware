# Be.Vlaanderen.Basisregisters.AspNetCore.Mvc.Middleware.AddCorrelationIdLogContext

Middleware component which adds the correlation id to the Serilog `LogContext`.

## Usage

```csharp
public void Configure(IApplicationBuilder app, ...)
{
    app
        ...
        .UseMiddleware<AddCorrelationIdToLogContextMiddleware>()
        .UseMiddleware<AddCorrelationIdToResponseMiddleware>()
        .UseMiddleware<AddCorrelationIdMiddleware>()
        ...
}
```
