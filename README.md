# OpenRDM

**Open Release & Delivery Manifest** — Making software delivery transparent, debuggable, and developer-friendly.

## Overview

OpenRDM is a framework for reverse-engineering, documenting, and transparently managing complex software delivery pipelines. It emerged from analyzing real-world installer chains (like Visual Studio) to understand how software components are bootstrapped, manifested, and deployed.

The goal: developers should understand *exactly* what gets downloaded, when, and why—not blackbox installers that phone home to mysterious URLs.

## What It Does

OpenRDM provides tools and patterns to:

- **Reverse-engineer** installation and delivery chains (e.g., bootstrapper → component manifest → full packages)
- **Document** the supply chain transparently (manifest files, channels, URIs, hashes)
- **Trace** dependencies and component relationships in complex builds
- **Audit** what gets delivered and ensure reproducibility
- **Share** clear documentation so other developers can understand your pipeline

## Why It Matters

Modern software installation often looks like this:
https://media3.giphy.com/media/v1.Y2lkPTZjMDliOTUybmk2cnRsOW5sMThzMzVlN3duanIxdjYyZXJtdThiMHBpankyZHl2NiZlcD12MV9naWZzX3NlYXJjaCZjdD1n/9o9dh1JRGThC1qxGTJ/giphy.gif
