# Everything Jerome has learned (running log)

Add every new learning here, in plain words, in the order it was learned. Mark ⚠️ if it didn't land and needs another try.

## Module 1 > The Model > How it's trained
1. Noise is random static, like TV snow. Every pixel's color gets nudged by a random amount.
2. "A known amount" of noise is a dial from 0% (clean) to 100% (pure static). The computer writes down exactly what it added, so it keeps the receipt.
3. Why noise: you can't teach a computer to draw from nothing because there's no right answer to grade it on. So we mess up a real picture with noise and teach it to clean. We made the mess, so we always know the answer. (Photo restorer idea: clean so well that "cleaning" pure static becomes drawing.)

## Side trip: How machine learning works
4. Yes, this is machine learning. Machine learning means instead of writing rules by hand, you show a computer tons of examples and it adjusts itself until it gets good.
5. A model is not Python code. It's a giant file of numbers (billions), and those numbers are the weights.
6. ⚠️ Song file vs music player analogy (model = song, ComfyUI = player). Did NOT land, because Jerome doesn't know ComfyUI yet. Don't use analogies built on things he hasn't learned.
7. ⚠️ Transistors = tiny on/off switches, on = 1, off = 0, one switch = a bit. Jerome ALREADY KNEW this. Skip basics he knows; he wants the "how does that become a computer" mechanism.
8. Binary = writing numbers using only 0 and 1. Switches wired together into logic gates (AND, OR, XOR) can make decisions, and a few gates together can add numbers. That's how a calculator is made from switches.
