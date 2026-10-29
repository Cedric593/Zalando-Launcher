Zalando Launcher

Version 0.3.0 | Minecraft Java Edition Launcher

Zalando Launcher is an independent, open-source-oriented desktop launcher project for Minecraft: Java Edition, developed using Electron, Node.js, JavaScript, HTML, and CSS.

The launcher aims to provide a modern interface for managing Minecraft installations, Java runtimes, player accounts, and game configurations.

Development Status: Zalando Launcher is currently under active development. Some features are experimental or not yet fully implemented.

Features

Minecraft Version Management

Retrieve available Minecraft Java Edition versions.

Download and install supported Minecraft versions.

Detect locally installed Minecraft versions.

Prepare game libraries and native dependencies.

Java Runtime Management

Automatically detect installed Java runtimes.

Identify Java requirements for Minecraft versions.

Download supported Java runtimes when required.

Microsoft Authentication

Microsoft OAuth 2.0 authentication with PKCE.

Xbox Live and XSTS authentication.

Integration with Minecraft Services.

Minecraft player profile retrieval.

Current limitation: Microsoft and Xbox authentication are implemented, but Minecraft Services authentication currently requires approval of the application's Microsoft Client ID.

Game Launching

Prepare Minecraft launch configurations.

Configure Java memory allocation.

Resolve required libraries and native dependencies.

The authenticated game launch process is still under development.

User Interface

Desktop interface built with Electron.

Minecraft version selection.

Account management interface.

Java configuration and runtime detection.

Planned mod and cosmetics management features.

Technology Stack

Component

Technology

Desktop Framework

Electron

Backend

Node.js

Frontend

HTML, CSS, JavaScript

Authentication

Microsoft OAuth 2.0 with PKCE

Xbox Authentication

Xbox Live and XSTS

Minecraft Integration

Minecraft Services API

Game Runtime

Java

Authentication and Game Ownership

Zalando Launcher is designed to authenticate users through their own Microsoft accounts.

The authentication process uses Microsoft's OAuth 2.0 authorization code flow with PKCE.

The intended authentication flow is:

The user initiates Microsoft authentication.

Authentication takes place in the user's default browser.

The launcher receives an authorization code through a local callback.

Microsoft authentication is exchanged for Xbox Live and XSTS authentication.

Minecraft Services authentication is performed.

The user's Minecraft Java Edition profile is retrieved.

An authenticated game session can be prepared.

Zalando Launcher is intended for users who legitimately own Minecraft: Java Edition.

The project does not aim to bypass Microsoft authentication, Minecraft account ownership verification, or official licensing requirements.

Authentication tokens are handled by the backend and are not intentionally exposed to the frontend.

Persistent secure token storage is not yet implemented.

Application Registration

Application Name: Zalando Launcher

Application Type: Desktop Application

Platform: Windows

Microsoft Application (Client) ID:

e086b7f4-cd50-448c-8f60-410127cd3738

Authentication: Microsoft OAuth 2.0 with PKCE

Redirect URI: http://localhost:53682/callback

The application is currently awaiting approval for Minecraft Services authentication.

Development Roadmap

Electron desktop application

Minecraft version retrieval

Minecraft version installation

Java runtime detection

Java runtime installation

Minecraft native library preparation

Minecraft launch configuration preparation

Microsoft OAuth authentication implementation

Xbox Live and XSTS authentication

Minecraft Services application approval

Complete authenticated Minecraft launching

Secure persistent account storage

Improved account management

Mod management

Additional launcher settings

Development

This project is currently being developed and tested on Windows.

A local development environment requires Node.js, npm, and the project's dependencies.

Install dependencies:

npm install

Start the launcher:

npm start

Disclaimer

Zalando Launcher is an independent, unofficial Minecraft launcher project.

It is not affiliated with, endorsed by, sponsored by, or officially associated with Mojang Studios or Microsoft.

Minecraft and related trademarks belong to their respective owners.

Users must comply with the Minecraft End User License Agreement and applicable usage guidelines.

This project does not distribute Minecraft game assets or grant access to the game without a valid license.
