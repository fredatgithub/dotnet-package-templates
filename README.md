<h1 align="center">
  <br>
  .NET Library Package Templates
  <br>
</h1>

<h4 align="center">"dotnet new" templates for building NuGet-published multi-targeting libraries with all the bells and whistles</h4>

<div align="center">

[![](https://img.shields.io/github/actions/workflow/status/dennisdoomen/dotnet-package-templates/build.yml?branch=main)](https://github.com/dennisdoomen/dotnet-package-templates/actions?query=branch%3amain)
[![Coveralls branch](https://img.shields.io/coverallsCoverage/github/dennisdoomen/dotnet-package-templates?branch=main)](https://coveralls.io/github/dennisdoomen/dotnet-package-templates?branch=main)
[![](https://img.shields.io/github/release/dennisdoomen/dotnet-package-templates.svg?label=latest%20release&color=007edf)](https://github.com/dennisdoomen/dotnet-package-templates/releases/latest)
[![](https://img.shields.io/nuget/dt/dotnet-package-templates.svg?label=downloads&color=007edf&logo=nuget)](https://www.nuget.org/packages/dotnet-package-templates)
[![](https://img.shields.io/librariesio/dependents/nuget/Reflectify.svg?label=dependent%20libraries)](https://libraries.io/nuget/Reflectify)
![GitHub Repo stars](https://img.shields.io/github/stars/dennisdoomen/dotnet-package-templates?style=flat)
[![GitHub contributors](https://img.shields.io/github/contributors/dennisdoomen/dotnet-package-templates)](https://github.com/dennisdoomen/dotnet-package-templates/graphs/contributors)
[![GitHub last commit](https://img.shields.io/github/last-commit/dennisdoomen/dotnet-package-templates)](https://github.com/dennisdoomen/dotnet-package-templates)
[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/dennisdoomen/dotnet-package-templates)](https://github.com/dennisdoomen/dotnet-package-templates/graphs/commit-activity)
[![open issues](https://img.shields.io/github/issues/dennisdoomen/dotnet-package-templates)](https://github.com/dennisdoomen/dotnet-package-templates/issues)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
![](https://img.shields.io/badge/release%20strategy-githubflow-orange.svg)
![Static Badge](https://img.shields.io/badge/4.7%2C_6.0%2C_8.0%2C_netstandard2.0%2C_netstandard2.1-dummy?label=dotnet&color=%235027d5)

<a href="#about">About</a> •
<a href="#how-to-use-it">How To Use</a> •
<a href="#download">Download</a> •
<a href="#contributors">Contributors</a> •
<a href="#versioning">Versioning</a> •
<a href="#credits">Credits</a> •
<a href="#related">Related</a> •
<a href="#license">License</a>

</div>

## About

### What's this?

A bunch of `dotnet new` templates to quickly get you started building high-quality libraries including everything you need to publish it on NuGet or make it available as open-source.

It includes:
* Multi-targeting to cover as many .NET frameworks as possible
* Code coverage using [Coverlet](https://github.com/coverlet-coverage/coverlet) and [Coveralls.io](https://coveralls.io/)
* Static code analysis using Roslyn analyzers [StyleCop], [Roslynator], [CSharpGuidelinesAnalyzer] and [Meziantou].
* Auto-formatting using `.editorconfig` and settings honored by [JetBrains Rider] and [ReSharper]
* A [Nuke] C# build script that you can run locally as well as using GitHub Actions (or others)
* A GitHub Actions workflow that builds, tests, packages and publishes your library
* An extensive read-me
* Automatic versioning using [GitVersion] and tagging
* Contribution guidelines
* Bug report templates
* Customized release notes templates for GitHub
* A test project using [xUnit] and [Fluent Assertions 7]
* Support for content-only NuGet packages
* Validation of the public API of the library against snapshots using [Verify]

### What's so special about that?

I like to build my software systems in a nicely broken down set of libraries that are easy to maintain, test and deploy based on the [Principles Of Successful Package Management](https://www.dennisdoomen.com/2016/10/principles-for-successful-package.html). But every time I or the teams I work with need to start a new library or reusable component, we have to scramble so much from other projects, I felt this good fill the gap.

This is the result of years of experience in building in-house and open-source libraries that are used by thousands of developers around the world. I hope it's a great starting point for building your own libraries.

### Who created this?
My name is Dennis Doomen and I'm a Microsoft MVP and Principal Consultant at [Aviva Solutions](https://avivasolutions.nl/) with 28 years of experience under my belt. As a software architect and/or lead developer, I specialize in designing full-stack enterprise solutions based on .NET as well as providing coaching on all aspects of designing, building, deploying and maintaining software systems. I'm the author of several open-source projects such as [Fluent Assertions](https://www.fluentassertions.com), [Reflectify](https://github.com/dennisdoomen/reflectify), [Liquid Projections](https://www.liquidprojections.net), and I've been maintaining [coding guidelines for C#](https://www.csharpcodingguidelines.com) since 2001.

Contact me through [Email](mailto:dennis.doomen@avivasolutions.nl), [Bluesky](https://bsky.app/profile/ddoomen.bsky.social), [Twitter/X](https://twitter.com/ddoomen) or [Mastadon](https://mastodon.social/@ddoomen)

## Download

This library is available as [a NuGet package](https://www.nuget.org/packages/dotet) on https://nuget.org. To install it, use the following command-line:

`dotnet new -i DotNetPackageTemplates`

`dotnet new Binary.Package.Template --name YourLibraryName`

## How do I use it?

todo: what to customize after creating the project
todo: silent formatting in Rider and ReSharper

## Contributors

Your contributions are always welcome! Please have a look at the [contribution guidelines](CONTRIBUTING.md) first.

<a href="https://github.com/dennisdoomen/dotnet-package-templates/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=dennisdoomen/dotnet-package-templates" alt="contrib.rocks image" />
</a>

(Made with [contrib.rocks](https://contrib.rocks))

## Versioning
This library uses [Semantic Versioning](https://semver.org/) to give meaning to the version numbers. For the versions available, see the [tags](/releases) on this repository.

## Credits
This library wouldn't have been possible without the following tools, packages and companies:

* [ASP.NET Core Template](https://github.com/NikolayIT/ASP.NET-Core-Template) - Created by [Nikolay Kostov](https://github.com/NikolayIT) and the inspiration for this repo.
* [Nuke](https://nuke.build/) - Smart automation for DevOps teams and CI/CD pipelines by [Matthias Koch](https://github.com/matkoch)
* [Rider](https://www.jetbrains.com/rider/) - The world's most loved .NET and game dev IDE by [JetBrains](https://www.jetbrains.com/)
* [xUnit](https://xunit.net/) - Community-focused unit testing tool for .NET by [Brad Wilson](https://github.com/bradwilson)
* [Coverlet](https://github.com/coverlet-coverage/coverlet) - Cross platform code coverage for .NET by [Toni Solarin-Sodara](https://github.com/tonerdo)
* [Polysharp](https://github.com/Sergio0694/PolySharp) - Generated, source-only polyfills for C# language features by [Sergio Pedri](https://github.com/Sergio0694)
* [GitVersion](https://gitversion.net/) - From git log to SemVer in no time
* [ReportGenerator](https://reportgenerator.io/) - Powerful code coverage visualization
* Roslynator
* CSharpCodingGuidelines
* Roslynator
* Meziantou

## Support the project
* [Github Sponsors](https://github.com/sponsors/dennisdoomen)
* [Tip Me](https://paypal.me/fluentassertions)
* [Buy me a Coffee](https://ko-fi.com/dennisdoomen)
* [Sponsor Me](https://www.patreon.com/bePatron?u=9250052&redirect_uri=http%3A%2F%2Ffluentassertions.com%2F&utm_medium=widget)

## You may also like

* [My Blog](https://www.dennisdoomen.com)
* [FluentAssertions](https://github.com/fluentassertions/fluentassertions) - Extension methods to fluently assert the outcome of .NET tests
* [C# Coding Guidelines](https://csharpcodingguidelines.com/) - Forkable coding guidelines for all C# versions

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
