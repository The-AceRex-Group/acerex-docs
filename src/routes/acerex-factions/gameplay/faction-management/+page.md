# Faction Management

Once your faction is up and running, you'll need to manage its members, ranks, and settings. This page covers ranks and permissions, member management, renaming, and disbanding.

---

## Ranks

Factions typically have a rank hierarchy that determines what each member can do.

| Rank | Typical Permissions |
|---|---|
| **Leader** | Full control — invite, kick, promote/demote, claim, unclaim, disband, set relations, manage faction bank |
| **Officer** | Can usually invite and kick members, claim/unclaim land, and manage some settings — but cannot disband the faction or demote the Leader |
| **Member** | Can claim land (if permitted), access faction chat, and use faction home — but cannot manage other members |
| **Recruit** | Newly joined members on some servers — limited permissions until promoted |

> ⚠️ **Verify on your server:** Exact rank names and what each rank can do may differ. Use `/f help` in-game for the precise permission breakdown on AceRex.

---

## Promoting and Demoting Members

The Leader (and often Officers, depending on settings) can adjust member ranks:

```
/f promote <playername>   — Move a member up one rank
/f demote <playername>    — Move a member down one rank
```

Promote members you trust to Officer so they can help manage the faction while you're offline — inviting new members, organizing claims, or handling day-to-day faction chat.

---

## Kicking and Removing Members

```
/f kick <playername>
```

Removes a player from the faction immediately. They lose access to faction chat, faction home, and any build permissions tied to membership.

**When to kick someone:**
- Inactivity — dead weight members reduce your average power efficiency and clutter your roster
- Suspected insider activity — if someone's behavior seems off, it's safer to remove them before they act
- Conflict within the faction that can't be resolved

> 💡 Kicking a member does **not** remove their personal power contribution retroactively in most setups — but going forward, your faction's total power will reflect your remaining members. See the [Power](power) page for details.

---

## Leaving a Faction

If you want to leave on your own:

```
/f leave
```

If you're the Leader, you typically can't leave until leadership is transferred to someone else (see below) or the faction is disbanded.

---

## Transferring Leadership

Before stepping down or going inactive long-term, transfer leadership to a trusted member:

```
/f leader <playername>
```

This hands full Leader permissions to the chosen player. Once transferred, your own rank drops to Officer (or whatever rank the server assigns to former leaders). Only do this for someone you fully trust — the new Leader has total control, including the ability to disband the faction or kick everyone else.

---

## Renaming Your Faction

```
/f rename <newname>
```

Same naming rules apply as when creating a faction — the new name must be unique and follow the server's naming restrictions. Your claims, power, and members carry over; only the name changes.

---

## Faction Description and Titles

```
/f desc <text>      — Set your faction's description (shown on /f show)
/f title <text>     — Set a personal title shown next to your name (if supported)
```

Use these for recruitment, branding, or just to add some personality to your faction's profile.

---

## Faction Chat

```
/f chat       — Toggle faction-only chat
/f chat a     — Switch to ally chat (visible to allies too)
/f chat p     — Switch back to public chat
```

Faction chat is useful for coordinating without enemies seeing your plans in public chat — especially important when discussing raids, defenses, or base locations.

---

## Permissions (`/f perm`)

Some servers allow fine-grained control over what each rank can do — claiming, unclaiming, inviting, kicking, accessing the faction bank, and more.

```
/f perm
```

Opens (or lists) the permission settings for your faction, depending on server setup. Use this to restrict sensitive actions — like unclaiming land or withdrawing from the faction bank — to Officers and the Leader only, reducing the damage a compromised or rogue member can do.

---

## Disbanding a Faction

If your faction is done — merging with another, splitting up, or simply ending — the Leader can disband it entirely:

```
/f disband
```

**What happens when you disband:**
- All claimed land is immediately unclaimed and becomes available to anyone
- All members are removed from the faction
- Any faction bank balance is typically lost — withdraw everything first
- The faction name may become available for others to use

> ⚠️ Disbanding is permanent. Make sure every member has retrieved their belongings and the faction bank has been emptied before you do this.

---

## Quick Reference

| Command | Description |
|---|---|
| `/f promote <player>` | Promote a member one rank |
| `/f demote <player>` | Demote a member one rank |
| `/f kick <player>` | Remove a member from the faction |
| `/f leave` | Leave your current faction |
| `/f leader <player>` | Transfer leadership to another member |
| `/f rename <name>` | Rename your faction |
| `/f desc <text>` | Set your faction's description |
| `/f chat` | Toggle faction-only chat |
| `/f perm` | View or manage rank permissions |
| `/f disband` | Permanently disband the faction |