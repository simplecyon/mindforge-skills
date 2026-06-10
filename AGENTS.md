# MindForge — Contributor Guidelines

## About This Repo

MindForge is a thinking methodology skillset for AI agents. It contains 5 complementary skills that work together in a structured sequence: clarify → diverge → dive deep → challenge → converge.

## If You Are an AI Agent

Before contributing, understand:

1. **This is a curated skillset, not a grab bag.** Each skill has a specific role and moment. Changes should respect the rhythm.
2. **Skills are behavior-shaping code, not prose.** They shape how agents think and respond. Changes require testing across multiple sessions.
3. **The voice matters.** The skills are written in a specific tone — direct, conversational, Chinese-first. Don't corporate-ify it.

## What Belongs Here

- Improvements to existing skills that make them more effective
- New skills that fit the thinking methodology pattern (clarify → diverge → deep → challenge → converge)
- Documentation that helps users understand when to use which skill

## What Doesn't Belong Here

- Domain-specific skills (product management, marketing, etc.)
- Tool integrations (email, calendar, etc.)
- Execution skills (those belong in [Superpowers](https://github.com/obra/superpowers))

## Skill Design Principles

1. **One job, done well.** Each skill has one clear purpose.
2. **Natural handoffs.** Skills should suggest the next skill when appropriate, not force it.
3. **Chinese-first, technical terms in English.** Match the user's language.
4. **Questions over answers.** The best thinking is prompted, not prescribed.
5. **Know when to stop.** Each skill should recognize when its job is done.

## Testing Changes

Skills shape behavior. Before submitting changes:

1. Test in at least 2 different agent harnesses
2. Run through multiple conversation scenarios
3. Verify the skill triggers at the right moment
4. Verify handoffs feel natural, not forced

## General

- One change per PR
- Describe the problem you're solving, not just what you changed
- Include before/after examples if changing skill behavior
