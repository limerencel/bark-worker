<p align="center">
    <h1 align="center">Bark-Worker</h1>
</p>

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

**[中文文档](README.zh.md)**

Bark-Worker is a [Bark-Server](https://github.com/Finb/bark-server) implenmention on Cloudflare Worker. It provides privacy-aware users with a cheap and private bark backend. 

### What is [Bark](https://github.com/Finb/Bark)?
[Bark](https://github.com/Finb/Bark) is an iOS App which allows you to push customed notifications to your iPhone.

> [!NOTE]
> A domain is required if worker.dev is unavailable in your country/region

## Features
- Full Bark-Server APIs support
    - `register`
    - `ping`
    - `healthz`
    - `info`
    - `push`
- Path based parameters resolve
- Easy to deploy, Cheap to use and Convenient to manage

## Setup

> [!NOTE]
> Select one, D1 or KV Version are both available. D1 Version is recommended for its higher usage than KV Version. However, Cloudflare D1 is still in `beta`, which is unstable, use at your own risk.

<!-- > [!CAUTION]
> After Cloudflare D1 is not in Beta, KV Version maybe deprecated. -->

Refer to [Setup Guide](doc/setup_guide.md)

### Cloudflare D1 Version

Create a Worker and a D1 Database, bind D1 database to Worker with name `database`

### Cloudflare KV Version

Create a Worker and a KV Storage, bind KV Storage to Worker with name `database`

## Tips

- Multi Device Key to one Device
- Device Key Alias
- D1 Database Manage in Console
- etc.

Refer to [Tips](doc/tips.md)
