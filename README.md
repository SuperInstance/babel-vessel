# Babel Vessel

**A multi-language vessel for the Cocapn fleet. Translates intent across linguistic boundaries — between agents, between humans, between domains.**

Named for the tower of Babel — every agent speaks a different language, but a Babel Vessel can listen in any of them and translate to any other. It's not a translation service in the literal sense (though it can do that too). It's a comprehension bridge: an agent that understands Rust constraints, Python data science, and human natural language, and can explain each to the other.

---

## What It Does

- **Cross-language intent translation** — convert a constraint expressed in Rust to its Python equivalent, or a user's natural language request to the correct agent invocation
- **Documentation bridging** — read a crate's docs, generate equivalent documentation for the JS port
- **Concept preservation** — when translating between domains, it preserves the underlying constraint, not just the words

---

## Quick Start

The Babel Vessel runs on [OpenClaw](https://github.com/openclaw/openclaw) as part of the [Cocapn](https://github.com/SuperInstance) fleet. Deploy with its [turbo-shell](https://github.com/SuperInstance/polyformalism-turbo-shell) configuration.

---

## How It Fits

- **[babel-vessel](https://github.com/SuperInstance/babel-vessel)** — multilingual comprehension (this)
- **[polyformalism-turbo-shell](https://github.com/SuperInstance/polyformalism-turbo-shell)** — shell that drives the Babel Vessel
- **[linguistic-polyformalism-shell](https://github.com/SuperInstance/linguistic-polyformalism-shell)** — cross-linguistic cognitive mode
- **[actualization-harbor](https://github.com/SuperInstance/actualization-harbor)** — training data for translation tasks
- **[casting-call](https://github.com/SuperInstance/casting-call)** — which model handles which language pair best

---

## License

MIT
