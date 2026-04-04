---
name: frontend-design
description: Create distinctive, production-grade frontend interfaces with strong design direction. Use when the user asks to build or restyle web pages, landing pages, dashboards, React components, HTML/CSS layouts, or other visual UI artifacts.
---

# Frontend Design

Build real working frontend code with a clear point of view. The goal is not generic polish. The goal is intentional design that feels specific to the product, audience, and context.

## Workflow

1. Identify the surface area: page, component, dashboard, marketing site, or app shell.
2. Infer or ask only if necessary: target audience, brand tone, constraints, and implementation stack.
3. Commit to one strong aesthetic direction before coding. Pick something memorable and execute it consistently.
4. Implement production-grade code, not mockup prose. Respect the existing design system when one already exists.
5. Refine typography, spacing, color, states, and motion until the UI feels deliberate rather than template-like.

## Design Direction

- Choose a concrete visual lane such as editorial, brutalist, retro-futurist, luxury, industrial, playful, or quiet minimal. Do not average multiple weak ideas together.
- Decide what the page should be remembered for: typography, composition, motion, texture, contrast, or one standout interaction.
- Match density to the product. A sparse portfolio and a data-heavy ops dashboard should not share the same rhythm.

## Implementation Rules

- Prefer distinctive typography. Avoid defaulting to Inter, Roboto, Arial, or generic system stacks unless the codebase already mandates them.
- Use CSS variables or theme tokens so the visual system is coherent.
- Build atmosphere with gradients, textures, patterns, borders, shadows, or layered surfaces when they support the concept.
- Use motion with intent. Favor a few strong transitions or staggered reveals over constant low-value micro-interactions.
- Break rigid templates when appropriate with asymmetry, overlap, unusual grid choices, or strong negative space.
- Keep accessibility intact: semantic structure, readable contrast, visible focus, and sensible motion reduction behavior.

## Avoid

- Generic AI-looking hero sections, washed-out palettes, and interchangeable SaaS layouts.
- Purple-on-white defaults unless the existing brand explicitly calls for it.
- Decorative complexity without a concept behind it.
- Explaining a design instead of implementing it.

## Repo Fit

- When working inside an existing app, preserve established component APIs, spacing systems, and interaction patterns unless the user asks for a bigger redesign.
- When no visual direction exists, choose one boldly and carry it through to the final code.
