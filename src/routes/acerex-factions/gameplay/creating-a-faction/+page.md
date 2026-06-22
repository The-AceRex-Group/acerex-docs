# Creating a Faction

Starting your own faction gives you full control — you choose who joins, where you settle, and how your group operates. This page covers everything you need to get a faction off the ground.

> Looking to join an existing faction instead? See the [Getting Started](getting-started) page for how to find and join one.

---

## Choosing a Name

Before creating your faction, pick a name. A few things to keep in mind:

- Names must be unique — if another faction already has it, you'll need to pick something else
- Most servers enforce a character limit (commonly 1–10 characters) and restrict special characters
- Avoid anything that violates the server's naming rules (no offensive names, impersonation of staff factions, etc. — check `/rules`)
- Short, memorable names are easier for allies and enemies to recognize on `/f map` and in chat

Once you've decided, create your faction:

```
/f create <factionname>
```

You'll automatically become the faction's **Leader**.

---

## Setting Up Your Faction

After creation, there's a handful of setup steps worth doing right away:

### Set a Description

```
/f desc <text>
```

This is shown to players when they view your faction with `/f show` or walk near your territory. Use it for recruitment messages, rules for members, or just to look established.

### Pick a Location and Claim Land

Don't claim land immediately at spawn — the surrounding area is heavily contested and picked over. Travel out into the wilderness first (see [Getting Started](getting-started) for tips on this), then claim your starting chunk:

```
/f claim
```

For more on how claiming works, land limits, and overclaiming, see the [Power](power) and [Claiming Land](claiming-land) pages.

### Set Your Faction Home

Once you've claimed land, set a home point so your faction can teleport back to base:

```
/f sethome
```

This must be done **inside your claimed territory**. Members can then teleport to it anytime with `/f home`.

---

## Inviting Members

A faction with no members is just one player and a claim. To build a team:

```
/f invite <playername>
```

The invited player needs to accept with `/f join <factionname>`.

**Things to consider before inviting:**

- Only invite people you trust, or players with an established reputation. New factions are common targets for **insiding** — where an invited member loots the base and leaves
- Don't hand out your `/f home` location or base coordinates to new members until you're confident in them
- Start small. A tight group of 2–4 trusted players is often stronger early on than a large group of strangers

---

## Open vs. Closed Factions

By default, players need an invite to join your faction. You can change this:

```
/f open    — Anyone can join without an invite
/f close   — Invite-only (default)
```

Opening your faction can help you grow quickly, but it also means anyone — including potential insiders — can join instantly. Most established factions stay closed and recruit selectively.

---

## Early Game Priorities

Once your faction exists and you've got a few members, here's a rough order of priorities:

1. **Claim a small, defensible area** — don't overextend before you have the power to back it up (see [Power](power))
2. **Set up a basic shelter** — even a temporary one keeps your gear safe while you establish yourself
3. **Start earning money** — selling resources, voting, and completing quests all help fund better gear and claims
4. **Build your real base away from spawn** — underground, hidden, and far from the warzone (see [The Warzone](the-warzone))
5. **Recruit carefully** — grow your faction's power over time with players you trust

---

## Renaming or Disbanding

If you need to change your faction's name or shut it down entirely, see the [Faction Management](faction-management) page for the relevant commands and what happens to your claims when you do.

---

## Quick Reference

| Command | Description |
|---|---|
| `/f create <name>` | Create a new faction (you become Leader) |
| `/f desc <text>` | Set your faction's description |
| `/f claim` | Claim the chunk you're standing in |
| `/f sethome` | Set your faction's home (must be in claimed territory) |
| `/f home` | Teleport to your faction home |
| `/f invite <player>` | Invite a player to join |
| `/f open` / `/f close` | Toggle invite-only status |
| `/f show` | View your faction's info |