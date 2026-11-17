# Course Menu (where Jerome is)

▶ = current position. ✅ = done. Built word for word from the lesson's own structure.
Update the pointer every time we move. Show the breadcrumb at the top of every teaching reply.

**Current breadcrumb:**
Module 1 > Part 1 > 🧠 How a model is made > Training is a guessing game > Step 2 > Side trip: How ML works > Foundations > ▶ How a computer works: ones and zeros

---

## Module 1: How diffusion works

### Part 1: The four parts

#### 🧠 How a model is made
- **Training is a guessing game, repeated billions of times**
  - Step 1: Take a real image along with its caption
  - ▶ Step 2: Add a *known* amount of noise to it
    - ✅ What noise is (random static, pixel-by-pixel random nudges)
    - ✅ What "a known amount" means (the dial from 0 to 100%, and the computer keeps the receipt)
    - ✅ Why does it need to be noise? (we teach it to clean, not to draw, because we made the mess so we always have the answer)
    - ▶ SIDE TRIP: How machine learning works (Jerome's questions, one at a time)
      - ✅ Is this machine learning? What is a model? (a file of numbers, not Python code)
      - ▶ Foundations first (Jerome wants to go to the bottom and build up)
        - ▶ How a computer works: ones and zeros (bits and bytes)
        - How a computer runs instructions
        - Who invented machine learning, and how
        - How machine learning actually works inside a computer
        - What coding language they use to build and train models (Python, PyTorch, CUDA on the GPU)
      - Other ways to train a model besides noise
      - Quick skim of all image model types (diffusion, Grok, ChatGPT, others)
      - Other concepts besides models
  - Step 3: Ask the model: "What noise did I add?"
  - Step 4: It guesses, and the guess gets compared to the real answer
  - Step 5: Its internal numbers (weights) get nudged to be a little less wrong
  - Step 6: Repeat with millions of images
  - Pure noise plus a caption: "finding" an image that was never there
- **A checkpoint** (saved snapshot of weights, `.safetensors`)
- **Base model vs fine-tune**
  - Base model
  - Fine-tune (Illustrious, NoobAI on Danbooru)
- 💡 Why anime models understand Danbooru tags

#### 📝 How the text encoder is made
- How it learned (matching images and text in "number space")
- What happens to your prompt
  - Tokens
  - Lists of numbers
  - Fed in at every cleaning step
- Key facts
  - CLIP (two of them)
  - 77-token chunks
  - Tags vs sentences, newer encoders (T5, LLMs)

#### 🎨 The sampler: not trained at all
- Pure math, not AI
- What the sampler decides
- Sampler vs scheduler
- 💡 Ancestral samplers (euler_a)

#### 🖼️ The VAE: the compressor
- The problem (3 million numbers)
- The fix: the latent (latent diffusion)
- Two halves: encoder and decoder
- How it's made
- ⚠️ Wrong or missing VAE = washed-out colors

#### The full picture in one line
- Quick check (unanswered): Which of the 4 parts is not AI, and why does that matter?

### Part 2: The settings you control
- Steps
- CFG
- Seed

---

## Modules 2 to 9
2. The anime model landscape
3. ComfyUI from zero
4. Prompting for anime models
5. Character accuracy
6. Style accuracy
7. Control
8. Training my own LoRAs
9. Production systems
