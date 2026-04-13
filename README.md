# Awesome F# [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) <img src="https://fsharp.org/img/logo/fsharp.svg" width="48" height="48" align="right"/> with stars

F# is a programming language with focus on immutability, type inference, first-class functions, powerful data types and pattern matching, targeting .NET and other platforms.

This is a curated list of awesome F# frameworks, libraries, software and resources.

## Contents

* [Main Language-Related Repositories](#main-language-related-repositories)
* [F# Wrappers for Popular .NET Libraries](#f-wrappers-for-popular-net-libraries)
* [Actor Frameworks](#actor-frameworks)
* [Build Tools](#build-tools)
* [Cloud](#cloud)
* [Code Analysis](#code-analysis)
* [Code Generation](#code-generation)
* [Compilers for Other Platforms](#compilers-for-other-platforms)
* [Concurrent, Asynchronous, and Parallel Programming](#concurrent-asynchronous-and-parallel-programming)
* [Configuration](#configuration)
* [Data Science](#data-science)
* [Development Tools](#development-tools)
  * [IDE](#ide)
  * [Editor Plugins](#editor-plugins)
  * [Performance Analysis](#performance-analysis)
* [General Purpose Libraries](#general-purpose-libraries)
* [Game Development](#game-development)
* [GUI](#gui)
* [HTTP Clients](#http-clients)
* [Logging](#logging)
* [Package Management](#package-management)
* [Parsing](#parsing)
* [Serialization](#serialization)
* [Simulation](#simulation)
* [Static Site Generators](#static-site-generators)
* [Testing](#testing)
* [Type Providers](#type-providers)
  * [Creating Type Providers](#creating-type-providers)
* [Visualization](#visualization)
* [Web Frameworks](#web-frameworks)
* [.NET Core Templates](#net-core-templates)
* [Resources](#resources)
  * [Blogs](#blogs)
  * [Books](#books)
  * [Cheatsheets](#cheatsheets)
  * [Community](#community)
  * [Other Lists](#other-lists)
  * [Websites](#websites)
  * [Videos](#videos)
  * [Courses](#courses)

## Main Language-Related Repositories

* [F# main repository](https://github.com/dotnet/fsharp) ⭐ 4,276 | 🐛 1,285 | 🌐 F# | 📅 2026-04-13
* [F# RFCs](https://github.com/fsharp/fslang-design) ⭐ 547 | 🐛 28 | 🌐 F# | 📅 2026-03-10
* [F# suggestions](https://github.com/fsharp/fslang-suggestions) ⭐ 369 | 🐛 344 | 📅 2025-02-27
* [F# projects](https://github.com/fsprojects)

## F# Wrappers for Popular .NET Libraries

Looking to have a more enjoyable experience when consuming a popular .NET library? Here is a quick table.

<!-- The following table includes some entries that are duplicated in the list below. This is by design. -->  

<!--lint disable double-link -->

| .NET Library                                                                                                                                                                                                                                                       | F# Wrapper                                                                                                                                                                                                                                                                                              |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [ASP.NET Core Blazor](https://github.com/dotnet/aspnetcore/tree/main/src/Components) ⭐ 37,827 \| 🐛 3,859 \| 🌐 C# \| 📅 2026-04-12                                                                                                                                | [Bolero](https://github.com/fsbolero/Bolero) ⭐ 1,127 \| 🐛 73 \| 🌐 F# \| 📅 2025-10-26                                                                                                                                                                                                                 |
| [ASP.NET Core](https://github.com/dotnet/aspnetcore) ⭐ 37,827 \| 🐛 3,859 \| 🌐 C# \| 📅 2026-04-12                                                                                                                                                                | [Giraffe](https://github.com/giraffe-fsharp/Giraffe) ⭐ 2,237 \| 🐛 46 \| 🌐 F# \| 📅 2026-04-11 (+ optionally [Saturn](https://github.com/SaturnFramework/Saturn) ⭐ 724 \| 🐛 55 \| 🌐 F# \| 📅 2024-07-31)<br/>[Oxpecker](https://github.com/Lanayx/Oxpecker) ⭐ 405 \| 🐛 10 \| 🌐 F# \| 📅 2026-04-08 |
| [Avalonia](https://github.com/AvaloniaUI/Avalonia) ⭐ 30,563 \| 🐛 1,888 \| 🌐 C# \| 📅 2026-04-11                                                                                                                                                                  | [Avalonia.FuncUI](https://github.com/fsprojects/Avalonia.FuncUI) ⭐ 1,213 \| 🐛 19 \| 🌐 F# \| 📅 2026-04-08                                                                                                                                                                                             |
| [MAUI](https://github.com/dotnet/maui) ⭐ 23,217 \| 🐛 4,028 \| 🌐 C# \| 📅 2026-04-12/[Xamarin.Forms](https://github.com/xamarin/Xamarin.Forms) ⚠️ Archived                                                                                                        | [Fabulous](https://github.com/fabulous-dev/Fabulous) ⭐ 1,255 \| 🐛 13 \| 🌐 F# \| 📅 2025-11-14                                                                                                                                                                                                         |
| [MSTest](https://github.com/microsoft/testfx) ⭐ 998 \| 🐛 205 \| 🌐 C# \| 📅 2026-04-13/[NUnit](https://github.com/nunit/nunit) ⭐ 2,619 \| 🐛 258 \| 🌐 C# \| 📅 2026-04-13/[xUnit.net](https://github.com/xunit/xunit) ⭐ 4,558 \| 🐛 56 \| 🌐 C# \| 📅 2026-04-12 | [FsUnit](https://github.com/fsprojects/FsUnit) ⭐ 445 \| 🐛 6 \| 🌐 F# \| 📅 2025-07-11                                                                                                                                                                                                                  |
| [System.Text.Json](https://github.com/dotnet/runtime/tree/main/src/libraries/System.Text.Json) ⭐ 17,799 \| 🐛 8,234 \| 🌐 C# \| 📅 2026-04-13                                                                                                                      | [FSharp.SystemTextJson](https://github.com/Tarmil/FSharp.SystemTextJson) ⭐ 365 \| 🐛 42 \| 🌐 F# \| 📅 2026-03-04                                                                                                                                                                                       |
| [WPF](https://github.com/dotnet/wpf) ⭐ 7,613 \| 🐛 1,625 \| 🌐 C# \| 📅 2026-04-12                                                                                                                                                                                 | [Elmish.WPF](https://github.com/elmish/Elmish.WPF) ⭐ 463 \| 🐛 61 \| 🌐 F# \| 📅 2024-10-01                                                                                                                                                                                                             |

<!--lint enable double-link -->

## Actor Frameworks

* [Orleans](https://github.com/dotnet/orleans) ⭐ 10,755 | 🐛 714 | 🌐 C# | 📅 2026-04-11 - Distributed virtual actor model.
* [Akka.NET](https://github.com/akkadotnet/akka.net) ⭐ 5,036 | 🐛 416 | 🌐 C# | 📅 2026-04-10 - Community-driven port of the popular Java/Scala framework Akka to .NET.
* [Proto.actor](https://github.com/AsynkronIT/protoactor-dotnet) ⭐ 1,883 | 🐛 21 | 🌐 C# | 📅 2026-03-13 - Cross-platform actor framework for .NET, Go, Java and Kotlin.
* [Orleankka](https://github.com/OrleansContrib/Orleankka) ⭐ 506 | 🐛 3 | 🌐 C# | 📅 2025-12-15 - Functional extension for Microsoft Orleans framework.
* [Akkling](https://github.com/Horusiath/Akkling) ⭐ 232 | 🐛 10 | 🌐 F# | 📅 2026-04-08 - F# typed API for Akka.NET.

## Build Tools

* [FAKE](https://github.com/fsharp/FAKE) ⭐ 1,332 | 🐛 51 | 🌐 F# | 📅 2025-11-26 - "F# Make" is a cross platform build automation system.
* [Xake](https://github.com/OlegZee/Xake) ⭐ 5 | 🐛 0 | 🌐 F# | 📅 2026-03-18 - Another Make utility implementation on F#, fully declarative with no-brain parallelism, inspired by Shake.

## Cloud

* [Farmer](https://github.com/CompositionalIT/farmer) ⭐ 544 | 🐛 108 | 🌐 F# | 📅 2026-04-11 - Repeatable Azure deployments with ARM templates made easy.
* [Pulumi.FSharp.Extensions](https://github.com/UnoSD/Pulumi.FSharp.Extensions) ⭐ 98 | 🐛 3 | 🌐 F# | 📅 2026-02-28 - F# computational expressions to reduce boilerplate in Pulumi code.
* [FsFirestore](https://github.com/mrbandler/FsFirestore) ⭐ 26 | 🐛 2 | 🌐 F# | 📅 2021-04-11 - Functional F# library to access Firestore database hosted on Google Cloud Platform (GCP) or Firebase.
* [Chia](https://github.com/DanpowerGruppe/Chia) ⭐ 12 | 🐛 31 | 🌐 CSS | 📅 2023-01-06 - An F# library which contains HelperFunctions for reporting, logging and Azure cloud operations.

## Code Analysis

* [Ionide FSharp.Analyzers.SDK](https://github.com/ionide/FSharp.Analyzers.SDK) ⭐ 85 | 🐛 37 | 🌐 F# | 📅 2026-03-30 - Library for building custom analyzers for F# / FSharp.Analyzers.Cli.

## Code Generation

* [Myriad](https://github.com/MoiraeSoftware/myriad) ⭐ 378 | 🐛 33 | 🌐 F# | 📅 2026-03-30 - A pre-compilation code generator.
* [Hawaii](https://github.com/Zaid-Ajaj/Hawaii) ⭐ 160 | 🐛 17 | 🌐 F# | 📅 2024-04-08 - A dotnet CLI tool to generate type-safe F# clients from OpenAPI/Swagger services.

## Compilers for Other Platforms

* [Fable](https://github.com/fable-compiler/Fable) ⭐ 3,069 | 🐛 227 | 🌐 F# | 📅 2026-04-13 - F# to JavaScript compiler.
* [FunScript](https://github.com/ZachBray/FunScript) ⭐ 445 | 🐛 47 | 🌐 F# | 📅 2017-02-14 - F# to JavaScript compiler with JQuery etc. mappings through a TypeScript type provider.
* [Fez](https://github.com/kjnilsson/fez) ⭐ 284 | 🐛 12 | 🌐 F# | 📅 2019-05-16 - F# to Erlang compiler.
* [Juniper](https://github.com/calebh/Juniper) ⭐ 102 | 🐛 8 | 🌐 F# | 📅 2024-11-16 - Functional Reactive Programming for the Arduino and other microcontrollers.

## Concurrent, Asynchronous, and Parallel Programming

* [Hopac](https://github.com/Hopac/Hopac) ⭐ 536 | 🐛 32 | 🌐 F# | 📅 2022-02-24 - Concurrent ML style concurrent programming library for F#.
* [Ply](https://github.com/crowded/ply) ⭐ 245 | 🐛 4 | 🌐 F# | 📅 2022-11-30 - High performance System.Threading.(Value)Task computation expressions for F#.
* [TaskBuilder.fs](https://github.com/rspeele/TaskBuilder.fs) ⭐ 234 | 🐛 9 | 🌐 F# | 📅 2021-01-31 - F# computation expression builder for System.Threading.Tasks.
* [FSharp.Control.AsyncSeq](https://github.com/fsprojects/FSharp.Control.AsyncSeq) ⭐ 173 | 🐛 1 | 🌐 F# | 📅 2026-04-13 - Asynchronous sequence support, integration with `IAsyncEnumerable`.
* [FSharp.Control.FusionTasks](https://github.com/kekyo/FSharp.Control.FusionTasks) ⭐ 162 | 🐛 2 | 🌐 F# | 📅 2022-11-12 - F# Async workflow <--> .NET Task/ValueTask easy seamless interoperability library.
* [IcedTasks](https://github.com/TheAngryByrd/IcedTasks) ⭐ 149 | 🐛 4 | 🌐 F# | 📅 2025-11-21 - Cold tasks, cancellable tasks, and extensions for the `async` workflow.
* [Reaction.AsyncRx](https://github.com/dbrattli/Reaction) ⭐ 143 | 🐛 103 | 🌐 F# | 📅 2023-01-06 - An implementation of Async Observables in F# for .NET and Fable.
* [FSharpx.Async](https://github.com/fsprojects/FSharpx.Async) ⭐ 95 | 🐛 20 | 🌐 F# | 📅 2024-01-12 - Collection of asynchronous programming utilities for F#.
* [FIO](https://github.com/iyyel/fio) ⭐ 77 | 🐛 0 | 🌐 F# | 📅 2026-04-12 - A type-safe, highly concurrent and asynchronous library for F# based on pure functional programming.

## Configuration

* [Argu](https://github.com/fsprojects/Argu) ⭐ 483 | 🐛 27 | 🌐 F# | 📅 2026-03-30 - Declarative CLI argument/XML configuration parser for F# applications.
* [FsConfig](https://github.com/demystifyfp/FsConfig) ⭐ 170 | 🐛 5 | 🌐 F# | 📅 2023-10-24 - F# library for reading configuration data from environment variables and AppSettings with type safety.
* [docopt.fs](https://github.com/docopt/docopt.fs/) ⭐ 36 | 🐛 0 | 🌐 F# | 📅 2020-01-15 - Command line arguments parser, F# port of [docopt](https://github.com/docopt/docopt) ⭐ 8,011 | 🐛 266 | 🌐 Python | 📅 2025-06-23.
* [Skid](https://github.com/Meyhem/Skid) ⭐ 5 | 🐛 0 | 🌐 F# | 📅 2022-08-16 - Simple, single-file portable CLI utility for configuration templating.

## Data Science

* [Math.NET Numerics](https://github.com/mathnet/mathnet-numerics) ⭐ 3,728 | 🐛 326 | 🌐 C# | 📅 2025-03-03 - Methods and algorithms for numerical computations in science, engineering and every day use. F# specific bindings available.
* [m2cgen](https://github.com/BayesWitnesses/m2cgen) ⭐ 2,970 | 🐛 62 | 🌐 Python | 📅 2024-08-03 - A CLI tool to transpile trained classic ML models into a native F# code with zero dependencies.
* [Deedle](https://github.com/BlueMountainCapital/Deedle) ⭐ 998 | 🐛 5 | 🌐 F# | 📅 2026-04-13 - Exploratory data library for .NET.
* [DiffSharp](https://github.com/DiffSharp/DiffSharp) ⭐ 614 | 🐛 38 | 🌐 F# | 📅 2024-04-15 - Functional automatic differentiation (AD) library.
* [IfSharp](https://github.com/fsprojects/IfSharp) ⭐ 443 | 🐛 12 | 🌐 Jupyter Notebook | 📅 2022-03-17 - F# for Jupyter Notebooks.
* [Math.NET Symbolics](https://github.com/mathnet/mathnet-symbolics/) ⭐ 369 | 🐛 54 | 🌐 F# | 📅 2024-01-15 - A basic open source computer algebra library for .NET, Silverlight and Mono written entirely in F#.
* [SIMDArray](https://github.com/jackmott/SIMDArray) ⭐ 137 | 🐛 5 | 🌐 F# | 📅 2026-02-20 - SIMD enhanced Array extensions for faster computation.
* [Synapses](https://github.com/mrdimosthenis/Synapses) ⭐ 73 | 🐛 0 | 📅 2021-09-23 - Neural network library in F#.
* [FsLab](https://github.com/fslaborg/FsLab) ⭐ 34 | 🐛 5 | 🌐 F# | 📅 2024-04-19 - A collection of libraries for data-science. It provides a rapid development environment that lets you write advanced analysis with few lines of production-quality code.

## Development Tools

### IDE

* [F# Playground](https://github.com/Seng-Jik/FSharpPlayground) ⭐ 15 | 🐛 1 | 🌐 C# | 📅 2022-11-08 - Minimal playground for F#.
* [JetBrains Rider](https://www.jetbrains.com/rider) - Cross-platform .NET IDE with F# support (Proprietary, free for non-commercial use).
* [MonoDevelop](http://www.monodevelop.com/) - Cross-platform IDE mostly aimed at Mono/.NET developers.
* [Visual Studio](https://www.visualstudio.com/) - IDE from Microsoft with first class F# support (Windows only, Proprietary).

### Editor Plugins

* [Fantomas](https://github.com/fsprojects/fantomas) ⭐ 824 | 🐛 90 | 🌐 F# | 📅 2026-04-13 - F# code formatter.
* [VimSpeak](https://github.com/AshleyF/VimSpeak) ⭐ 418 | 🐛 4 | 🌐 F# | 📅 2020-09-09 - A tool to control Vim with your voice using speech recognition.
* [FSharpLint](https://github.com/fsprojects/FSharpLint) ⭐ 321 | 🐛 93 | 🌐 F# | 📅 2026-02-12 - F# code linter.
* [Emacs F# mode](https://github.com/fsharp/emacs-fsharp-mode) ⭐ 213 | 🐛 43 | 🌐 Emacs Lisp | 📅 2026-04-02 - F# support in Emacs (including Intellisense and Interactive mode).
* [FSharpFar](https://github.com/nightroman/FarNet) ⭐ 146 | 🐛 0 | 🌐 C# | 📅 2026-04-06 - F# support for Far Manager.
* [Vim F#](https://github.com/fsharp/vim-fsharp) ⚠️ Archived - F# support for Vim.
* [neofsharp.vim](https://github.com/adelarsq/neofsharp.vim) ⭐ 42 | 🐛 1 | 🌐 Vim Script | 📅 2024-04-06 - Basic F# support for (Neo)Vim.
* [fsharp-notebook](https://github.com/pablofrommars/fsharp-notebook) ⭐ 2 | 🐛 3 | 🌐 HTML | 📅 2023-03-03 - Data science notebook for F# Interactive.
* [Ionide](http://ionide.io/) - Atom Editor and Visual Studio Code package suite for cross platform F# development.

### Performance Analysis

* [fasm](https://github.com/d-edge/fasm) ⭐ 192 | 🐛 3 | 🌐 F# | 📅 2023-11-22 - F# JIT disassembler, as a dotnet tool.

## General Purpose Libraries

* [FSharpPlus](https://github.com/gmpl/FSharpPlus) ⭐ 937 | 🐛 66 | 🌐 F# | 📅 2026-02-13 - Extensions for F#.
* [FSharpx.Extras](https://github.com/fsprojects/FSharpx.Extras) ⭐ 697 | 🐛 10 | 🌐 F# | 📅 2025-12-20 - A collection of libraries and tools for use with F#.
* [FsToolkit.ErrorHandling](https://github.com/demystifyfp/FsToolkit.ErrorHandling) ⭐ 543 | 🐛 7 | 🌐 F# | 📅 2026-04-08 - Clear, simple and powerful error handling with railway-oriented programming. Inspired by Chessie.
* [FSharpLu](https://github.com/Microsoft/fsharplu) ⭐ 374 | 🐛 9 | 🌐 F# | 📅 2024-06-11 - Lightweight utilities for string manipulations, logging, collection data structures, file operations, text processing, security, async, parsing, diagnostics, configuration files and Json serialization.
* [Npgsql.FSharp](https://github.com/Zaid-Ajaj/Npgsql.FSharp) ⭐ 339 | 🐛 16 | 🌐 F# | 📅 2026-02-28 - Thin F# wrapper around [Npgsql](https://github.com/npgsql/npgsql) ⭐ 3,673 | 🐛 211 | 🌐 C# | 📅 2026-04-11, the PostgreSQL database driver.
* [TypeShape](https://github.com/eiriktsarpalis/TypeShape) ⭐ 321 | 🐛 0 | 🌐 F# | 📅 2025-02-07 - Small, extensible F# library for practical generic programming.
* [SqlHydra](https://github.com/JordanMarr/SqlHydra) ⭐ 261 | 🐛 9 | 🌐 F# | 📅 2026-04-06 - Suite of NuGet packages for working with databases in F# including query expressions and code generation tools (for generating strongly typed F# DTO record types based on your database tables). Supports MySQL, PostgreSQL, Oracle, SQL Server, and SQLite.
* [Fli](https://github.com/CaptnCodr/Fli) ⭐ 218 | 🐛 2 | 🌐 F# | 📅 2026-03-28 - Computational expression to run system processes and manage their output.
* [Donald](https://github.com/pimbrouwers/Donald) ⭐ 193 | 🐛 2 | 🌐 F# | 📅 2024-12-02 - A simple F# interface for ADO.NET.
* [Chessie](https://github.com/fsprojects/Chessie) ⭐ 187 | 🐛 15 | 🌐 F# | 📅 2018-08-26 - Railway-oriented programming.
* [LiteDB.FSharp](https://github.com/Zaid-Ajaj/LiteDB.FSharp) ⭐ 184 | 🐛 8 | 🌐 F# | 📅 2022-12-08 - F# Support for [LiteDB](https://github.com/mbdavid/LiteDB) ⭐ 9,382 | 🐛 745 | 🌐 C# | 📅 2026-03-13, an embedded single file database for .NET.
* [Aether](https://github.com/xyncro/aether) ⭐ 181 | 🐛 11 | 🌐 F# | 📅 2021-10-12 - Optics library for F#, similar to the Haskell Data.Lens package.
* [ExtCore](https://github.com/jack-pappas/ExtCore) ⭐ 180 | 🐛 19 | 🌐 F# | 📅 2021-11-07 - Extended core library for F#.
* [Validus](https://github.com/pimbrouwers/Validus) ⭐ 159 | 🐛 2 | 🌐 F# | 📅 2024-05-16 - A composable validation library for F#, with built-in validators for most primitive types and easily extended through custom validators.
* [Fumble](https://github.com/tforkmann/Fumble) ⭐ 115 | 🐛 3 | 🌐 CSS | 📅 2025-12-05 - Thin F# API for SQLite for easy data access to SQLite database with functional seasoning on top.
* [FSharp.CosmosDb](https://github.com/aaronpowell/fsharp.cosmosdb) ⭐ 82 | 🐛 7 | 🌐 F# | 📅 2024-09-03 - An F# wrapper around the CosmosDB SDK, making it more functional-friendly.
* [DustyTables](https://github.com/Zaid-Ajaj/DustyTables) ⭐ 81 | 🐛 8 | 🌐 F# | 📅 2024-01-16 - Thin F# API for SqlClient for easy data access to ms sql server with functional seasoning on top.
* [FSharp.HashCollections](https://github.com/mvkara/fsharp-hashcollections) ⭐ 69 | 🐛 5 | 🌐 F# | 📅 2024-04-07 - Fast hash-based immutable map and set.
* [Fling](https://github.com/cmeeren/Fling) ⭐ 48 | 🐛 0 | 🌐 F# | 📅 2025-12-19 - Significantly reduces boilerplate needed to efficiently save/load complex domain entities to/from multiple tables.
* [Vp.FSharp.Sql](https://github.com/veepee-oss/Vp.FSharp.Sql) ⭐ 35 | 🐛 11 | 🌐 F# | 📅 2024-11-25 - Generic F# ADO provider wrapper (SqlServer, PostgreSQL, SQLite).

## Game Development

* [Nu Game Engine](https://github.com/bryanedds/Nu) ⭐ 1,319 | 🐛 196 | 🌐 F# | 📅 2026-04-12 - Cross-platform F# 2D game engine built in the functional style. Uses SDL2 and Farseer Physics.
* [Garnet](https://github.com/bcarruthers/garnet) ⚠️ Archived - Lightweight game composition library for F# with entity-component-system (ECS) and actor-like messaging features.
* [FsUnity](https://github.com/FsUnity) - F# libraries, tools, and plugins for the Unity game engine.
* [Godot](https://www.lkokemohr.de/fsharp_godot.html) - Tutorial how to use F# with Godot.

## GUI

<!--lint disable double-link -->

* [Fabulous](https://github.com/fabulous-dev/Fabulous) ⭐ 1,255 | 🐛 13 | 🌐 F# | 📅 2025-11-14 - F# functional app development, using declarative dynamic UI.
* [Avalonia.FuncUI](https://github.com/fsprojects/Avalonia.FuncUI) ⭐ 1,213 | 🐛 19 | 🌐 F# | 📅 2026-04-08 - Develop cross-platform MVU GUI Applications using F# and Avalonia.
* [Elmish.WPF](https://github.com/elmish/Elmish.WPF) ⭐ 463 | 🐛 61 | 🌐 F# | 📅 2024-10-01 - Elmish (or MVU) approach to WPF programming.
* [Epoxy](https://github.com/kekyo/epoxy) ⭐ 255 | 🐛 4 | 🌐 C# | 📅 2024-12-10 - An independent flexible XAML MVVM library for .NET.

<!--lint enable double-link -->

## HTTP Clients

* [FsHttp](https://github.com/ronaldschlenker/FsHttp) ⭐ 499 | 🐛 30 | 🌐 F# | 📅 2026-04-01 - A convenient library for consuming HTTP/REST endpoints via F#.
* [Http.fs](https://github.com/haf/Http.fs) ⭐ 318 | 🐛 19 | 🌐 HTML | 📅 2023-08-02 - A simple, functional HTTP client library for F#.
* [Oryx](https://github.com/cognitedata/oryx) ⭐ 212 | 🐛 7 | 🌐 F# | 📅 2026-03-31 - A high performance .NET cross-platform functional HTTP request handler library for writing HTTP clients and orchestrating web requests.

## Logging

* [Logary](https://github.com/logary/logary/) ⭐ 532 | 🐛 71 | 🌐 F# | 📅 2023-05-18 - High performance, multi-target logging, metric, tracing and health-check library for mono and .NET.
* [FsLibLog](https://github.com/TheAngryByrd/FsLibLog) ⭐ 59 | 🐛 4 | 🌐 F# | 📅 2023-03-14 - A single file you can copy and paste or add through Paket GitHub dependencies to provide your F# library with a logging abstraction.

## Package Management

* [NuGet](https://www.nuget.org/) - The package manager for the Microsoft development platform including .NET.
* [Paket](https://github.com/fsprojects/Paket) ⭐ 2,086 | 🐛 782 | 🌐 F# | 📅 2026-01-20 - Dependency manager for .NET with support for NuGet packages and Git repositories.

## Parsing

* [FParsec](https://github.com/stephan-tolksdorf/fparsec) ⭐ 560 | 🐛 30 | 🌐 F# | 📅 2023-11-13 - The parser combinator library for F#.
* [XParsec](https://github.com/corsis/XParsec) ⭐ 55 | 🐛 0 | 🌐 F# | 📅 2018-03-14 - Extensible, type-and-source-polymorphic, non-linear applicative parser combinator library for F# 3.0 and 4.0.
* [FsAttoparsec](https://github.com/haf/FsAttoparsec) ⭐ 10 | 🐛 0 | 🌐 F# | 📅 2018-02-04 - Port of Bryan O'Sullivan's attoparsec from Haskell to F#.

## Serialization

<!--lint disable double-link -->

* [FSharp.SystemTextJson](https://github.com/Tarmil/FSharp.SystemTextJson) ⭐ 365 | 🐛 42 | 🌐 F# | 📅 2026-03-04 - System.Text.Json extensions for F# types.
* [FsPickler](https://github.com/mbraceproject/FsPickler) ⭐ 326 | 🐛 16 | 🌐 F# | 📅 2022-03-21 - Fast, multi-format messaging serializer for .NET.
* [FSharp.Json](https://github.com/vsapronov/FSharp.Json) ⭐ 228 | 🐛 32 | 🌐 F# | 📅 2025-08-30 - Reflection-based serialization library.
* [Fleece](https://github.com/mausch/Fleece) ⭐ 201 | 🐛 26 | 🌐 F# | 📅 2023-10-22 - JSON mapper for F#. It simplifies mapping from a Json library's JsonValue onto your types, and mapping from your types onto JsonValue.
* [FsCodec](https://github.com/jet/FsCodec) ⭐ 82 | 🐛 8 | 🌐 F# | 📅 2026-04-01 - F# Event-Union Contract Encoding with versioning tolerant converters.
* [Legivel](https://github.com/fjoppe/Legivel) ⭐ 63 | 🐛 6 | 🌐 F# | 📅 2023-08-01 - F# Yaml 1.2 parser.
* [Thoth.Json](https://thoth-org.github.io/Thoth.Json/) - JSON encoder/decoder library inspired by Elm.

<!--lint enable double-link -->

## Simulation

* [F# RISC-V Instruction Set formal specification](https://github.com/mrLSD/riscv-fs) ⭐ 288 | 🐛 0 | 🌐 F# | 📅 2024-09-11 - RISC-V CPU formal ISA Specification. RISC-V CPU simulator with ELF files execution.

## Static Site Generators

* [SkunkHTML](https://github.com/mg0x7BE/skunk-html) ⭐ 166 | 🐛 0 | 🌐 F# | 📅 2026-04-06 - Markdown blog with GitHub Pages.

## Testing

<!--lint disable double-link -->

* [NBomber](https://github.com/PragmaticFlow/NBomber) ⭐ 2,215 | 🐛 155 | 🌐 CSS | 📅 2026-03-23 - Simple load testing framework for Pull and Push scenarios.
* [FsCheck](https://github.com/fscheck/FsCheck) ⭐ 1,212 | 🐛 23 | 🌐 F# | 📅 2026-02-02 - Random testing for .NET.
* [Expecto](https://github.com/haf/expecto) ⭐ 730 | 🐛 63 | 🌐 F# | 📅 2026-03-19 - Smooth testing framework for F# with tests-as-values and parallelism by default.
* [altcover](https://github.com/SteveGilham/altcover) ⭐ 529 | 🐛 5 | 🌐 F# | 📅 2026-03-11 - Cross-platform coverage gathering and processing tool set for .NET/.NET core and Mono.
* [canopy](https://github.com/lefthandedgoat/canopy) ⭐ 510 | 🐛 28 | 🌐 F# | 📅 2022-08-08 - F# web automation and testing framework.
* [FsUnit](https://github.com/fsprojects/FsUnit) ⭐ 445 | 🐛 6 | 🌐 F# | 📅 2025-07-11 - Makes unit-testing with F# more enjoyable. It adds a special syntax to your favorite .NET testing framework.
* [unquote](https://github.com/swensensoftware/unquote) ⭐ 299 | 🐛 8 | 🌐 F# | 📅 2024-12-01 - Write F# unit test assertions as quoted expressions.
* [fsharp-hedgehog](https://github.com/hedgehogqa/fsharp-hedgehog) ⭐ 283 | 🐛 35 | 🌐 F# | 📅 2026-03-23 - Property-based testing system for F#.
* [Faqt](https://github.com/cmeeren/Faqt) ⭐ 77 | 🐛 3 | 🌐 F# | 📅 2025-12-19 - Fantastic fluent assertions for your F# tests and domain code.
* [Persimmon](https://github.com/persimmon-projects/Persimmon) ⭐ 41 | 🐛 6 | 🌐 F# | 📅 2022-03-05 - Unit test framework for F# using computation expressions.
* [xUnit.net](https://xunit.net/) - Free, open source, community-focused unit testing tool for the .NET Framework.

<!--lint enable double-link -->

## Type Providers

* [FSharp.Data](https://github.com/fsharp/FSharp.Data) ⭐ 869 | 🐛 3 | 🌐 F# | 📅 2026-04-13 - Data science library that contains type providers for CSV, HTML, JSON, XML, and WorldBank data.
* [Rezoom.SQL](https://github.com/rspeele/Rezoom.SQL) ⭐ 678 | 🐛 30 | 🌐 F# | 📅 2020-07-13 - Statically typed SQL for F#.
* [SQLProvider](https://github.com/fsprojects/SQLProvider) ⭐ 625 | 🐛 121 | 🌐 F# | 📅 2026-04-07 - General F# SQL database erasing type provider, supporting LINQ queries, schema exploration, individuals, CRUD operations and much more besides.
* [SwaggerProvider](https://github.com/fsprojects/SwaggerProvider) ⭐ 274 | 🐛 17 | 🌐 F# | 📅 2026-04-13 - Generative type provider for Swagger.
* [R Type Provider](https://github.com/BlueMountainCapital/FSharpRProvider) ⭐ 239 | 🐛 41 | 🌐 F# | 📅 2023-04-11 - Type provider to interop with R.
* [FSharp.Data.SqlClient](https://github.com/fsprojects/FSharp.Data.SqlClient) ⭐ 205 | 🐛 72 | 🌐 F# | 📅 2026-04-12 - F# type provider for statically typed access to T-SQL command parameters and result set.
* [FsXaml](https://github.com/fsprojects/FsXaml) ⭐ 170 | 🐛 12 | 🌐 F# | 📅 2019-12-06 - F# Tools for working with XAML Projects.
* [Facil](https://github.com/cmeeren/Facil) ⭐ 152 | 🐛 8 | 🌐 F# | 📅 2026-03-20 - Generates F# data access source code from SQL queries and stored procedures.
* [ExcelProvider](https://github.com/fsprojects/ExcelProvider) ⭐ 148 | 🐛 20 | 🌐 F# | 📅 2025-10-30 - Excel type provider.
* [FSharp.Data.Npgsql](https://github.com/demetrixbio/FSharp.Data.Npgsql) ⭐ 128 | 🐛 8 | 🌐 F# | 📅 2022-09-04 - F# type providers library on a top of well-known Npgsql ADO.NET client library.
* [FSharp.Configuration](https://github.com/fsprojects/FSharp.Configuration) ⭐ 116 | 🐛 48 | 🌐 F# | 📅 2025-05-03 - The project contains type providers for the configuration of .NET projects. Handles AppSettings, ResX, Yaml and Ini files.
* [FSharp.Management](https://github.com/fsprojects/FSharp.Management) ⭐ 93 | 🐛 16 | 🌐 F# | 📅 2019-06-17 - The project contains various type providers for the management of the machine. Handles file system, registry,  Windows Management Instrumentation, PowerShell and SystemTimeZones.
* [AzureStorageTypeProvider](https://github.com/fsprojects/AzureStorageTypeProvider) ⭐ 83 | 🐛 20 | 🌐 F# | 📅 2020-04-21 - F# Azure type provider which can be used to explore Blob, Table and Queue Azure Storage assets and easily apply CRUD operations on them.
* [FSharp.Text.RegexProvider](https://github.com/fsprojects/FSharp.Text.RegexProvider) ⭐ 78 | 🐛 1 | 🌐 F# | 📅 2019-10-11 - Type provider for regular expressions.
* [FSharp.Data.Toolbox](https://github.com/fsprojects/FSharp.Data.Toolbox) ⭐ 57 | 🐛 7 | 🌐 F# | 📅 2021-11-24 - Library for various data access APIs based on FSharp.Data. The library currently includes the Twitter type provider for access to Twitter users and feeds, and SAS type provider to read SAS dataset files.
* [FSharp.Data.TypeProviders](https://github.com/fsprojects/FSharp.Data.TypeProviders) ⭐ 38 | 🐛 1 | 🌐 F# | 📅 2021-11-20 - Library that contains type providers for `.edmx` files, `.dbml` files, WSDL services, OData services, and SQL databases.
* [FsYaml](https://github.com/bleis-tift/FsYaml) ⭐ 37 | 🐛 6 | 🌐 F# | 📅 2022-06-20 - Typed Yaml library for F#.
* [GraphProvider](https://github.com/fsprojects/GraphProvider) ⭐ 36 | 🐛 2 | 🌐 F# | 📅 2016-04-04 - `.dgml` state machine type provider.
* [EasyBuild.FileSystemProvider](https://github.com/easybuild-org/EasyBuild.FileSystemProvider) ⭐ 35 | 🐛 5 | 🌐 F# | 📅 2026-01-14 - Type provider to provide a typed representation of files and directories based on your project structure or a virtual file system.
* [S3Provider](https://github.com/fsprojects/S3Provider) ⭐ 22 | 🐛 5 | 🌐 F# | 📅 2016-04-04 - Experimental type provider for Amazon S3.
* [DynamicsCRMProvider](https://github.com/fsprojects/DynamicsCRMProvider) ⭐ 15 | 🐛 7 | 🌐 F# | 📅 2020-07-19 - Type provider for Microsoft Dynamics CRM 2011.
* [FSharp.Data.Tdms](https://github.com/mettekou/FSharp.Data.Tdms) ⚠️ Archived - TDMS support for F#.
* [MatDataProvider](https://github.com/fsprojects/matprovider) ⭐ 10 | 🐛 0 | 🌐 F# | 📅 2018-02-28 - Erased type provider for `.mat` files (binary MATLAB format files).

### Creating Type Providers

* [FSharp.TypeProviders.StarterPack](https://github.com/fsprojects/FSharp.TypeProviders.StarterPack) ⭐ 302 | 🐛 8 | 🌐 F# | 📅 2026-04-13 - The ProvidedTypes SDK for creating F# type providers.

## Visualization

* [Plotly.NET](https://github.com/plotly/Plotly.NET) ⭐ 846 | 🐛 46 | 🌐 F# | 📅 2026-04-02 - A Plotly-based general purpose plotting library for F#.
* [XPlot](https://github.com/fslaborg/XPlot) ⭐ 288 | 🐛 27 | 🌐 F# | 📅 2024-12-26 - A plotting library for the F# programming language.
* [FSharp.Charting](https://github.com/fslaborg/FSharp.Charting) ⭐ 209 | 🐛 36 | 🌐 F# | 📅 2020-07-06 - Charting library suitable for interactive F# scripting.
* [GG.Net](https://github.com/pablofrommars/GGNet) ⭐ 87 | 🐛 2 | 🌐 C# | 📅 2026-03-16 - Visualization library for data scientists.
* [SharpVG](https://github.com/ChrisNikkel/SharpVG) ⭐ 79 | 🐛 13 | 🌐 F# | 📅 2026-04-12 - Create SVG vector graphics in F#.

## Web Frameworks

<!--lint disable double-link -->

* [Giraffe](https://github.com/giraffe-fsharp/Giraffe) ⭐ 2,237 | 🐛 46 | 🌐 F# | 📅 2026-04-11 - Native functional ASP.NET Core web framework for F# developers.
* [Suave](https://github.com/SuaveIO/suave) ⭐ 1,345 | 🐛 12 | 🌐 F# | 📅 2026-01-16 - A simple web development F# library providing a lightweight web server and a set of combinators to manipulate route flow and task composition.
* [Bolero](https://github.com/fsbolero/Bolero/) ⭐ 1,127 | 🐛 73 | 🌐 F# | 📅 2025-10-26 - F# in WebAssembly, develop SPAs with the full power of F# and .NET Blazor.
* [Saturn](https://github.com/SaturnFramework/Saturn) ⭐ 724 | 🐛 55 | 🌐 F# | 📅 2024-07-31 - Opinionated, web development framework for F# which implements the server-side, functional MVC pattern.
* [Falco](https://github.com/pimbrouwers/Falco/) ⭐ 630 | 🐛 6 | 🌐 F# | 📅 2026-03-19 - A functional-first toolkit for building brilliant ASP.NET Core applications using F#.
* [WebSharper](https://github.com/intellifactory/websharper) ⭐ 629 | 🐛 271 | 🌐 F# | 📅 2026-04-10 - F#-based web programming platform including a compiler from F# code to JavaScript.
* [Feliz](https://github.com/Zaid-Ajaj/Feliz) ⭐ 602 | 🐛 1 | 🌐 F# | 📅 2026-03-21 - A fresh retake of the React API in Fable and a collection of high-quality components to build React applications in F#.
* [Oxpecker](https://github.com/Lanayx/Oxpecker) ⭐ 405 | 🐛 10 | 🌐 F# | 📅 2026-04-08 - ASP.NET Core based F# framework + supporting tools (ViewEngine, Htmx, OpenApi).
* [Felicity](https://github.com/cmeeren/Felicity) ⭐ 95 | 🐛 1 | 🌐 F# | 📅 2025-12-19 - Boilerplate-free, idiomatic JSON:API for your beautiful, idiomatic F# domain model.
* [Genit](https://github.com/lefthandedgoat/genit) ⭐ 67 | 🐛 16 | 🌐 CSS | 📅 2018-03-01 - Cross-platform website generator and server using F#, Suave and PostgreSQL or MS SQL Server.

<!--lint enable double-link -->

## .NET Core Templates

<!--lint disable awesome-list-item-->

* [Fable-elmish](https://github.com/fable-compiler/fable-elmish) ⭐ 892 | 🐛 8 | 🌐 F# | 📅 2026-03-30 - `dotnet new -i Fable.Template.Elmish.React::*`
* [SAFE Stack Template](https://github.com/SAFE-Stack/SAFE-template) ⭐ 288 | 🐛 15 | 🌐 F# | 📅 2025-11-15 - `dotnet new -i SAFE.Template::*`
* [MiniScaffold](https://github.com/TheAngryByrd/MiniScaffold) ⭐ 273 | 🐛 5 | 🌐 F# | 📅 2026-03-10 - F# Template for creating and publishing libraries targeting .NET Full (net45) and Core (netstandard1.6), `dotnet new -i MiniScaffold::*`
* [Giraffe Template](https://github.com/giraffe-fsharp/giraffe-template) ⭐ 39 | 🐛 5 | 🌐 F# | 📅 2024-08-19 - `dotnet new -i "giraffe-template::*"`
* [Expecto Template](https://github.com/MNie/Expecto.Template) ⭐ 25 | 🐛 1 | 🌐 F# | 📅 2025-03-12 - `dotnet new -i Expecto.Template::*`
* [ASP.NET Core WebAPI F# Template](https://github.com/MNie/FSharpNetCoreWebApiTemplate) ⭐ 17 | 🐛 1 | 🌐 F# | 📅 2019-07-08 - `dotnet new -i WebAPI.FSharp.Template::*`
* [NancyFx Template](https://github.com/MNie/NancyFxCore) ⭐ 3 | 🐛 0 | 🌐 F# | 📅 2019-11-29 - `dotnet new -i NancyFx.Core.Template::*`
* [Fable, F# |> Babel](http://fable.io) - `dotnet new -i Fable.Template::*`

<!--lint enable awesome-list-item-->

## Resources

### Blogs

* [.NET Blog (F# tag)](https://devblogs.microsoft.com/dotnet/tag/f/) - News and discussions about F# from the .NET team.
* [Codesuji](https://codesuji.com) - A community member blog, focusing on functional aspects on F#.
* [Krzysztof Cieslak](https://kcieslak.io/) - A blog of the Ionide maintainer.
* [Mark Seemann](https://blog.ploeh.dk/) - A blog discussing various aspects of software design.
* [Sergey Tihon (F# Weekly)](https://sergeytihon.com/) - Weekly newsletter collected across the ecosystem.
* [Tomas Petricek](http://tomasp.net/blog/) - A well-known community member working on a diverse set of topics.

### Books

* [Domain Modeling Made Functional by Scott Wlaschin](https://pragprog.com/titles/swdddf/domain-modeling-made-functional/) - Tackle software complexity with domain-driven design and F#.
* [F# in Action by Isaac Abraham](https://www.manning.com/books/f-sharp-in-action) - A practical guide in software development in F#.

### Cheatsheets

* [Guide for Rust devs to learn F#](https://github.com/Dhghomon/rust-fsharp) ⭐ 265 | 🐛 14 | 📅 2023-01-14 - Informal manual for users of Rust and F# to read through to learn about the other language.
* [Guide for C# devs to learn F#](https://github.com/knocte/2fsharp/blob/master/csharp2fsharp.md) ⭐ 167 | 🐛 4 | 📅 2026-02-11 - A 30-minute F# tutorial for C# programmers, with back-to-back code snippets.
* [Guide for Python devs to learn F#](https://github.com/knocte/2fsharp/blob/master/python2fsharp.md) ⭐ 167 | 🐛 4 | 📅 2026-02-11 - A 30-minute F# tutorial for Python programmers, with back-to-back code snippets.
* [F# Snips](https://fssnip.net/) - Share your snippets of F# code.
* [F# cheatsheet](https://fsprojects.github.io/fsharp-cheatsheet/) - Quick reference for the main language features.
* [F# tour](https://docs.microsoft.com/en-us/dotnet/articles/fsharp/tour) - Official language tour from Microsoft.
* [Learn F# in Y minutes](https://learnxinyminutes.com/docs/fsharp) - A guide recommended to quickly start programming in F#.

### Community

* [Amplifying F#](https://amplifyingfsharp.io)
* [F# on BlueSky](https://bsky.app/hashtag/fsharp)
* [F# on Discord](https://discord.com/invite/fsharp-196693847965696000)
* [F# on Discourse](https://forums.fsharp.org/)
* [F# on Reddit](https://www.reddit.com/r/fsharp/)
* [F# on Telegram](https://t.me/fsharp_chat)
* [F# on Twitter](https://x.com/hashtag/fsharp)

### Other Lists

* [Awesome .NET!](https://github.com/quozd/awesome-dotnet) ⭐ 21,245 | 🐛 60 | 📅 2026-03-26 - Collection of awesome .NET libraries, tools, frameworks and software.
* [Companies using F#](https://github.com/fsprojects/fsharp-companies) ⭐ 408 | 🐛 25 | 📅 2026-01-26 - Community curated list of companies that use F# (maybe useful if you're looking for a job?)
* [F# Community Projects](http://fsharp.org/community/projects/) - Everything produced by the F# community.
* [Fable Resources](https://fable.io/resources.html) - A curated list of useful Fable-related tutorials, libraries and software.

### Websites

* [Community for F#](http://c4fsharp.net/) - Links to dojos and recordings of community presentations.
* [Decompiler.com](https://www.decompiler.com/) - Online C#/VB/F# decompiler.
* [DotNetFiddle](https://dotnetfiddle.net/) - Online REPL.
* [F# Software Foundation](http://fsharp.org/) - Main website.
* [F# for Fun and Profit](https://fsharpforfunandprofit.com/) - Reference tutorials.
* [SharpLab](https://sharplab.io/) - C#/VB/F# compiler playground.
* [Try F#](https://try.fsharp.org/) - Online tutorials, currently without execution of code due to Silverlight dependency.
* [cs2fs](https://jindraivanek.gitlab.io/cs2fs-online) - Transform C# code to F# code.
* [fantomas-tools](https://fsprojects.github.io/fantomas-tools) - A set of Fantomas related tools like AST viewer and online bug reporter.

### Videos

* [Amplifying F# YouTube Channel](https://www.youtube.com/@amplifyingfsharp)
* [F# Online YouTube Channel](https://www.youtube.com/@fonline6018)
* [Austin F# Meetup Group Recorded Presentations](http://usergroup.tv/videos/category/group/austin-f-meetup)
* [F# Chats on performance](https://www.youtube.com/watch?v=EIBRoNEpg6c\&list=PLqWncHdBPoD4O1sr2Q3W9gAuJ30s09U2r)
* [Fast Dictionary in F#](https://www.youtube.com/watch?v=KMR2y1vcO-s\&list=PLqWncHdBPoD4-d_VSZ0MB0IBKQY0rwYLd)
* [Intro to F#](https://www.youtube.com/watch?v=1ioGr701c5Q\&list=PLqWncHdBPoD4YEWoXQlRj1tiTc96HZxH8)
* [Topological Sort](https://www.youtube.com/playlist?list=PLqWncHdBPoD5hEK31CcfmTHP-7icw2Xd0)

### Courses

* [Write yourself a scheme in 48 hours using F#](https://write-yourself-a-scheme.pangwa.com/)
