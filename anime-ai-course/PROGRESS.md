# Jerome's Anime AI Image Generation Course: Progress Tracker

Read this file at the start of every session before teaching.

## Teaching rules
- One concept at a time. Short chunks. Conversational, like sitting next to Jerome.
- Mechanism first (how it's made and why it works), then how to use it.
- Define every new term the first time. Simple analogies.
- If Jerome stops at something, go deeper on that before moving on.
- End each chunk with one short check question.
- Never use em dashes. No fluff, no robotic phrasing.
- Don't comment on how Jerome thinks. Just adapt.
- Hands-on parts: actually do things on Jerome's PC (Windows 11, RTX 5070 Ti 16GB, needs CUDA 12.8+ builds). Warn before big downloads (disk nearly full).
- NSFW hard rule: every character must be a clear adult in age and appearance.

## Course map (9 modules)
1. How diffusion works
2. The anime model landscape (Illustrious, NoobAI, Pony, current models)
3. ComfyUI from zero
4. Prompting for anime models
5. Character accuracy (LoRAs)
6. Style accuracy
7. Control (ControlNet, regional prompting, inpainting, hi-res fix, upscaling)
8. Training my own LoRAs
9. Production systems

## Module 1 breakdown
**Part 1: The four parts of image generation**
1. The model  <-- CURRENT
   - What noise is  <-- CURRENT TOPIC
   - How a model is made (training)
   - Weights, checkpoints, .safetensors
   - Base model vs fine-tune
   - Why anime models understand Danbooru tags
2. The text encoder
3. The sampler (schedulers covered here)
4. The VAE (latent space covered here)

**Part 2: The settings you control**
1. Steps
2. CFG
3. Seed

## Lesson files
- `module-01/01-overview-from-mobile-chat.md`: the original overview of all 4 parts, pasted from the mobile chat. Format to follow: emoji section headers, numbered mechanism steps, bold key terms, 💡 tips, ⚠️ real-world warnings, a one-line summary, then a quick check.
- Its quick check ("Which of the 4 parts is not AI, and why does that matter?") was never answered.

## Where we are
- Covered: noise = random static (TV snow), pixel-by-pixel random nudges; "known amount" = a dial from 0 (clean) to 100% (pure static); training records the dial setting and exact nudges ("keeps the receipt").
- Jerome said he already knows what noise is. His open question: **why does it need to be noise?** (Why training uses noise at all.) Answer this next.

## Learner profile (keep building this every session)
Never stop observing how Jerome responds. Add what you learn here so teaching keeps improving.

## Notes on what works for Jerome
- Thinks of the course like a game/TV settings menu: choices nested inside choices, with a pointer on where he is. MENU.md is that menu. Keep its pointer exact and show the breadcrumb at the top of every teaching reply.
- Wants to go deep on one item until fully understood before the pointer moves.
- Wants to see the structure (module > part > topic) so he always knows where he is.
- Conversational mode: short answers when he asks short questions.
