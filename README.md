***

> [!WARNING]  
> This is the development release of the Tingen Web Service, and is not intended for use in production environments.

***

<div align="center">

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/repository/logo/Tingen-WebService-CommunityRelease-Logo-Trans-ForDark-512x346.png">
    <source media="(prefers-color-scheme: light)" srcset=".github/repository/logo/Tingen-WebService-CommunityRelease-Logo-Trans-ForLight-512x346.png">
    <img alt="Fallback image description" src=".github/repository/logo/Tingen-WebService-CommunityRelease-Logo-Trans-ForLight-512x346.png">
  </picture>
  
  <h3>The Community Release of the Tingen Web Service</h3>

  ![RELEASE](https://img.shields.io/badge/release-26.6-teal)&nbsp;
  ![LICENSE](https://img.shields.io/badge/license-apache-blue)&nbsp;
  ![Platform](https://img.shields.io/badge/platform-Windows-lightgrey)&nbspp

</div>

***

<h6 align="center">

  [MANUAL](docs/man/README.md)&nbsp;&bull;&nbsp;[CHANGELOG](docs/CHANGELOG.md)&nbsp;&bull;&nbsp;[ROADMAP](docs/ROADMAP.md)&nbsp;&bull;&nbsp;[KNOWN ISSUES](docs/KNOWN-ISSUES.md)
  
</h6>

***

| CONTENTS                                                      |
|:------------------------------------------------------------- |
| [ABOUT THE TINGEN WEB SERVICE](#about-the-tingen-web-service) |
| [FEATURES](#features)                                         |
| [HOW IT WORKS](#how-it-works)                                 |
| [GETTING STARTED](#getting-started)                           |
| [BUILT WITH](#built-with)                                     |
| [RELATED PROJECTS](#related-projects)                         |
| [LICENSE](#license)                                           |

***

## ABOUT THE TINGEN WEB SERVICE

Netsmart's [AvatarNX™ EHR](https://www.ntst.com/Solutions-and-Services/Offerings/myAvatar) is a behavioral health Electronic Health Records application that offers a recovery-focused suite of solutions that leverage real-time analytics and clinical decision support to drive value-based care.

While AvatarNX™ is a robust platform, it isn't perfect. The good news is that you can extend AvatarNX™ functionality via [Netsmart's Web Services](URL), and/or custom web services that are written by other AvatarNX™ users.

The **Tingen Web Service** is one such custom web service which includes various tools and utilities for AvatarNX™ that aren't included in the official release, and provides a solid foundation for building additional functionality quickly and efficiently.

## FEATURES

* Several built-in tools and utilities that extend the functionality of AvatarNX™
* A solid foundation to build additional AvatarNX™ custom tools and utilities
* Extremely customizable
* Robust logging
* ...and more!

## HOW IT WORKS

A very high level overview of how the Tingen Web Service works:

1. Avatar sends an `OptionObject` and a `ScriptParameter` to the Tingen Web Service
2. The Tingen Web Service processes the request and returns a modified `OptionObject` back to Avatar

```mermaid
flowchart TB
  %% Components
  Start@{shape: circle, label: "Avatar"}
  TingenWebService@{shape: rounded, label: "Tingen Web Service"}
  %% Layout
  Start:::G1_ -- 1. Request --> TingenWebService:::E4_ -- 2. Response --> Start
  %% Styles
  classDef G1_ stroke:#e9f7ef,stroke-width:3px,fill:#a9dfbf,color:#145a32
  classDef E4_ stroke:#fdf2e9,stroke-width:3px,fill:#784212,color:#fdf2e9
```

## GETTING STARTED

### Requirements

You can find all of the information you need to install and use the Tingen Web Service in the [Tingen Web Service Manual](docs/man/README.md).

If you are interested in contributing to the development of the Tingen Web Service, or are just curious about how it works under the hood, please check out the [Development Manual](docs/man/dev/README.md) and/or the [API documentation](https://spectrum-health-systems.github.io/Tingen-WebService/api/html/Welcome.htm).

## BUILT WITH

* [.NET Framework 4.8](https://dotnet.microsoft.com/en-us/download/dotnet-framework/net48)
* [ScriptLink Standard](https://rcskids.github.io/ScriptLinkStandard/) - A class library for creating SOAP web services [AvatarNX™](https://www.ntst.com/Solutions-and-Services/Offerings/myAvatar)
* [Sandcastle Help File Builder](https://github.com/EWSoftware/SHFB)  - Documentation generation

## RELATED PROJECTS

* [Tingen Transmorger](https://github.com/spectrum-health-systems/Tingen-Transmorger) - Utilities for Netsmart's AvatarNX™ TeleHealth platform
* [The Unofficial AvatarNX Runbook](https://github.com/spectrum-health-systems/The-Unofficial-AvartarNX-Runbook) - A collection of tips, tricks, and best practices for working with AvatarNX™

## LICENSE

Distributed under the [Apache 2.0 License](LICENSE)  
Copyright &copy; 2026 [A Pretty Cool Program](https://github.com/APrettyCoolProgram)

***

<h6 align="center">

  [FAQ](docs/FAQ.md)&nbsp;&bull;&nbsp;[DEVELOPMENT](docs/DEVELOPMENT.md)&nbsp;&bull;&nbsp;[API](https://spectrum-health-systems.github.io/Tingen-WebService/api/html/Welcome.htm)&nbsp;&bull;&nbsp;[TESTING](docs/TESTING.md)&nbsp;&bull;&nbsp;[SUPPORT](docs/SUPPORT.md)&nbsp;&bull;&nbsp;[NOTICES](docs/NOTICES.md)
  
</h6>








<div align="center">

  ![logo](./.github/images/logos/TingenCommunityRelease_README.png)
  
  ![PRODUCTION_VERSION](https://img.shields.io/badge/release-00.00-seagreen?style=flat-square)&nbsp;&nbsp;
  ![DotNet](https://img.shields.io/badge/.net-Framework_4.8-darkslateblue?style=flat-square)&nbsp;&nbsp;
  ![Platform](https://img.shields.io/badge/platform-Windows-blue?style=flat-square)&nbsp;&nbsp;
  ![License](https://img.shields.io/github/license/spectrum-health-systems/Outpost31?style=flat-square)&nbsp;&nbsp;

</div>

# About the Tingen Community Release

[Tingen](https://github.com/spectrum-health-systems/Tingen) is a custom web service for Netsmart's Avatar EHR.

The Tingen Community Release is:

* The **stable, tested** version of Tingen!
* **Intended** to be used in production environments!
* Has beautiful code*! Like **poetry**!
* For use by the Avatar Community!

# Repository branches

There are three types of branches in this repository:

* **[main](https://github.com/spectrum-health-systems/Tingen_development/tree/main)**  
  This is the current Tingen Community Release.
  
  Feel free to use it in your production environments.
  
* **Community Release archive snapshots**  
  When development starts on a new monthly version, the previous version is archived to a separate branch (e.g., `24.9.0-CommunityRelease`).

# Documentation

You can find all the documentation you could ever want about Tingen (and related projects) [here](https://github.com/spectrum-health-systems/Tingen-Documentation).

<sup>* Not really, but I think it's nice.</sup>
