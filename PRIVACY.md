# Privacy Policy — Reaccoin

**Last updated:** 12/11/2026 (DD/MM/YYYY)
**Bot:** Reaccoin
**Operator / Contact:** ANormalDumbass / 96_

This policy explains what data Reaccoin ("the Bot", "we") collects when it is
used in a Discord server, why, and what happens to it. **Short version: the
Bot counts reactions and records who reacted to what. It does not read or
store the text of your messages.**

---

1.- What we collect

When the Bot is active in a server, it automatically records:

| Data | Purpose |
|---|---|
| **User IDs** (Discord snowflakes) — of the message author and of the reacting user | To credit "coins" to the message author, prevent self-reactions from mining, maintain wallets, and show leaderboards |
| **Reaction data** — which emoji was used (including custom and external emoji names/IDs), and whether it was added or removed | This is the core data of the Bot: reactions are simulated as market "demand buys" |
| **Message IDs, channel IDs, server (guild) IDs** | To attribute reactions to specific messages and to reverse ("claw back") coins when a reaction or message is removed |
| **Timestamps** of the above events | For the market price history, charts, and daily faucet cooldowns |
| **In-bot transaction data** — simulated $CASH and coin balances, trades, wallet contents | To operate the simulated market |

**Message content:** the Bot uses the *Message Content* privileged intent for
technical reliability (resolving message authors for uncached messages), but
it **does not read, store, or transmit the text or attachments of your
messages**. Only the message's author ID and its ID are recorded. If message
content is ever displayed, it is only what a user typed directly into a bot
command as an argument (e.g., an emoji), and that is not persisted beyond the
resulting market action.

**What we do NOT collect:**
- Message text, attachments, embedded links, or file contents
- Voice data, direct messages, or anything from servers where the Bot, Reaccoin, is not installed
- Email addresses, phone numbers, IP addresses, or payment information (we don't have a
  website where this information could even be accessed by us)

2.- Why we process this data (lawful basis)

- To operate the service you voluntarily use (the reaction-tracking market) —
  legitimate interest / contract performance.
- All participation is **voluntary**: using the Bot's commands or reacting in a
  server where it operates. Server admins choose to install the Bot; users can
  avoid tracking by not reacting to messages or not trading.

3.- Storage, retention, and security

- Data is stored in a **SQLite database plus CSV mirror** on the machine the
  Bot, Reaccoin, is hosted on (currently a private local/cloud server operated by
  Reaccoin's operator).
- Reaction records are kept **indefinitely** as a historical ledger (needed
  for coin "provenance" and clawbacks).
- We apply reasonable technical measures (file-system access being limited to
  the operator; no public endpoints expose the data).
- **Data is never sold, rented, or shared with third parties.** The only
  parties involved are Discord (whose own privacy policy governs Discord's
  processing) and the hosting provider of Reaccoin's process, if any.

4.- Your rights and choices

You can, at any time:

- **Request a copy** of the data associated with your Discord user ID.
- **Request deletion** of your user data (wallets, trades, leaderboard
  entries). Reaction-ledger rows may be anonymized (user ID replaced with a
  placeholder) rather than deleted, since the ledger is append-only, but the
  association with your identity will be removed.
- **Opt out** by simply not using Reaccoin's commands or not reacting to
  messages in servers where it is installed.
- Server administrators may remove the Bot at any time, which stops all new
  data collection (existing data can be deleted on request).

To exercise any of these, contact the operator at the address above.

5.- Data of deleted messages

When a message or reaction is deleted on Discord, the Bot performs financial
"clawbacks" using its stored records. The fact that something was deleted may
be reflected in the transaction ledger (it is part of how the simulated market
works), but no message content is ever involved.

6.- Children

The Bot is not directed at children. Consistent with Discord's Terms of
Service, users must be at least 13 years old (or the minimum age required by
their country's law) to use Discord, and therefore to use the Bot.

7.- Changes to this policy

Material changes will be announced in the Bot's designated announcement
channel. Continued use after changestake effect constitutes acceptance.

8.- A note on value

Everything the Bot tracks and simulates ("coins", "$CASH", market caps,
portfolios) has **no real-world value of any kind**. No personal data is
processed for any financial purpose because there is no money here.
