# Pythology Aegis Pages

Public GitHub Pages carrier for **Pythology Aegis**.

Production source remains private in `PythologyIntelligence/pythologyaegis`. This repository contains only the deployment workflow required to build the public-safe static site and publish it with GitHub Pages.

## Public hostname

`https://aegis.pythology.co.nz`

## Deployment boundary

- Public marketing site + synthetic interactive demo: GitHub Pages
- Aegis API/control plane: Pythology VPS
- Authenticated operational Command Centre: Pythology VPS
- Sovereign customer edge: customer environment

## Required repository secret

`AEGIS_SOURCE_TOKEN`

Use a fine-grained GitHub token with **read-only Contents access** to the private `PythologyIntelligence/pythologyaegis` repository. No write access to the private source repository is required.

The public Pages build never receives VPS, Resend, database, model or customer secrets.
