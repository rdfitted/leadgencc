# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Personal Branding workspace directory used for generating content related to personal branding, marketing materials, and professional positioning. The directory also serves Claude Code configuration and session management. 

## Directory Structure

- `.claude/` - Claude Code configuration directory
  - `agents/` - Custom agent configurations (currently empty)
  - `commands/` - Custom command definitions (currently empty)
- `ai_docs/` - Strategic documentation for AI positioning and messaging
- `Client Stories/` - Client conversations, situations, insights, and case studies
- `logs/` - Session tracking and status information
  - `status_line.json` - Claude Code session metadata and cost tracking

## Usage Notes

This directory primarily serves as:
- A workspace for generating personal branding content (social media posts, marketing copy, professional bios, etc.)
- Configuration storage for custom agents and commands  
- Session logging and cost tracking

No specific build tools, dependencies, or development commands are configured for this workspace.

## Content Generation Focus

When working in this directory, prioritize:
- Creating compelling personal branding content
- Developing marketing materials and messaging
- Crafting professional positioning statements
- Generating social media content and engagement strategies

## Content Source Guidelines

When generating content, leverage these resources:
- **ai_docs/**: Reference strategic documentation for consistent AI positioning and messaging
- **Client Stories/**: Draw from client conversations, situations, insights, and case studies to inform authentic content creation
- Use these materials to ensure content aligns with established positioning and incorporates real-world experiences

## Key Reference Documents

**Start with these foundational documents when generating content:**
- **Business_Owners_Mirror_Report.md** - Core identity, strengths, blind spots, voice prompts, and signature themes for Ryan Duffy/Fitted Automation
- **LinkedIn_Post_Frameworks.md** - Tactical templates, hooks, and structures for high-performing LinkedIn content
- **Proprietary_Systems_Framework.md** - Detailed breakdown of Ryan's business frameworks, client-facing assets, and vertical solutions for content authenticity

These documents provide the strategic foundation and tactical execution framework for all content creation.

## Output Formatting Guidelines

- **Documents for history/storage**: Use Markdown format (.md files) for all saved documents, templates, and reference materials
- **Content outputs**: Provide final content outputs as formatted plain text (ready to copy/paste into platforms, emails, etc.)
- This ensures documents are well-organized for future reference while outputs are immediately usable

## LinkedIn Posting Integration

When asked to post content to LinkedIn, use the pd-linkedin MCP server with these tools:

**Available Tools:**
- `mcp__pd-linkedin__linkedin-post` - Create and publish LinkedIn posts
- `mcp__pd-linkedin__linkedin-create-post` - Alternative posting method
- `mcp__pd-linkedin__linkedin-search-organization` - Search for organizations on LinkedIn
- `mcp__pd-linkedin__linkedin-get-multiple-member-profiles` - Retrieve member profile data

**Usage Example:**
```
mcp__pd-linkedin__linkedin-post
- text: [post content]
```

**Configuration:** The LinkedIn MCP server is configured in `.mcp.json` as `pd-linkedin` pointing to the Pipedream gateway endpoint.