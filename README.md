# Font Expert for Claude Code

A custom Claude Code subagent for choosing and implementing typography in newspapers, printed props, labels, screens, and physical 3D signs.

Font Expert makes a final, context-specific font decision, creates meaningful text and layouts, and checks the actual rendered result when the required tools are available. It preserves your project's established character design and caption style.

## Install

Repository: [reelaspect9-gif/claude-font-expert](https://github.com/reelaspect9-gif/claude-font-expert)

Agent file: [view the subagent](https://github.com/reelaspect9-gif/claude-font-expert/blob/main/.claude/agents/font-expert.md) · [download raw Markdown](https://raw.githubusercontent.com/reelaspect9-gif/claude-font-expert/main/.claude/agents/font-expert.md)

Download [font-expert.md](.claude/agents/font-expert.md) and save it in one of these locations:

- **One project:** `<your-project>/.claude/agents/font-expert.md`
- **All your projects:** `~/.claude/agents/font-expert.md`

Preserve any existing agent with the same name before replacing it. Keep the filename ending in `.md`, with the YAML frontmatter at the beginning. If Claude Code does not discover the agent, check the project location and start a fresh session.

This follows [Claude Code's documented custom-subagent format](https://code.claude.com/docs/en/sub-agents): a Markdown file with `name` and `description` in YAML frontmatter, followed by the agent instructions. It is a subagent, not a replacement animation skill, MCP server, or executable plugin. No GitHub key is needed to download this public file.

If a definition already exists, retain it and prepare the proposed additions separately. A backup alone does not authorize overwriting existing instructions; obtain explicit permission before replacement. For a new installation, create only the missing agent file.

## Use

Ask Claude Code to delegate explicitly:

> Use the font-expert subagent to choose, implement, and verify typography for the newspaper and storefront sign in this scene. Read the project brief first. Preserve the existing character and caption design.

Include the era, location, language, exact wording or scope for original copy, asset dimensions, camera distance, output resolution, relevant references, and files the agent may edit. For a more focused task:

> Use font-expert to choose the masthead, headline, and body typography for a reconstructed 1920s newspaper. Research relevant examples, write coherent original supporting copy, and retain editable text. Compare candidates using the real headline, choose the final fonts, and inspect the layout at its intended screen size. Do not substitute black bars for text.

For dimensional signs:

> Use font-expert to build the sign lettering as actual glyph geometry or modeled engraving. Check spacing, counters, bevels, materials, attachment, and readability from the shot camera. Preserve editable wording before converting it to meshes.

The agent is invoked by delegation; installing it does not automatically create a `/font-expert` slash command.

## What it covers

- Contextual font research and a decisive selection for each typographic role.
- Meaningful newspaper and document copy, grids, hierarchy, and print treatment.
- Physical 3D lettering with proper depth, counters, spacing, and material integration.
- Font-file verification, licensing records, multilingual glyph coverage, and text shaping.
- Actual render and motion checks for readability, clipping, fallback fonts, aliasing, and shimmer.
- Editable source files, a font manifest, proof artifacts, and honest reporting of unfinished checks.

## Requirements and limits

Use Claude Code with custom subagents available. Research, font inspection, layout, and 3D rendering depend on the tools and permissions in your own environment. This repository does not install fonts or rendering software, provide service credentials, or bundle copyrighted font binaries.

The agent definition has been reviewed for structure and self-contained instructions. It has not been live-tested in Claude Code or validated by producing a finished scene. A prompt cannot guarantee a perfect font match; the agent must distinguish verified identification from an approximation and inspect the actual output.
