<!-- slopstopper · coherent doesn't mean correct -->

# slopstopper

Coherent doesn't mean it's correct.
Saying it's completed doesn't always mean it's been checked.
Confidence doesn't mean it has provenance.
It looks like it works — but does it have the right effect?

**Slop**: output that's fluent, plausible, and confident — and unmoored from
anything that checked it. Not wrongness; wrongness is cheap to catch.
Coherence without provenance: text that sounds finished, numbers that look
measured, plans that read as decided, produced at zero marginal cost by tools
paid to sound sure.

Coherence used to be a signal. If a document held together, someone had
probably thought about it. Generative tools broke that — holding together is
now the default texture of everything, including nonsense.

slopstopper is a workshop of instruments against it, enforced by machines,
not vibes. Each works alone.

```
/plugin marketplace add slopstopper/marketplace
```

## The bench

Trued and in use:

| instrument | measures | in one line |
|---|---|---|
| [**plumb-line**](https://github.com/slopstopper/plumb-line) | whether claims are honest | provenance primitives (JS + Python) plus skills that audit for laundered uncertainty — and refuse to launder it back out during the fix. |
| [**tokenomics**](https://github.com/slopstopper/tokenomics) | which model should do the work | route work to the cheapest capable tier, name your own lanes (no defaults shipped), carry strategy across sessions in a playbook that stays method, not ledger. |
| [**recursive-spine**](https://github.com/slopstopper/recursive-spine) | where tracked state lives | GitHub issues + milestones as the only home of work state; skills to teach, stamp, migrate, and digest it. Its own tracker existed before its first commit. |

Three seams, deliberately disjoint: honesty of claims, economics of effort,
location of state. Where they meet, the vocabulary is pinned in the
[shared marketplace](https://github.com/slopstopper/marketplace) so the same
word can't mean three things.

The bench is meant to fill.

## The calibration

The spec every instrument here is trued against:

- **Record first, compare after.** Interpretation is a privilege the data
  has to earn.
- **"We don't know yet" is a shippable answer.** A null result is a
  first-class outcome, not a failure to be padded over.
- **Every claim carries its provenance, or it's a rumour.** Mock, derived,
  measured, asserted — the label travels with the value.
- **State lives where it's queryable, not where it merges.**
- **Deferral requires a record.** Aging must be measurable or the deferral
  didn't happen.
- **Honest denominators.** A report says what it didn't read. A sweep that
  exempts itself is lying about its coverage.
- **Boundaries checked by tooling.** Discipline that depends on remembering
  is a bug that hasn't fired yet.

## Applied to itself

plumb-line's audit skill was run against plumb-line and produced a
remediation plan it then had to survive. recursive-spine's issues and
milestones existed before its first commit, its labels were stamped by its
own bootstrap, and its own deferrals age on its own digest. The rule of the
house: if a discipline is too heavy to follow while building the tool that
states it, the discipline is wrong — fix the rule, not the record.

## The risk register

What goes wrong when fluent tools meet real work:

| Risk | How it arrives |
|---|---|
| **Laundered uncertainty** | A mock value becomes a number, the number becomes a dashboard, the dashboard becomes a decision. Nobody lied; the confidence label just fell off in transit. |
| **Self-graded homework** | The system that produced the claim is the system that assures you it's fine. It is very reassuring. That is the problem. |
| **Prose-ledger rot** | Work state kept in documents merges as text, loses rows silently, and drifts from reality the day it's written. The doc stays confident throughout. |
| **Silent deferral** | "Later" without a record isn't a plan, it's a deletion with a delay. |
| **Economics slop** | The expensive model doing work the cheap one could — or the cheap one doing work it can't, which costs more, twice. |
| **Overstated maturity** | Everything is "production-ready" now. Including this table, if we're not careful. |

## Install

```
/plugin marketplace add slopstopper/marketplace
```

then `/plugin install` the instruments you want. Each works alone; none
requires its siblings — they offer, never demand.

## Status

Extracted from live practice in a small number of real projects. Practice
reports, not benchmarks. We would love to tell you these tools are
battle-tested; our own CI fails any README containing that phrase.

None of this stops you from shipping slop. It makes it visible,
attributable, and slightly embarrassing.
