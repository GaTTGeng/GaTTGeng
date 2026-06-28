# GaTT Geng

.NET and infrastructure tooling developer based in Wuhan, China.

I mostly work on managed SDKs that make platform protocols usable from ordinary .NET applications: chart rendering and Kubernetes release workflows on one side, network file-system clients and RPC protocol models on the other.

## Focus

- C# / .NET libraries with clean NuGet distribution.
- Kubernetes, Helm-style workflows, and deployment automation.
- NFS, RPC/XDR protocol modeling, and storage-facing client APIs.
- Compatibility testing against real tools and services instead of only hand-written fixtures.

## Projects

### [HelmSharp](https://github.com/GaTTGeng/HelmSharp)

[![HelmSharp CI](https://github.com/GaTTGeng/HelmSharp/actions/workflows/ci.yml/badge.svg)](https://github.com/GaTTGeng/HelmSharp/actions/workflows/ci.yml)
[![NuGet](https://img.shields.io/nuget/v/HelmSharp.Action.svg)](https://www.nuget.org/packages/HelmSharp.Action)

A managed Helm-style SDK for .NET. HelmSharp is aimed at applications that need to load charts, merge values, render templates, package charts, inspect repositories, and drive release operations against Kubernetes without treating the Helm CLI as a runtime dependency.

The current work is centered on Helm template parity: golden tests compare HelmSharp output with `helm template` across small fixtures and real public charts such as ingress-nginx, cert-manager, metrics-server, external-dns, and podinfo.

### [NfsSharp](https://github.com/GaTTGeng/NfsSharp)

[![NfsSharp CI](https://github.com/GaTTGeng/NfsSharp/actions/workflows/ci.yml/badge.svg)](https://github.com/GaTTGeng/NfsSharp/actions/workflows/ci.yml)
[![NuGet](https://img.shields.io/nuget/v/NfsSharp.Client.svg)](https://www.nuget.org/packages/NfsSharp.Client)

A managed NFS client and protocol SDK for .NET. The high-level client focuses on NFSv3 over TCP: export discovery, mounting, directory traversal, file reads and writes, links, attributes, and file-system capability queries.

The lower-level protocol package contains XDR primitives, NFS models, status codes, RPC-related abstractions, and experimental direct NFSv4 COMPOUND APIs for protocol work that needs more control than the facade exposes.

## GitHub Stats

![GaTTGeng GitHub stats](https://github-readme-stats.vercel.app/api?username=GaTTGeng&show_icons=true&hide_border=true&theme=transparent)

![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=GaTTGeng&layout=compact&hide_border=true&theme=transparent)

## Links

- [NuGet profile](https://www.nuget.org/profiles/GaTT)
- [HelmSharp documentation](https://gattgeng.github.io/HelmSharp/)
