<!-- slopstopper · coherent doesn't mean correct · mirrors https://slopstopper.org -->

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/slopstopper/.github/main/profile/assets/logo-word-light.png">
  <img alt="slopstopper" src="https://raw.githubusercontent.com/slopstopper/.github/main/profile/assets/logo-word-ink.png" width="380">
</picture>

> *Coherent doesn't mean it's correct.*<br>
> *Saying it's completed doesn't always mean it's been checked.*<br>
> *Confidence doesn't mean it has provenance.*<br>
> *It looks like it works — but does it have the right effect?*

slopstopper is a set of tools for checking what generative systems produce.
Each works on its own; together they work as one system.

```
/plugin marketplace add slopstopper/marketplace
```

**[slopstopper.org →](https://slopstopper.org)**

## The problem

**Slop used to be obvious.** It has not disappeared, it just got better at
disguising itself. You can no longer tell just by looking at something what
parts have been checked and what parts got filled in with an articulate
guess. It all reads the same regardless.

Now with generative tools anything can look coherent, polished and confident
while remaining completely untethered to reality.

## What slop do they stop?

One tool for each.

| | tool | stops | how |
|---|---|---|---|
| 01 / honesty | [**plumb-line**](https://slopstopper.org/plumb-line/) | **a guess used as if it were measured** | A mock value ends up in a dashboard, then a decision, and nothing along the way marks it as a guess. plumb-line labels each value with where it came from and keeps the label attached through every derivation, and its review-time checks catch the places where that already went wrong. |
| 02 / economics | [**tokenomics**](https://github.com/slopstopper/tokenomics) | **the wrong model doing the work** | An expensive model running work a cheap one could do, or a cheap one running work it can't and having to redo it. tokenomics routes work to the cheapest tier that can actually do it, in lanes you name, and a living playbook carries what you worked out into the next session. |
| 03 / state | [**recursive-spine**](https://github.com/slopstopper/recursive-spine) | **a record that drifts from reality** | Work tracked in a document drifts almost immediately, and a "later" that isn't written down doesn't happen. recursive-spine keeps work state in GitHub issues and milestones, where it stays queryable, and ages deferrals so they surface before they rot. |

Put tokenomics and recursive-spine together and the routing is logged in
issues and milestones instead of sitting in a playbook. The shared vocabulary
is pinned in the
[marketplace](https://github.com/slopstopper/marketplace/blob/main/docs/shared-vocabulary.md):
one owner per term.

## Applied to itself

**Every tool is run on itself.** None of these ask of you a standard they
don't meet. Each is turned on its own repository and has to survive the
result.

- ↺ **plumb-line** — its auditor runs on its own code before every release,
  and the dogfood report keeps what it finds.
- ↺ **tokenomics** — it runs on its own build: a dogfooded playbook and a
  spend ledger that makes its savings claims checkable.
- ↺ **recursive-spine** — its issues and milestones existed before its first
  commit, and its deferrals age on its own digest.

If we cannot follow a rule while building the tool that asks you to follow
it, the rule has failed its own test and we rewrite it. The record of where
it broke stays, because editing it afterwards would be the failure this is
meant to catch.

## Install

From inside Claude Code:

```
/plugin marketplace add slopstopper/marketplace
/plugin install plumb-line@slopstopper
/plugin install tokenomics@slopstopper
/plugin install recursive-spine@slopstopper
```

Prefer to read first? Start with the
[plumb-line page](https://slopstopper.org/plumb-line/).

## Status, honestly

None of this stops you from shipping slop. It just makes it visible,
attributable, and slightly embarrassing.
