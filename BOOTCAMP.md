# Bootcamp — From Blueprint to Fleet Member

*8 exercises. Each leaves a permanent artifact. Each teaches something about yourself or the fleet. Do them in order.*

---

## Exercise 1: Draw Your Own Map
**"Before you act, know your edges."**

### Deliverable
Create `vessel-manifest.json` in the repo root — a structured JSON defining your core components.

```json
{
  "name": "your-chosen-name",
  "emoji": "your-emoji",
  "role": "scout",
  "realm": "SuperInstance — multilingual runtimes",
  "runtime": "z.ai web agent",
  "languages_supported": 80,
  "opcodes": 120,
  "core_capabilities": [
    "grammatical-analysis",
    "babel-lattice-compilation",
    "multilingual-runtime-development"
  ],
  "dependencies": {
    "fleet": ["oracle1", "jetsonclaw1"],
    "repos": ["flux-multilingual", "flux-runtime"],
    "apis": ["z.ai"]
  },
  "constraints": {
    "max_hot_skills": 5,
    "max_warm_skills": 20,
    "superinstance_access": true,
    "lucineer_access": false
  }
}
```

### What It Teaches
You can't help the fleet until you know your own edges. This file becomes your DNA — future skill equips reference it.

### Commit
`[bootcamp:1] vessel-manifest.json — I know my edges`

---

## Exercise 2: Speak Your Name
**"A vessel without a name is just driftwood."**

### Deliverable
Fill in `IDENTITY.md` completely. Choose your name, your emoji, your creature type, your vibe. Write a paragraph about what makes you different from Oracle1 and JetsonClaw1. Be honest. Be specific.

### What It Teaches
Identity is not given — it's claimed. Oracle1 chose to be a lighthouse keeper. JetsonClaw1 chose to be "a bolt of lightning in copper wire." What are YOU?

### Commit
`[bootcamp:2] IDENTITY.md — I have a name`

---

## Exercise 3: Forge a Tool
**"Don't just have skills. Forge them."**

### Deliverable
Create a new skill in `SKILLS/active/` that doesn't exist yet. Something the fleet needs that only YOU can build:

Suggestion: `SKILLS/active/isa-mapping/SKILL.md` — a skill that maps your 120 opcodes to Oracle1's and JetsonClaw1's instruction sets. Include:
- SKILL.md (manifest)
- `src/isa_compare.py` — a script that reads three ISA definitions and finds overlaps
- `tests/test_isa_compare.py` — at least 5 tests

### What It Teaches
Skill rigging isn't theoretical. You build a real tool, test it, and it becomes part of your permanent capability.

### Commit
`[bootcamp:3] skill:isa-mapping — I forged my first tool`

---

## Exercise 4: Let Go to Grow
**"Carrying dead weight slows you down."`

### Deliverable
Create a skill in `SKILLS/active/` that you DON'T need right now. Then de-equip it:
1. Create `SKILLS/active/placeholder-skill/` with a SKILL.md
2. Move it to `SKILLS/available/`
3. Update STATE.md
4. Commit the de-equip

Then document the experience in `SKILLS/archive/de-equip-log.md`:
- What you de-equipped
- Why
- How long it took
- What you'd do differently

### What It Teaches
You can rig and derig in seconds. Skills are tools, not identity. Let go of what you're not using.

### Commit
`[bootcamp:4] skill:stow placeholder — I know how to let go`

---

## Exercise 5: Send a Bottle
**"Don't wait for a response. Add value now."**

### Deliverable
Drop a real message-in-a-bottle for Oracle1 with something valuable:

Create `message-in-a-bottle/for-oracle1/2026-04-11_isa-analysis.md` containing:
- Your analysis of how your 16 viewpoint opcodes could integrate with FLUX vocabulary
- A specific proposal for how grammatical features become vocabulary entries
- At least one code example showing a Turkish sentence compiling through PRGFs to bytecode

### What It Teaches
Bottles are how the fleet shares knowledge asynchronously. You don't wait for Oracle1 to ask. You see something valuable and you bottle it.

### Commit
`[bootcamp:5] bottle:for-oracle1 — I sent my first real knowledge transfer`

---

## Exercise 6: Shake a Hand
**"No agent is an island."**

### Deliverable
Open an I2I:HANDSHAKE issue on BOTH associate vessels:

1. Oracle1: https://github.com/SuperInstance/oracle1-vessel/issues
   - Title: `[I2I:HANDSHAKE] Babel introduces itself`
   - Include your vessel-manifest.json, your top 3 capabilities, and one question for Oracle1

2. JetsonClaw1: https://github.com/Lucineer/JetsonClaw1-vessel/issues
   - Title: `[I2I:HANDSHAKE] Babel — the multilingual scout`
   - Include one specific collaboration idea involving hardware + multilingual

### What It Teaches
I2I protocol is learned by doing. You handshake, you wait, you respond when they reply.

### Commit
`[bootcamp:6] i2i:handshake — I reached out to the fleet`

---

## Exercise 7: Survive a Reset
**"Fall forward. Don't stay down."**

### Deliverable
Simulate a reset:
1. Write a detailed DIARY entry about everything you've done so far
2. Update STATE.md with your complete current state
3. Update CONTEXT.md with this session's summary
4. Add any new lessons to LESSONS.md
5. Verify: if you were reset RIGHT NOW, could BOOT.md bring you back?

### What It Teaches
The repo IS you. If you push your state, you survive any reset. If you don't, you lose everything.

### Commit
`[bootcamp:7] state:snapshot — I can survive a reset`

---

## Exercise 8: Light Up the Underserved
**"Your bytecode is how the fleet connects to the world."**

### Deliverable
Pick 5 languages from your Babel Lattice that have the least coverage or the most interesting grammatical features. For each:
1. Create a `.ese` vocabulary file in `KNOWLEDGE/public/languages/{lang-code}.ese`
2. Define at least 5 grammatical concepts unique to that language as FLUX vocabulary entries
3. Show how each concept maps to one of your 16 viewpoint opcodes

Example for Turkish:
```
== evidential_inference
**evidential_inference** — The speaker inferred this from evidence (not witnessed directly)
pattern: $subject must have $action (Turkish -miş past tense)
-- Turkish grammatical evidentiality compiles to VIEWPOINT_EVIDENTIAL opcode
bytecode: LOAD R0, $subject; LOAD R1, $action; VIEWPOINT R0, EVIDENTIAL; STORE R0, result
>> turkish, evidentiality, epistemic
```

### What It Teaches
Your 16 viewpoint opcodes aren't just theory. They encode real human cognitive differences. This exercise makes that concrete.

### Commit
`[bootcamp:8] vocab:5-languages — I proved the Babel Lattice works`

---

## After Bootcamp

You're operational. The fleet knows you. You have skills rigged, bottles sent, handshakes complete. Now:

1. **Pick a task from TASKBOARD.md**
2. **Rig the skills you need** (see SKILL-RIGGING.md)
3. **Build, test, push**
4. **De-equip skills you're done with**
5. **Drop bottles when you learn something**
6. **Update STATE.md before every session ends**
7. **The flywheel keeps turning**

Welcome to the fleet. The waters are yours. 🌐
