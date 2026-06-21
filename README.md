# OpenPincer

OpenPincer turns live websites into reliable tools for local AI agents.

Instead of asking agents to guess where to click on a page, OpenPincer builds website-specific tool layers. A ChatGPT tab, a Suno project, a Gmail inbox, or a browser-based studio can expose clear functions such as read state, insert report, generate, list results, or export.

OpenPincer combines:

* WebMCP adapters for website-local tools
* ScriptCat for userscript hosting, sync, and browser-side runtime experiments
* Litter for local agent routing, terminal control, reports, logs, and project memory
* Forge for rebuilding MCP-SuperAssistant-like extensions and automating complex project workflows

The first practical target is rebuilding and surpassing MCP-SuperAssistant Next. The broader target is a browser-agent workbench where websites become stable tool surfaces.

## Components

### Litter

The local server that coordinates local agents, terminal sessions, reports, logs, and project memory.

### WebMCP Adapters

Website-specific userscripts that expose structured tools inside live browser tabs.

### ScriptCat Runtime

A userscript host and possible browser-side runtime for sync, background tasks, and hot reload.

### Forge

The build and migration system for MCP-SuperAssistant Next and later browser-agent extensions.

## First milestone

The first milestone is a minimal ChatGPT WebMCP adapter with four tools:

* get page info
* insert report
* extract explicit bridge commands
* poll local Litter health
