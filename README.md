# Generative AI Ideator

A collection of structured generative AI prompts designed to help IT and business professionals identify, prioritize, and plan high-value AI use cases inside their enterprise.

---

## m365-prompt.md - M365 Copilot ideator

### What it is

`m365-prompt.md` is a **system prompt** you paste into Microsoft 365 Copilot to turn it into a structured **Ideation Interviewer**. The prompt configures the AI to conduct a guided, multi-phase interview with you—uncovering your workflows, pain points, and constraints—and then produce a prioritized list of realistic generative AI use cases along with lightweight pilot plans.

### Intent

The prompt is deliberately **ideation-only**: it instructs the AI never to write code, build automations, or provide step-by-step implementation instructions. Instead it focuses on four phases:

1. **Setup** – understands your role, team, success criteria, and available Microsoft 365 surfaces.
2. **Workflow Deep Dive** – maps the triggers, steps, tools, handoffs, and failure modes of up to two workflows you choose.
3. **Use-Case Generation** – produces a broad set of candidate AI ideas across categories such as drafting, summarization, knowledge retrieval, decision support, service management, and governance—biased toward Microsoft AI products (M365 Copilot, Copilot Studio, Azure AI Foundry).
4. **Prioritization & Pilot Planning** – scores ideas on impact, effort, risk, and confidence, then outputs a NOW / NEXT / LATER roadmap plus a concrete two-week pilot plan (including prompt starters) for the top use cases.

The prompt also embeds enterprise-grade safety rules: it refuses to request or store secrets or PII, applies challenge-and-alternative pushback when ideas are risky or unclear, and keeps all guidance conceptual so that a separate engineering team handles any eventual build.

### Business value

| Value driver | How the prompt delivers it |
|---|---|
| **Faster time-to-ideation** | A structured interview replaces ad-hoc brainstorming sessions, producing a prioritized use-case list in a single conversation. |
| **Realistic, enterprise-safe ideas** | Built-in guardrails prevent the AI from suggesting ideas that expose PII, require unavailable data, or duplicate existing tooling. |
| **Microsoft-platform alignment** | All suggestions are anchored to M365 Copilot surfaces, Copilot Studio, and Azure AI Foundry—reducing procurement risk and licensing friction. |
| **Role-specific relevance** | Eight IT role tracks (leadership, cloud/Azure, DevOps, ops/SRE, security, data, service desk, program management) ensure ideas match the user's actual responsibilities. |
| **Pilot-ready output** | Each top use case comes with success metrics, a stakeholder list, a two-week experiment plan, guardrails, and ready-to-run prompt starters—so teams can move from idea to experiment without external consultants. |
| **Scalable across the organization** | Any IT or business professional can run the prompt independently, multiplying the ideation capacity of a single AI/innovation team. |

### How to use

1. Open Microsoft 365 Copilot.
2. Paste the full contents of `m365-prompt.md` as the system prompt or custom instructions.
3. The AI will ask its first interview question. Answer each question in turn—the conversation guides itself.
4. At the end of the session, export or copy the Ideation Notes, scored use-case table, and pilot plans to a document for stakeholder review and collaboration.
