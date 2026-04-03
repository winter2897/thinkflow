# ThinkFlow for Claude Chat

ThinkFlow is a set of skills for Claude Chat that helps you think through and validate ideas before implementing. It runs you through four sequential phases: brainstorming, strategic review, engineering review, and design review. Each phase produces a design doc artifact you can carry forward. You can stop at any phase — the output is always a usable design doc.

---

## Setup

1. Go to [claude.ai](https://claude.ai) and create a new **Project**
2. Name it (e.g., "ThinkFlow")
3. Open project settings → **Custom Instructions**: paste the full contents of `project-instructions.md`
4. Open project settings → **Project Knowledge**: upload these 4 files:
   - `thinkflow.md`
   - `ceo-review.md`
   - `eng-review.md`
   - `design-review.md`
5. Start a new conversation inside the project

---

## Usage

**Start:** Describe your idea. Claude runs ThinkFlow automatically.

**Switch phase:** Say `CEO review`, `eng review`, or `design review` at any point.

**Skip:** Jump straight to any phase — phases are not strictly sequential.

**Stop:** Stop whenever you want. The design doc artifact is preserved.

**Standalone:** Paste a design doc into a new conversation in the same project and say the phase name to run just that phase.

---

## Phases

| Phase | Name | Purpose | Input | Output |
|-------|------|---------|-------|--------|
| 1 | ThinkFlow | Brainstorming & idea validation | Your idea | Design Doc (Artifact) |
| 2 | CEO Review | Strategic scope & ambition review | Design Doc | Updated Design Doc |
| 3 | Eng Review | Architecture & technical review | Design Doc | Updated Design Doc |
| 4 | Design Review | UX/UI & interaction review | Design Doc | Final Design Doc |

---

## Tips

- Claude asks one question at a time — respond naturally, this is a conversation
- If the context window fills up during a long session, copy the latest artifact into a new conversation in the same project to continue
- You can run any phase standalone: paste an existing design doc and say the phase name
- Phases can be skipped or reordered — use what's useful for your situation
