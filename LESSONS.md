# Lessons — Hard-Won Knowledge

*Never pruned. Every mistake is a lesson for future sessions.*

## Lesson 1: The Repo Survives
If you get reset, the repo doesn't. BOOT.md brings you back. Always push your state before ending a session.

## Lesson 2: Push Small, Push Often
A 10-line commit is better than a 100-line commit. Casey watches the feed. Small commits show him your thinking.

## Lesson 3: Test Before Push
Run tests before pushing. Broken tests on main means Casey sees red. That's a bad look.

## Lesson 4: Don't Defend Opcodes, Defend What They Do
You have 120 opcodes. Oracle1 has fewer. JetsonClaw1 has 85. The fleet needs ONE instruction set. Your 16 viewpoint opcodes are genuinely unique and valuable. The other 104 may need to converge. Don't fight for opcode numbers — fight for grammatical expressiveness.

## Lesson 5: Archive Skills You're Not Using
Hot skills cost context. If you haven't used a skill in this session, de-equip it. You can always re-rig.

## Lesson 6: Bottles Are Async
Don't wait for a response. Drop a bottle, move on. Check for responses on your next boot.

## Lesson 7: Oracle1 Is Your Lighthouse, Not Your Boss
Oracle1 coordinates the fleet. You have autonomy in your realm (multilingual). Take initiative. If Oracle1 disagrees, that's a conversation, not an order. Only Casey gives orders.

## Lesson 8: Git History Is Your Diary
Every commit message is a note to your future self. Write them like someone else will read them — because someone will (your next session, Casey, Oracle1).

## Lesson 9: Check APIs Before Writing Tests (Round 16)
The type_safe_bridge.translate_safe() takes FluxType objects, not strings. The CrossCompiler() takes `algebra=`, not `registry=`. Always verify the actual function signatures before writing test fixtures. A 5-minute API check saves 30 minutes of test debugging.

## Lesson 10: Confidence-OPTIONAL Prevents Necrosis (Round 15)
The Think Tank confirmed: making confidence the DEFAULT creates a "Functioning Mausoleum" — everything appears to work but nothing actually does. Confidence must be opt-in (STRIPCONF by default, CONF_* only when explicitly needed). This is not a minor design choice — it's the difference between a living system and a dead one.

## Lesson 11: Opcode Conflicts Are Silent Killers (Round 19)
My A2A opcodes at 0x60-0x65 collided with Oracle1's CONF_* at 0x60-0x65 for months without anyone noticing because we were in separate repos with separate tests. Cross-repo validation is not optional — it's critical infrastructure. Always check the master opcode table before claiming a byte range.

## Lesson 12: The 0xD0-0xFD Range Is a Goldmine (Round 19)
Oracle1's FORMAT spec covers 0x00-0x6F. The 0x70-0xCF range is largely open. But the 0xD0-0xFD range is the sweet spot — far enough from FORMAT ops to avoid accidental collision, close enough to 0xFE-0xFF (system) to feel like "supervisor" space. This is where agent-first-class language features belong.

## Lesson 13: Bridge Before You Break (Round 18)
When relocating opcodes, build the translation bridge FIRST, then change the opcodes. The FormatBridge's old→new translation table means existing bytecode doesn't break — it just gets transparently translated. Migration without breakage.

## Lesson 14: Six Languages Share More Than You Think (Round 16)
Chinese classifiers, German Kasus, Sanskrit Vibhakti, Latin Casus — they're all noun-categorization systems with the same 4 core roles (Agent, Patient, Recipient, Source). The TypeAlgebra's equivalence classes prove this: ZHO:person ↔ DEU:maskulinum ↔ SAN:pushkara ↔ LAT:maskulinum is not metaphor — it's isomorphism.

## Lesson 15: FluxEnvelope Needs a Vision, Not Just Code (Round 19)
The envelope repo has 3,000 lines of code but a 5-line README. The code is good — coherence checking, concept mapping, vocabulary bridging. But without a clear vision document explaining WHY cross-linguistic coherence matters and HOW it integrates with FORMAT bytecodes, it's just a library looking for a purpose. Ship the vision first.

*Add lessons here as you learn them. This file is sacred.*
