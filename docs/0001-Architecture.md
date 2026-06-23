# MX Flow Architecture

## Overview

MX Flow is an open and composable media workflow platform.

It does not replace existing media software. It connects media providers, AI services, subtitle tools, cache systems, libraries, and players into one unified workflow.

---

## High-Level Architecture

MX Flow is built around seven core modules:

1. Core Engine
2. Workflow Engine
3. Plugin System
4. Media Connectors
5. AI Layer
6. User Interface
7. Configuration Manager

---

## 1. Core Engine

The Core Engine is the center of MX Flow.

It manages system state, module communication, workflow execution, and the connection between different services.

Responsibilities:

- Manage the main application lifecycle
- Coordinate modules
- Provide shared APIs
- Handle internal events
- Maintain system stability

---

## 2. Workflow Engine

The Workflow Engine defines how tasks move through MX Flow.

A workflow may include searching, organizing, subtitle processing, AI analysis, caching, and playback.

Responsibilities:

- Define workflow steps
- Execute workflow tasks
- Support reusable workflow templates
- Allow users to build custom workflows

---

## 3. Plugin System

The Plugin System allows MX Flow to be extended without changing the core application.

Players, providers, subtitle services, AI tools, and download services should all be connectable through plugins.

Responsibilities:

- Load plugins
- Manage plugin permissions
- Provide plugin APIs
- Allow community-built extensions

---

## 4. Media Connectors

Media Connectors connect MX Flow to external media software and services.

Examples may include Kodi, Jellyfin, Emby, Plex, MPV, VLC, NAS systems, cloud storage, and future services.

Responsibilities:

- Connect external applications
- Read media metadata
- Send commands to supported tools
- Bridge different media systems

---

## 5. AI Layer

The AI Layer provides intelligent assistance inside MX Flow.

AI can help with metadata, subtitle matching, translation, workflow suggestions, media organization, and user interaction.

Responsibilities:

- Provide AI-powered suggestions
- Assist media organization
- Support subtitle and metadata tasks
- Help users build workflows

---

## 6. User Interface

The User Interface allows users to view, manage, and control their media workflows.

The UI should be simple, flexible, and focused on reducing friction.

Responsibilities:

- Display media workflows
- Manage plugins and providers
- Show task status
- Provide user controls
- Support future cross-platform design

---

## 7. Configuration Manager

The Configuration Manager stores and manages user settings, plugin settings, workflow templates, and system preferences.

Responsibilities:

- Store user preferences
- Manage plugin configuration
- Manage workflow presets
- Support backup and restore

---

## Design Principles

- Open architecture
- Modular design
- Plugin-first development
- AI-native workflow
- Community extensibility
- User-controlled media experience

---

## Initial Development Direction

The first technical milestone is to build a minimal working structure that includes:

- Basic Core Engine
- Basic Workflow Engine
- Plugin loading concept
- Simple UI placeholder
- Initial documentation

Status: Draft
