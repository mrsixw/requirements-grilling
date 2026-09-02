---
name: requirements-grilling
description: Interview the user about a plan, design, or feature until the important decisions, constraints, and success criteria are explicit.
---

# Requirements grilling

Produce an implementable decision record before substantial work begins. The
purpose is to remove consequential ambiguity, not to prolong discovery.

## Establish what is already known

Inspect the repository, supplied documents, and current tool state before asking
questions they can answer. State the desired outcome, then separate:

- observed facts and their sources;
- user decisions and preferences;
- hard constraints;
- working assumptions; and
- unresolved choices that would change the implementation.

Do not present an inference as an agreed requirement.

## Resolve the important choices

Ask one small batch at a time, starting with the choice that has the largest
effect on scope, safety, or user-visible behaviour. For each material choice:

1. Explain what is unknown and why it matters.
2. Give a recommendation when the evidence supports one.
3. State the trade-off in concrete terms.
4. Test ambiguous language with an example, boundary case, or counterexample.
5. Record the answer before moving on.

Avoid asking the user to choose implementation detail that the repository's
conventions already settle.

## Completion contract

Finish with the agreed goal, audience, in-scope behaviour, non-goals,
constraints, acceptance criteria, risks, decisions, and remaining assumptions.
Call out any blocker that still requires authority or information. Stop when a
different implementer could proceed without inventing product behaviour.

If durable project terminology or architecture decisions emerged, offer
`domain-context`. Do not create tickets, edit external systems, or send messages
unless the user separately authorises that work.
