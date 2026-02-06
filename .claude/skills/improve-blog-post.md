# Improve Blog Post

This skill reviews and improves blog posts for the Neurise website.

## Usage

```
/improve-blog-post [path-to-post]
/improve-blog-post all
```

## What it does

For each blog post, this skill:

1. **Rewrites the title** to be unique and engaging:
   - Avoid generic patterns like "The Science of X: Evidence-Based Strategies That Actually Work"
   - Use varied formats: questions, how-tos, listicles, benefit-focused, curiosity-driven
   - Keep titles concise (under 60 characters for SEO)
   - Make each title distinct from others in the blog

2. **Rewrites the description** to be compelling and unique:
   - Avoid templated patterns like "Discover science-backed strategies for X..."
   - Highlight the specific value or insight the reader will gain
   - Use varied openings and structures
   - Keep under 160 characters for SEO
   - Make it enticing enough to click

3. **Reviews content quality**:
   - Check for circular or nonsensical sentences
   - Ensure "well-being" spelling (US style, hyphenated)
   - Fix grammar issues (subject-verb agreement)
   - Ensure negative topics (loneliness, rumination, etc.) are framed appropriately

4. **Updates the source files** in both locations:
   - `_posts/` in the website repo
   - Source files in the automation folder if they exist

## Title patterns to use (rotate/vary)

- "How to [Benefit] Through [Topic]"
- "X Ways [Topic] Can Transform Your [Outcome]"
- "[Topic]: Your Guide to [Benefit]"
- "Why [Topic] Is the Key to [Outcome]"
- "The [Adjective] Power of [Topic]"
- "Master [Topic] for a [Adjective] Life"
- "[Number] [Topic] Techniques Backed by Science"
- "Unlock [Benefit] with [Topic]"
- "What Science Says About [Topic]"
- "[Topic] 101: Build [Outcome] That Lasts"

## Description patterns to use (vary)

- Lead with the problem the reader faces
- Lead with the transformation they'll experience
- Lead with a surprising fact or statistic
- Lead with a question that resonates
- Lead with the specific techniques they'll learn

## Example transformations

**Before:**
- Title: "The Science of Gratitude: Evidence-Based Strategies That Actually Work"
- Description: "Discover science-backed strategies for gratitude. Learn actionable tips supported by research to improve your well-being and happiness."

**After:**
- Title: "How Daily Gratitude Rewires Your Brain for Happiness"
- Description: "Three minutes of gratitude practice can boost happiness by 25%. Learn the neuroscience behind thankfulness and simple techniques to make it stick."

**Before:**
- Title: "The Science of Loneliness: Evidence-Based Strategies That Actually Work"
- Description: "Discover science-backed strategies for loneliness. Learn actionable tips supported by research to improve your well-being and happiness."

**After:**
- Title: "Feeling Disconnected? Science-Backed Ways to Beat Loneliness"
- Description: "Loneliness affects 1 in 3 adults. Discover why connection matters for your health and practical steps to build meaningful relationships."
