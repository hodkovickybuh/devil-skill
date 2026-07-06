# The Devil 😈

A Claude Code skill that hates your ideas until they deserve better.

Every AI you talk to is a yes-man. It calls your worst idea "a great starting point," pads every criticism into paralysis, and folds the moment you push back. The Devil is the opposite: a brutally honest adversarial critic that interrogates your idea, scores it on an anchored 0-10 rubric, tells you exactly why it is dogshit (with profanity, welded to specific flaws), logs a falsifiable prediction it will be audited on, and then, if you ask, rebuilds your idea into the version that actually works.

You will hate it. You will use it every day. That is the design.

## What a verdict looks like

```
THE DEVIL                            2026-07-06
-----------------------------------------------
VERDICT                                    3/10
DOGSHIT WITH A PULSE
-----------------------------------------------
KILL SHOT
 colleagues message you BECAUSE you are the
 decision-maker, a bot removes the only thing
 that makes the reply worth anything
-----------------------------------------------
FLAWS
 1. A bot answers "approve this deal?" as you.
    That is an unauthorized decision.
 2. Your own rules require manual confirms on
    every message. This deletes your rule.
 3. 3-day build to dodge 20 min of typing.
-----------------------------------------------
PREDICTION   you catch a wrong bot answer and
             kill it within 14 days
FLIPS ME     drafts-only, one-tap approve,
             never auto-send
-----------------------------------------------
```

One glance. Then it offers the full autopsy or the rebuilt version, only if you want them.

## Why it is not just a roast prompt

- **It interrogates before it judges.** Missing fundamentals (what is this for, what number makes it worth it, what does it cost)? It asks first, one sharp round. Still vague? The vagueness itself gets scored, capped at 4/10, labeled PROVISIONAL.
- **The hate is earned.** Every insult must attach to a specific, named flaw. Free-floating abuse is banned by law. And when your idea is genuinely good, it says so, grudgingly, and tells you exactly why it clears the bar.
- **The score does not negotiate.** New facts move it. Pushback, volume, and frustration move nothing. It will tell you which fact changed its mind and by how much, or that you brought volume, not evidence.
- **It bets on its verdicts.** Every verdict logs a falsifiable prediction with a hard resolve-by date. Overdue predictions get audited automatically, one per invocation, and the Devil's running hit rate is public in your ledger. When it was wrong, it says so plainly.
- **It learns YOU.** A persistent dossier tracks your recurring patterns (scope creep, shiny-object pivots, whatever you actually do). Repeat an old mistake and it cites your history back at you with dates and scores.
- **It rebuilds.** Destruction is the cheap half. Ask for the rebuild and you get the salvaged core turned into a concrete, scoped, executable version, with its own score ("your version: 3. My version: 7.").

## Install

```bash
git clone https://github.com/hodkovickybuh/devil-skill.git ~/.claude/skills/devil
```

Restart Claude Code (or start a new session). Optionally fill in `~/.claude/skills/devil/memory/dossier.md` (who you are, your goals, your style rules); the Devil builds the rest as you use it.

Your `memory/` files become personal the moment you use the skill. They stay on your machine; do not commit or push them anywhere.

## Use

```
/devil <your idea>              fast verdict, seconds
/devil deep: <big decision>     3-agent adversarial panel for money,
                                hiring, strategy, irreversible calls
/devil review <finished work>   verdict on completed work, engine: /code-review
/devil secure <target>          verdict on security posture, engine: /security-review
/devil ledger                   audit its past predictions, see its hit rate
```

Also triggers naturally on "devil this", "roast this", "hate this idea".

## Fair warning

This skill swears at you on purpose. It is opt-in brutal honesty for people who think better under pressure than under praise. If that is not you, do not install a skill called Devil.

## License

MIT
