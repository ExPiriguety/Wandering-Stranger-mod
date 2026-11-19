# Wandering Stranger

**Wandering Stranger** adds a custom wandering merchant to **Minecraft 1.20.1 with Forge**. Inspired by the vanilla Wandering Trader, this merchant appears near players according to configurable rules, offers common and special trades, and leaves after a configurable amount of time.

## Features

By default, the first visit is guaranteed to happen on or after day five, around noon. Later spawn attempts start with a 25% chance, which increases by 25% for each day the merchant does not appear.

The merchant spawns 20–40 blocks from a player and stays for about four minutes. If a player is still trading with it when its visit is over, it waits until the trade is finished before leaving.

You can customize the spawn schedule, chances, distance, minimum time between visits, stay duration, and arrival and departure announcements.

## Custom Trades

Trades are configured in `config/wandering_stranger/trades.json`, which is created automatically. You can define common and special trade pools, choose the items players pay and receive, set the number of uses for each offer, and select the merchant’s currency.

Any registered item can be used as currency, including items added by other mods. Each merchant’s offers are generated when it appears and saved with the entity, so they persist across world restarts. The mod does not overwrite the configuration file during normal use.

Operators can also manage trades in-game with `/stranger editor`.

## Commands

These commands require operator permissions:

- `/stranger editor` — Open the in-game trade editor.
- `/stranger reload` — Reload the configuration and trades.
- `/stranger status` — Check the spawn status and next spawn chance.
- `/stranger summon` — Summon a merchant at your location or at specified coordinates.
- `/stranger roll` — Attempt a spawn using the configured rules.
- `/stranger force` — Force a merchant to spawn.
- `/stranger reset` — Reset the saved spawn state.

## Vanilla Wandering Trader

You can choose whether vanilla Wandering Traders remain in the world, have their natural spawning disabled, or are removed completely. By default, the mod removes vanilla Wandering Traders.

## Credits

The merchant’s model, texture, and sounds were adapted from the community resource pack “Merchant from Resident Evil 4!”.
