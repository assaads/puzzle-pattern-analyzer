# 🧩 Puzzle Pattern Analyzer

An [OpenClaw](https://github.com/openclaw/openclaw) skill for solving word puzzles, odd-one-out questions, and pattern puzzles using advanced multi-hypothesis reasoning, linguistic analysis, and visual pattern recognition.

## What It Does

- **Word puzzles** — finds hidden connections between words using linguistic, semantic, and cultural analysis
- **Odd-one-out** — systematically tests multiple grouping hypotheses before choosing the outlier
- **Pattern puzzles** — detects visual, positional, alphabetical, phonetic, and mathematical patterns
- **Multi-hypothesis reasoning** — never stops at the first plausible answer; generates and ranks at least 5 hypotheses

## Install

```bash
openclaw skills install https://github.com/assaads/puzzle-pattern-analyzer
```

That's it. The skill auto-triggers when you send a puzzle or pattern question to your OpenClaw agent.

## Uninstall

```bash
openclaw skills uninstall puzzle-pattern-analyzer
```

## How It Works

The skill instructs the agent to follow a structured analysis pipeline:

1. **Observe** — catalog all elements (colors, positions, sizes, text types, shading)
2. **Generate** — build semantic networks around each element across multiple domains
3. **Hypothesize** — produce 5+ hypotheses (linguistic, structural, cultural, transformation-based, etc.)
4. **Test** — systematically validate each hypothesis against every element
5. **Rank** — output conventional and creative solution sets, ranked by strength

### Output Format

Every puzzle solution includes:

- **Conventional Solutions** — 5 logical, straightforward explanations ranked #1–#5
- **Far-Fetched Solutions** — 5 unconventional/creative explanations ranked #1–#5

Each solution includes the category, reasoning, visual cues, and which elements are most central.

## Use With

Send any puzzle directly to your OpenClaw agent:

```
Which word is the odd one out: BANK, CASTLE, MOAT, DRAWBRIDGE, TRENCH
```

```
What connects these: MARS, SNICKERS, BOUNTY, TWIX
```

## Structure

```
puzzle-pattern-analyzer/
├── README.md     ← you are here
├── SKILL.md      ← the skill definition
└── LICENSE       ← MIT
```

## Skill Definition

The full skill is in [`SKILL.md`](./SKILL.md). It's a single file — no scripts or dependencies needed.

## License

MIT
