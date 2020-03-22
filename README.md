## CompoundOptions

Compound Options allows you to configure some options for a new monument "Compound" (scientists town).

### Features

   - Configure sell prices and lists for vending machines (via data/CompoundOptions.json)
   - Disable Compound SafeZone trigger (attack player when enter to area with loaded gun or attack any NPC), defaults - off
   - Disable Compound Turrets, defaults - off
   - Disallow Compound NPC (for rollback need restart server/respawn npc), defaults - off
   - Disable Compound vending machines, defaults - off (for rollback if switched 'on' need restart server)

### Notes

For first run, the plugin automatically creates data/CompoundOptions.json with defaults (in-game). You can manually change fields in this file and reload plugin to apply.

On every server load, the plugin automatically creates data/CompoundOptions.json with the server default vending machine configuration.

Then we can see array of fields, where:

   - comment - comment for you, not used in code
   - sellId - ID of item what you sell
   - sellAmount - Price in currency for order
   - currencyId - ID of yours currency
   - currencyAmount - how many you sold for 1 order (sellAmount)

### Configuration
The settings and options for this plugin can be configured in the CompoundOptions.json file under the oxide/config directory. The use of a JSON editor or validation site such as jsonlint.com is recommended to avoid formatting issues and syntax errors.

```json
{
  "Allow custom sell list for Compound vending machines (see in data)": true,
  "Disable Compound SafeZone trigger": false,
  "Disable Compound Turrets": false,
  "Disable Compound Vending Machines": false,
  "Disallow Compound NPC": false
  "Disallow Bandit NPC": false
}
```

### Planned Features

   - More options for vending machines
   - Ability for restock time set
   - Numerous bug fixes
