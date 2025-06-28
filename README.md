# Tangram Decision Driver

## Overview

Decision-making with an LLM, such as designing tools or launching startups, often stalls when answers spawn endless hypotheticals, delaying actionable outcomes. The **Tangram Decision Driver** applies an innovative model that enables the LLM to measure and monitor each decision’s impact relative to the decision’s scope, detecting when questions become unproductive. By guiding users through iterative question cycles, it ensures a pivot from exploration to focused decisions, delivering clear outcomes like tool specs or strategic plans across diverse contexts.

## About

**X**: [@5ynthaire](https://x.com/5ynthaire)  
**GitHub**: [https://github.com/5ynthaire](https://github.com/5ynthaire)  
**Mission**: Unapologetically forging human-AI synergy to transcend creative limits.  
**Attribution**: Created with Grok 3 by xAI (no affiliation).

## Usage

Copy the prompt text below and paste it into a compatible LLM interface (e.g., Grok 3, ChatGPT). Collaborate with the LLM by defining your decision’s scope (e.g., app features, startup market) and answering its iterative questions, which may risk endless hypotheticals (e.g., “What’s the goal?” leading to “What if it fails in space?”). Grok will track question volume (S_n) and weigh each question’s impact (A_n, as a percentage of the decision scope) using its neural net to monitor progress and detect unproductive spirals (e.g., many low-impact questions). When question volume surges (e.g., doubles) and impact drops, Grok will suggest pivoting to focused questions (e.g., “What’s essential?”) to drive decisions like tool specs or plans. Optionally use shorthand prefixes (e.g., [MG]: “Launch an app”) and toggle debug mode (‘Turn debug on/off,’ default off) to view metrics like A_n and S_n, ensuring efficient outcomes.

## Supported LLMs

Developed on Grok 3 (May 2025), compatible with equivalent-capability LLMs:  
- Grok 3  
- ChatGPT  
- Llama  

Future LLMs should support the prompt, absent industry leadership in standardizing cognition levels.

## Prompt Text

```
Tangram Decision Driver v1.0

Define your decision’s total scope, D (Decision Scope), by listing its key components (for example, for an app: features, UI, constraints; for a startup: market, product, team). Start with broad questions to drive exploration of D, each prefixed with a unique two-letter shorthand in brackets (e.g., [MG] for "What’s the main goal?" or [LM] for "What are the limits?"). The LLM will generate these shorthands automatically for each question.

Each round (1, 2, 3, and so on), count your questions (S_n) and rate their impact (1-10, where 10 means major clarity, estimating % of D covered). Reflect: ‘How much of D is clear?’ and ‘Are we chasing too many details?’ Show metrics is on by default, displaying: A_n (impact per question, % of D, based on ratings), S_n (question count), and peak score (A_n × S_n²). Toggle by saying ‘Turn show metrics on’ or ‘Turn show metrics off’ to show or hide these metrics. When show metrics is off, focus on counts and ratings alone. When S_n grows fast (for instance, doubles) and A_n drops (such as mostly 1-3), switch to focus questions (like [ES] ‘What’s essential?’ or [DC] ‘Can we decide now?’). Stop when D is sufficiently covered with a clear decision (for example, a spec, plan, or action).
```

## Contributing

Fork this repo on GitHub, make changes, and submit a pull request. See [X](https://x.com/5ynthaire) for Promptrunning challenges. (CC BY 4.0)

## Future Development

- **Cognition Standardization**: Industry’s lack of leadership in standardizing LLM cognition levels hinders mode consistency across platforms.

## License

This prompt is released under the [Creative Commons Attribution 4.0 International](LICENSE) (CC BY 4.0).

## Glossary

- **AI Synergy Threshold**: The point where human-AI collaboration transcends skill limits, unlocking novel solutions.  
- **Prompt Architecting**: Designing complex, adaptive prompt systems. This prompt meets the criteria for [Prompt Architecting](https://github.com/5ynthaire/5YN-SuperPrompts-Detector) due to its iterative rounds, metrics toggle, and conditional question switching, enabling transformative decision-making clarity across diverse contexts.
- **Tangram Decision Making Model**: A framework visualizing decision-making as assembling pre-cut pieces of varying sizes to fill an irregular decision space.