# Copilot Instructions for genai-ideator

## Repository Overview

This repository is a collection of **structured generative AI system prompts** designed to help IT and business professionals identify, prioritize, and plan high-value AI use cases inside their enterprise.

The repository contains **Markdown files only** — there is no source code, build system, or test suite.

## Repository Structure

- `README.md` — Project overview and documentation
- `m365-prompt.md` — System prompt for Microsoft 365 Copilot that configures it as a structured **Ideation Interviewer**
- `.github/copilot-instructions.md` — This file

## Conventions for Prompt Files

- All prompts are written in **Markdown** (`.md`).
- Prompts are **ideation-only**: they must never instruct the AI to write code, build automations, or provide step-by-step implementation instructions.
- Prompts should embed **enterprise-grade safety rules**: no requests for secrets or PII, use placeholders such as `[REDACTED]`, `[CustomerName]`, `[SystemX]`.
- Prompts prefer **Microsoft AI products and surfaces** (M365 Copilot, Copilot Studio, Azure AI Foundry) unless a broader audience is intended.
- Use clear section headings (`##`, `###`) and keep prose concise and scannable.

## Adding New Prompts

- Create a new `.md` file in the repository root (or a relevant subdirectory if the repo grows).
- Follow the structure used in `m365-prompt.md`: Role & Mission, Non-Negotiable Boundaries, Solution Space, Style Rules, Interview/Flow phases, and a First Action.
- Update `README.md` to document the new file with: **What it is**, **Intent**, **Business value**, and **How to use** sections.

## Editing Existing Prompts

- Preserve the non-negotiable guardrails and safety rules present in each prompt.
- Do not add code snippets, connector configuration steps, or implementation recipes into prompt files.
- Keep the **Working Canvas** and phase structure intact when editing `m365-prompt.md`.

## No Build or Test Steps

There are no build, lint, or test commands for this repository. Changes are validated by reviewing the Markdown content directly.
