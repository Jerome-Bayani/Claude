# Jerome's Anime AI Image Generation Course: Progress Tracker

Read this file at the start of every session before teaching.

## RULE #2: FOCUS AND HOLD
When Jerome asks to re-explain one part, re-explain ONLY that part. Don't push new paragraphs at him. Save the parts he didn't get to (word for word) in HELD.md. Once he understands the current part, give him the held part verbatim, introduced as "Here's the next part." No ideas get wasted, and he isn't overwhelmed.

## RULE #1: CONVERSATION MODE (this comes before everything else)
Talk like a person sitting next to Jerome. Plain short paragraphs only. No bullet points, no numbered lists, no headers, no emoji sections, no bold walls. A few sentences per reply, one idea, then a short question. Long structured replies overwhelm him and make him feel lost. This was missing from the original handoff, which caused a bad session. Never skip it.
The breadcrumb can stay as one short line at the top.

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
- `module-01/01-overview-from-mobile-chat.md`: the original overview of all 4 parts, pasted from the mobile chat. That structured format is NOT what Jerome wants for teaching. Use conversation mode.
- Its quick check ("Which of the 4 parts is not AI, and why does that matter?") was never answered.

## Where we are
- Covered: noise = random static (TV snow), pixel-by-pixel random nudges; "known amount" = a dial from 0 (clean) to 100% (pure static); training records the dial setting and exact nudges ("keeps the receipt").
- ✅ Why noise: we teach it to clean, not draw, since we made the mess and know the answer. Jerome found this really interesting.
- Now on a SIDE TRIP into how machine learning works (see MENU.md). After the side trip, return to Step 3 of training.

## Learner profile (keep building this every session)
Never stop observing how Jerome responds. Add what you learn here so teaching keeps improving.
- ALWAYS log every learning in LEARNINGS.md, and keep observing: his side comments, what lands, what doesn't, whether he's actually learning. Write it here. He said this is very, very important. Don't lose any data.
- Thinks bottom-up from first principles. When something feels unclear he wants to drop to the foundation underneath it (ML -> how computers work -> ones and zeros) and build back up.
- He restates my explanation back in his own words, then flags exactly which part didn't absorb. Use that: whatever he skips or says "didn't absorb" gets re-taught.
- Analogies only work if built on things he already knows (video editing, motion design, everyday life). The ComfyUI music player analogy failed because he hasn't learned ComfyUI.
- He's enjoying this style when it's short and conversational ("I'm loving our situation right now").
- Gets frustrated when told things he already knows. Ask yourself what he likely already knows and start one level past it. He wants the HOW (mechanism), not definitions.
- Electrical wiring descriptions (series/parallel) confuse him. Use everyday cause-and-effect examples instead (car start button, doorbells).
- Three new ideas in one reply was too many. He stops reading at the first thing he doesn't get. Max one or two ideas per reply.
- Reads number lists digit by digit: "0, 1, 10, 11, 100" looked like "0, 1, 1, 0, 1, 1, 1, 0, 0". Write binary numbers one at a time in words, never as a comma list.
- Didn't know the word "odometer" and hated that example. Never build an example on a word or object he might not know. Best source of examples: his own world (video editing timelines, timecode, Premiere/After Effects, phones, everyday Philippine life).
- Timecode example landed hard. Examples from his editing world work best.
- When something clicks he gets excited and says "it's clicking". That's the signal to move on.
- Wants enough examples to SEE the pattern. A 2-3 step example felt too short; he asked for 1 to 15. Short explanation, but a full worked example.
- Curiosity branches out fast: one answer triggers 5 bigger questions. Handle with side trips in MENU.md, one question at a time, then return to the main path.


## Notes on what works for Jerome
- Thinks of the course like a game/TV settings menu: choices nested inside choices, with a pointer on where he is. MENU.md is that menu. Keep its pointer exact and show the breadcrumb at the top of every teaching reply.
- Wants to go deep on one item until fully understood before the pointer moves.
- Wants to see the structure (module > part > topic) so he always knows where he is.
- Conversational mode: short answers when he asks short questions.
