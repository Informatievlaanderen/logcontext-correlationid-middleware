# Be.Vlaanderen.Basisregisters.AspNetCore.Mvc.Middleware.AddCorrelationIdLogContext [![Build Status](https://github.com/Informatievlaanderen/logcontext-correlationid-middleware/workflows/CI/badge.svg)](https://github.com/Informatievlaanderen/logcontext-correlationid-middleware/actions)

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
