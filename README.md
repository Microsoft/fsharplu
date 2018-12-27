# FSharpLu F# library

This library provides F# lightweight utilities for string manipulations, logging, collection data structures, file operations, text processing, security, async, parsing, diagnostics, configuration files and Json serialization.

This is by no means a full-fledged utility library for F#, but rather a small collection of utilities and other thin wrappers accumulated throughout the development of various internal projects at Microsoft and meant to facilitate development with the .Net framework using the F# programming language.

Some of the provided utilities are just thin `let`-bindings wrappers around existing .Net libraries (e.g. module `FSharpLu.Text` or `FSharpLu.Parsing`) whereas some provide additional features (e.g. Json serialization in module `FSharpLu.Json`).


## Build status

| Branch | Status |
|--------|--------|
| current status | [![Build status](https://ci.appveyor.com/api/projects/status/y2lrc49c0lxprg77?svg=true)](https://ci.appveyor.com/project/blumu/fsharplu) |
|master | [![Build status](https://ci.appveyor.com/api/projects/status/y2lrc49c0lxprg77/branch/master?svg=true)](https://ci.appveyor.com/project/blumu/fsharplu/branch/master) |

## Build requirements

- F# compiler. See https://fsharp.org/use/Windows and https://fsharp.org/use/linux/

- Install .NET Core SDK from https://dotnet.microsoft.com/download/visual-studio-sdks.
    - .NET Core 2.2 SDK 
    - .NET Core 3.0 SDK 

- Install .NET Framework Developer Packs from https://www.microsoft.com/net/download/visual-studio-sdks 
for the following versions of .NET:
    - .NET Framework 4.5.2
    - .NET Framework 4.6.1
    - .NET Framework 4.6.2
    - .NET Framework 4.7.2


To build project run `dotnet build` under the top-level directory or run the script `scripts\build.ps1`.

## Documentation

For the documentation please visit the [Wiki](https://github.com/Microsoft/fsharplu/wiki)

## License

[MIT](LICENSE.MD)

## Packages

- `FSharpLu`: The core set of utilities
- `FSharpLu.Json`: Json serialization of F# data types implemented as JSon.Net converters and providing more succinct serialization for option types and discriminate unions.
- `FSharpLu.Tests`: Unit tests for the entire solution.

## FSharpLu modules

Here is a list of helper modules provided by FSharpLu. 
- [FSharp.Async](FSharpLu/Async.fs)
- [FSharp.Configuration](FSharpLu/Configuration.fs)
- [FSharp.Collection](FSharpLu/Collections.fs)
- [FSharp.Diagnostics](FSharpLu/Diagnostics.fs)
- [FSharp.ErrorHandling](FSharpLu/ErrorHandling.fs)
- [FSharp.File](FSharpLu/File.fs)
- [FSharp.Logger](FSharpLu/Logger.fs)
- [FSharp.Option](FSharpLu/Option.fs)
- [FSharp.Parsing](FSharpLu/Parsing.fs)
- [FSharp.Security](FSharpLu/Security.fs)
- [FSharp.Text](FSharpLu/Text.fs)
- [FSharp.TraceLogging](FSharpLu/TraceLogging.fs)



## Microsoft Open Source Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
