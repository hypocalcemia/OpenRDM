# OpenRDM

**Open Release & Delivery Manifest** — Making software delivery transparent, debuggable, and developer-friendly.

![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)

## Overview

OpenRDM is a framework for reverse-engineering, documenting, and transparently managing complex software delivery pipelines. It emerged from analyzing real-world installer chains (like Visual Studio bootstrappers) where users have no visibility into what gets downloaded, when, or why.

The goal is simple: **developers should understand exactly what gets downloaded, when, and why** — not rely on blackbox installers that phone home to mysterious URLs.

## The Problem

Modern software installation is often opaque:

- **Unknown dependencies**: You run an installer and have no idea what components are being pulled in
- **Supply chain blindness**: No clear record of sources, versions, or checksums
- **Reproducibility issues**: Different machines install different versions due to silent updates
- **Security concerns**: Hard to audit what's being downloaded and verify its authenticity
- **Debugging nightmare**: When something breaks, you can't trace back through the delivery chain

## What OpenRDM Solves

OpenRDM provides tools and patterns to:

- **Reverse-engineer** installation and delivery chains (e.g., bootstrapper → component manifest → full packages)
- **Document** the supply chain transparently (manifest files, channels, URIs, hashes)
- **Trace** dependencies and component relationships in complex builds
- **Audit** what gets delivered and ensure reproducibility
- **Share** clear documentation so other developers can understand and verify your pipeline
