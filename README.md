GeoTimeZone.StrongNamed  [![NuGet Version](https://img.shields.io/nuget/v/GeoTimeZone.StrongNamed.svg?style=flat)](https://www.nuget.org/packages/GeoTimeZone.StrongNamed/) 
===========

This is a fork of the original project [GeoTimeZone][4]

Provides a StrongNamed Package Version of the original GeoTimeZone which provides an IANA time zone identifier from latitude and longitude coordinates.

## Nuget Installation

```powershell
PM> Install-Package GeoTimeZone.StrongNamed
```

# From the Original Readme.md File


## Supported Environments

As of version 3.0, this library is targeting .NET Standard 1.1+, .NET Standard 2.0+, and .NET Framework 4.0+.
See the [.NET Standard Platform Support Matrix](https://docs.microsoft.com/en-us/dotnet/articles/standard/library) for further details.

## Example Usage

```csharp
string tz = TimeZoneLookup.GetTimeZone(50.4372, -3.5559).Result;  // "Europe/London"
```

## Usage Notes

This library uses the time zone border definitions from the [Timezone Boundary Builder][1] project,
which in-turn derive from [Open Street Map][2].  As some international borders are the subject of dispute,
the results may or may not align with your worldview.  Use at your own risk.

## License

This library is provided free of charge, under the terms of the [MIT license][3].


[1]: https://github.com/evansiroky/timezone-boundary-builder
[2]: https://www.openstreetmap.org/
[3]: https://raw.githubusercontent.com/mj1856/GeoTimeZone/master/LICENSE
[4]: https://github.com/mj1856/GeoTimeZone
