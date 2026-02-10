# Image Generation Instructions for Angle 01 - Drinking Exec

**Status:** Awaiting OpenAI API key to generate images

## Required Images

### 1. Hero Image: `angle-01-hero.png`

**Placement:** Top of landing page, right after headline

**DALL-E 3 Prompt:**
```
Professional man in his late 30s or early 40s, athletic build around 190 lbs, confident and peaceful expression, wearing a casual button-down shirt, warm and approachable demeanor, standing in modern minimalist home office with natural lighting, transformation and renewal energy, photorealistic style, cinematic lighting, representing a successful tech executive who has overcome personal struggles
```

**Specs:**
- Model: DALL-E 3
- Quality: HD
- Size: 1792x1024 (landscape)
- Style: natural

**Generation Command:**
```bash
python3 /opt/homebrew/lib/node_modules/openclaw/skills/openai-image-gen/scripts/gen.py \
  --model dall-e-3 \
  --prompt "Professional man in his late 30s or early 40s, athletic build around 190 lbs, confident and peaceful expression, wearing a casual button-down shirt, warm and approachable demeanor, standing in modern minimalist home office with natural lighting, transformation and renewal energy, photorealistic style, cinematic lighting, representing a successful tech executive who has overcome personal struggles" \
  --quality hd \
  --size 1792x1024 \
  --style natural \
  --out-dir /Users/hydi/.openclaw/workspace/dgm/landing-pages/assets
```

---

### 2. Before/After Concept: `angle-01-before-after.png`

**Placement:** Middle section, "What Happened Next"

**DALL-E 3 Prompt:**
```
Split-screen before and after transformation concept: LEFT side shows a tired, overweight man in his 40s looking defeated and stressed in dim lighting, slumped posture, representing struggle and exhaustion. RIGHT side shows the same man transformed, fit and athletic at 190 lbs, confident posture, bright natural lighting, peaceful and powerful expression, representing renewal and victory. Modern photorealistic style, dramatic lighting contrast, inspiring transformation narrative
```

**Specs:**
- Model: DALL-E 3
- Quality: HD
- Size: 1792x1024 (landscape)
- Style: vivid

**Generation Command:**
```bash
python3 /opt/homebrew/lib/node_modules/openclaw/skills/openai-image-gen/scripts/gen.py \
  --model dall-e-3 \
  --prompt "Split-screen before and after transformation concept: LEFT side shows a tired, overweight man in his 40s looking defeated and stressed in dim lighting, slumped posture, representing struggle and exhaustion. RIGHT side shows the same man transformed, fit and athletic at 190 lbs, confident posture, bright natural lighting, peaceful and powerful expression, representing renewal and victory. Modern photorealistic style, dramatic lighting contrast, inspiring transformation narrative" \
  --quality hd \
  --size 1792x1024 \
  --style vivid \
  --out-dir /Users/hydi/.openclaw/workspace/dgm/landing-pages/assets
```

---

### 3. ASKING Framework Visual: `angle-01-asking-framework.png`

**Placement:** Method explanation section, after "The ASKING Framework: 3 Minutes to Rewire Your Identity"

**DALL-E 3 Prompt:**
```
Clean infographic diagram showing the ASKING framework with 6 steps arranged in a circular flow: A (Awareness) - notice feelings, S (Sensations) - body awareness, K (Knowing) - truth recognition, I (Imagine) - visualization, N (Nurture) - feeling embodiment, G (Generate) - action. Modern minimalist design with soft gradient background in purple and blue tones, clear typography, icons for each step, professional coaching aesthetic, easy to read and understand
```

**Specs:**
- Model: DALL-E 3
- Quality: HD
- Size: 1024x1024 (square)
- Style: natural

**Generation Command:**
```bash
python3 /opt/homebrew/lib/node_modules/openclaw/skills/openai-image-gen/scripts/gen.py \
  --model dall-e-3 \
  --prompt "Clean infographic diagram showing the ASKING framework with 6 steps arranged in a circular flow: A (Awareness) - notice feelings, S (Sensations) - body awareness, K (Knowing) - truth recognition, I (Imagine) - visualization, N (Nurture) - feeling embodiment, G (Generate) - action. Modern minimalist design with soft gradient background in purple and blue tones, clear typography, icons for each step, professional coaching aesthetic, easy to read and understand" \
  --quality hd \
  --size 1024x1024 \
  --style natural \
  --out-dir /Users/hydi/.openclaw/workspace/dgm/landing-pages/assets
```

---

## Setup Required

Before running the commands above, ensure:

1. OpenAI API key is set as environment variable:
   ```bash
   export OPENAI_API_KEY="sk-..."
   ```

2. Or add to shell profile (~/.zshrc or ~/.bash_profile):
   ```bash
   echo 'export OPENAI_API_KEY="sk-..."' >> ~/.zshrc
   source ~/.zshrc
   ```

3. Verify the key is set:
   ```bash
   echo $OPENAI_API_KEY
   ```

## After Generation

Once images are generated:
1. Rename files to match the expected filenames if needed
2. Verify images are in `/Users/hydi/.openclaw/workspace/dgm/landing-pages/assets/`
3. Test the HTML landing page to ensure images load correctly
4. Consider optimizing images for web (compress if needed)

## Notes

- DALL-E 3 generates one image at a time (count is automatically limited to 1)
- HD quality provides the best results for landing page hero images
- Natural style is more photorealistic, vivid style is more dramatic
- Generation takes approximately 10-30 seconds per image
- Estimated cost: ~$0.12 per HD image (1792x1024) or ~$0.08 per standard image (1024x1024)

---

**Created:** 2026-02-09  
**Status:** Ready for generation once API key is available
