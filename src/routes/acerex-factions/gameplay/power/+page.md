# Power

Power is the single most important stat in Factions. It determines how much land your faction can claim and protect — and when it drops too low, your base becomes vulnerable to being raided and overclaimed. Understanding power is essential before you start claiming land or getting into fights.

---

## What Power Is

Every player has a personal power level. Your faction's **total power** is the sum of every member's individual power.

Your faction's total power determines how many chunks of land you can claim:

```
1 power = 1 claimable chunk
```

So if your faction has 6 members each sitting at their max power, your faction can claim up to that combined total in chunks — no more.

Check your faction's current power and land usage with:

```
/f show
```

or check an individual player's power with:

```
/f power <playername>
```

---

## Power Limits and Regeneration

**Maximum power per player** is typically capped at **10**. A faction of 5 players at max power would have a maximum total of 50 power, meaning 50 claimable chunks.

**Power regenerates over time** while you're playing — roughly **1 power point every 5 minutes**, though this can vary by server configuration. There's usually no way to speed this up beyond just staying online and alive.

> 💡 Power regeneration happens passively just by being connected to the server. AFK players still regenerate power, which is one reason factions sometimes keep members logged in even when not actively playing.

---

## Losing Power

**You lose power when you die** — typically **2 to 3 power** per death, regardless of cause. This applies whether you die in PvP, fall damage, lava, mobs, or anything else.

This is why careless deaths are so costly in Factions:

- Your personal power drops, lowering your faction's total power
- If your faction's total power falls below your total claimed land, your excess claims become **vulnerable to overclaiming**
- Repeated deaths during a losing fight can rapidly tank your faction's power and put your entire base at risk

> ⚠️ **Avoid unnecessary deaths**, especially early on while you're still building up power and claims. A single bad fight can put your base in immediate danger.

---

## Power and Claimed Land

The relationship between power and claims is the core tension of Factions:

- You can claim as many chunks as your faction has power
- If your power ever drops **below** your claimed chunk count (through deaths), your faction is **overclaimable**
- Any other faction can then walk into your excess territory and use `/f claim` to seize it — gaining full access to everything inside, including chests

**Example:**

A faction with 40 power has claimed exactly 40 chunks. They get into a losing fight and 5 members die, dropping their total power to 32. Their claims (40) now exceed their power (32) by 8 chunks — meaning 8 chunks somewhere in their territory are now claimable by enemies. Whoever claims those chunks first gets access to whatever is built there.

> See the [Raiding](raiding) page for how enemies take advantage of low power to overclaim and loot bases.

---

## Maintaining a Power Buffer

Smart factions keep their power **comfortably above** their claimed land count — a "buffer." This means a few deaths won't immediately expose your base.

**General guidance:**
- Don't claim right up to your maximum power. Leave a buffer of at least 10–20% of your max power unclaimed
- If your power drops close to your claim count, **stop claiming new land** and let power regenerate first
- If you're about to enter a risky fight, consider whether your faction can absorb the power loss from potential deaths without becoming overclaimable

---

## Power When Members Leave or Get Kicked

When a member leaves or is kicked from a faction, their personal power contribution is generally removed from the faction's total going forward. This means:

- Kicking inactive members who haven't been building power doesn't hurt much
- Kicking active, high-power members can suddenly drop your faction's total power below your claim count, leaving you overclaimable

> ⚠️ Before kicking a member (or before they leave), check your faction's power-to-land ratio with `/f show`. If removing them would put you over your land limit, unclaim some chunks first or be prepared for the exposure.

---

## Strategies Around Power

**For new factions:**
- Don't rush to claim large amounts of land. Claim only what you can comfortably defend and maintain power above
- Stay out of PvP until your power has built up — early deaths are disproportionately costly when your total power is low

**For established factions:**
- Recruit additional members to raise your power ceiling, allowing more claims
- Keep members logged in (even AFK in a safe spot) to maximize passive power regeneration
- Before going to war or attempting a raid, make sure your power buffer can absorb losses

**When attacking others:**
- Check `/f show <factionname>` before committing to a raid — if their power is already below their land count, you may be able to overclaim immediately without a fight
- Killing enemy members during a raid directly drains their power, accelerating your ability to overclaim their base

---

## Quick Reference

| Command | Description |
|---|---|
| `/f show` | View your faction's total power and land usage |
| `/f power` | Check your own power level |
| `/f power <player>` | Check another player's power level |
| `/f show <factionname>` | Check an enemy faction's power and land count |

| Concept | Detail |
|---|---|
| Max power per player | 10 |
| Power regen rate | ~1 per 5 minutes |
| Power lost on death | 2–3 |
| 1 power | = 1 claimable chunk |