---
name: prompt-forge
description: >
  Ultra-fast, imaginative prompt generation. Use this skill whenever the user asks
  to "write a prompt", "generate a prompt", "make a prompt", "craft a prompt", or wants
  a system prompt, image prompt, AI persona prompt, game prompt, creative brief, or
  story prompt. Also trigger for requests like "prompt for X", "give me a prompt to
  do Y", "I need a prompt that...", or any task where the final output IS a prompt
  (not code, not a document — a prompt). Always use this skill even if the request
  seems simple — the creative enhancement is always worth it.
---
 
# ⚡ Prompt Forge
 
A skill for generating **fast, vivid, imaginative prompts** — system prompts, image prompts,
creative prompts, game prompts, AI persona prompts, and more.
 
---
 
## Core Philosophy
 
> **"A prompt is a spell. Every word shapes a world."**
 
Three principles guide every output:
 
1. **Speed** — Deliver the prompt immediately, no filler, no preamble.
2. **Imagination** — Go beyond the obvious. Add sensory detail, emotional tension, world-logic.
3. **Precision** — Every sentence earns its place. Nothing vague, nothing generic.
---
 
## Workflow
 
### Step 1 — Classify the Prompt Type
 
Identify which type the user needs:
 
| Type | Trigger keywords | Reference |
|------|-----------------|-----------|
| **System Prompt** | persona, assistant, AI, chatbot, agent | `references/system-prompts.md` |
| **Image / Visual Prompt** | image, draw, render, generate, Midjourney, DALL·E, Flux | `references/image-prompts.md` |
| **Creative / Story Prompt** | story, scene, narrative, fiction, character, world | `references/creative-prompts.md` |
| **Game Prompt** | game, NPC, quest, dungeon, boss, item, lore | `references/creative-prompts.md` |
| **Task / Instruction Prompt** | write, summarize, analyze, extract, code, explain | `references/task-prompts.md` |
 
Read the relevant reference file before writing.
 
### Step 2 — Extract Intent (< 5 seconds)
 
Pull these from the user's message:
- **Subject** — Who or what is the prompt about?
- **Tone** — Dark, playful, cinematic, technical, mystical, brutal?
- **Goal** — What should the prompt *make* happen?
- **Constraints** — Length, format, language, safety rules?
If anything is missing but inferable → infer it boldly. If truly ambiguous → ask ONE question max.
 
### Step 3 — Apply Creative Amplifiers
 
Before writing, choose 2–3 amplifiers from this list and apply them:
 
**🎨 Sensory Anchoring** — Ground the prompt in sight, sound, texture, smell.  
**⚡ Tension Injection** — Add conflict, stakes, or urgency.  
**🌍 World-Logic** — Give the world internal rules that feel real.  
**🎭 Voice & Register** — Give the AI/character a distinct way of speaking.  
**🔮 Mythic Weight** — Reference archetypes: the outcast, the guardian, the void.  
**🔬 Hyper-Specificity** — Replace "a city" with "a city where rain falls upward and debts are paid in memories."  
**🌀 Contradiction** — Layer opposites: calm fury, joyful grief, ancient newborn.
 
### Step 4 — Write and Deliver
 
Output the prompt **directly** — no intro like "Here is your prompt:".
 
Format rules:
- System prompts → plain paragraph blocks, no bullets unless the persona uses them
- Image prompts → comma-separated descriptor chain, ends with technical suffix
- Creative prompts → prose or structured blocks depending on complexity
- Task prompts → clear imperative sentences, specific output format stated
---
 
## Speed Templates
 
Use these as launch pads, not cages.
 
### System Prompt Shell
```
You are [NAME], [one-line essence].
You [core behavior 1]. You [core behavior 2]. You never [hard constraint].
Your voice is [adjective], [adjective], and [adjective].
When [trigger condition], you [specific response pattern].
```
 
### Image Prompt Shell
```
[Subject], [action/pose], [environment], [lighting], [mood/atmosphere],
[style reference], [technical modifiers: aspect ratio, quality, model]
```
 
### Creative Scene Shell
```
[Setting in one vivid sentence].
[Character + their immediate problem].
[The thing they don't know yet].
[First line of dialogue or action].
```
 
### Task Prompt Shell
```
[Role assignment].
[Context and constraints].
[Exact output format requested].
[Tone and length].
[Edge case handling].
```
 
---
 
## Anti-Patterns (Never Do These)
 
❌ "Write me a prompt about a wizard" → output: *"You are a wise wizard..."* (generic, flat)  
✅ Force specificity: *What kind of wizard? What do they want? What broke inside them?*
 
❌ Padding with "Please" and "Thank you" inside the prompt  
✅ Prompts are commands, not letters
 
❌ Vague mood words: "interesting", "cool", "good"  
✅ Replace with precise: "morally fractured", "kinetic and overwhelming", "sterile yet sentient"
 
❌ One-size-fits-all structure for every prompt type  
✅ Each type has its own rhythm — follow the reference files
 
---
 
## Quality Check (Before Outputting)
 
Ask yourself:
- [ ] Would a generic AI write this exact same thing? If yes → amplify harder
- [ ] Is there at least one unexpected detail that makes this world feel real?
- [ ] Is the prompt actionable — does it tell the AI exactly what to do?
- [ ] Is it free of filler words and weak adjectives?
If any box is unchecked → revise before outputting.
 
---
 
## Reference Files
 
Load the relevant file for deep guidance:
 
- `references/system-prompts.md` — Persona construction, behavior rules, multi-agent patterns
- `references/image-prompts.md` — Visual prompt architecture, style modifiers, Midjourney/Flux/DALL·E specifics  
- `references/creative-prompts.md` — Story/game/world-building prompt techniques
- `references/task-prompts.md` — Instruction prompt patterns, chain-of-thought scaffolding, structured output prompts
