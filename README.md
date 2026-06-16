# NCustomItem
Pre-made configurations for custom items in NCustomItem

## Adding a preset from this repo

1. Download a preset, e.g. `poseidon.yml`.
2. Drop it into `plugins/NCustomItems/customitems/`.
3. Register it in `plugins/NCustomItems/config.yml` under the `items:` section:

   ```yaml
   items:
     poseidon:              # ← item ID (used in /nci give)
       enabled: true
       file: 'poseidon.yml' # ← file name inside customitems/
   ```

4. Reload the plugin:

   ```
   /nci reload
   ```

5. Give yourself the item:

   ```
   /nci give <player> poseidon
   ```

   …or open the GUI with every registered item: `/nci gui`.

> **Important:** dropping the `.yml` into `customitems/` is not enough on its own —
> the item only loads once it has an entry in the `items:` section of `config.yml`.
