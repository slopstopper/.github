<!-- slopstopper · coherent doesn't mean correct -->

# slopstopper

```
coherent    ≠  correct
completed   ≠  checked
confident   ≠  provenance
works       ≠  right effect
```

Coherent doesn't mean it's correct.
Saying it's completed doesn't always mean it's been checked.
Confidence doesn't mean it has provenance.
It looks like it works — but does it have the right effect?

**Slop**: fluent, plausible, confident output, unmoored from anything that
checked it. Coherence without provenance: sounds finished, looks measured,
reads as decided.

Coherence used to be a signal. If a document held together, someone had
probably thought about it. Generative tools broke that. Now everything holds
together, including nonsense.

slopstopper is a set of tools that catch slop in code. Each works alone.

```
/plugin marketplace add slopstopper/marketplace
```

## The tools

In use:

| tool | measures | in one line |
|---|---|---|
| [**plumb-line**](https://github.com/slopstopper/plumb-line) | whether claims are honest | provenance primitives (JS + Python) plus skills that audit for laundered uncertainty, and refuse to launder it back out during the fix. |
| [**tokenomics**](https://github.com/slopstopper/tokenomics) | which model should do the work | route work to the cheapest capable tier, name your own lanes (no defaults shipped), carry strategy across sessions in a playbook of reusable method. |
| [**recursive-spine**](https://github.com/slopstopper/recursive-spine) | where tracked state lives | GitHub issues + milestones as the only home of work state; skills to teach, stamp, migrate, and digest it. Its own tracker existed before its first commit. |

Three concerns that don't overlap: honesty of claims, economics of effort,
location of state. Shared vocabulary is pinned in the
[marketplace](https://github.com/slopstopper/marketplace) so one word can't
mean three things.

More will follow.

## The rules

What every tool here is held to:

- **Record first, compare after.** Interpretation is a privilege the data
  has to earn.
- **"We don't know yet" is a shippable answer.** A null result is a
  first-class outcome.
- **Every claim carries its provenance, or it's a rumour.** Mock, derived,
  measured, asserted: the label travels with the value.
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
own bootstrap, and its own deferrals age on its own digest. If a discipline
is too heavy to follow while building the tool that states it, the discipline
is wrong. Change the rule and leave the record alone.

## What goes wrong

When fluent tools meet real work:

| Risk | How it arrives |
|---|---|
| **Laundered uncertainty** | A mock value gets used as if it were measured. It ends up in a dashboard, then a decision, and nothing along the way marks it as a guess. |
| **Self-graded homework** | The tool that made the claim is the same tool that checks it. |
| **Prose-ledger rot** | Work tracked in a document drifts from reality almost immediately. Merges drop rows and the file still reads fine. |
| **Silent deferral** | A "later" that isn't written down anywhere usually just doesn't happen. |
| **Economics slop** | An expensive model running work a cheap one could do, or a cheap one running work it can't and having to redo it. |
| **Overstated maturity** | Everything gets called "production-ready," including things that aren't. |

## Install

```
/plugin marketplace add slopstopper/marketplace
```

then `/plugin install` the tools you want. Each works alone; none needs its
siblings.

## Status

From live practice in a few real projects, written up as practice reports.
We would love to tell you these tools are battle-tested; our own CI fails any
README containing that phrase.

None of this stops you from shipping slop. It makes it visible, attributable,
and slightly embarrassing.
