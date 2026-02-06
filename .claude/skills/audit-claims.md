# Audit Claims

This skill reviews content for claims about Neurise app features to ensure we don't overpromise.

## Usage

```
/audit-claims [path-to-file]
/audit-claims all
```

## What it does

1. **Scans content** for claims about what Neurise does or offers
2. **Compares against verified features** in `.claude/verified-features.md`
3. **Flags unverified claims** that might overpromise
4. **Reports findings** with specific quotes and locations

## What to look for

### Feature claims
- "Neurise helps you..."
- "Our app provides..."
- "With Neurise you can..."
- "The app includes..."
- "Features like..."

### Outcome claims
- "You'll see results in..."
- "Proven to increase..."
- "Guaranteed to..."
- "Will make you happier..."

### Comparison claims
- "Better than..."
- "The only app that..."
- "Unlike other apps..."

## How to audit

1. Read the content file
2. Identify any claims about features or outcomes
3. Check each claim against `.claude/verified-features.md`
4. For unverified claims, report:
   - The exact quote
   - File and line number if possible
   - Whether it's a feature claim or outcome claim
   - Suggested action (remove, soften, or add to verified list)

## Output format

```
## Audit Report: [filename]

### Verified Claims
- [quote] ✓

### Unverified Claims
- [quote] — File:line — Suggested action

### Recommendations
- [summary of changes needed]
```

## After auditing

If a claim is legitimate and the feature exists:
1. Add it to `.claude/verified-features.md`
2. Note the date verified

If a claim is overpromising:
1. Flag for removal or softening
2. Suggest alternative wording
