# Different ways to run schematics from the angular schematic

| Run schematic 🔽          | Create a rule                                                   | Add task in context                                                          |
| ------------------------ | --------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| From same collection     | `rule = schematic(schemaName, options)`                         | `context.addTask(new RunSchematicTask(schemaName, options))`                 |
| From external collection | `rule = externalSchematic(collectionName, schemaName, options)` | `context.addTask(new RunSchematicTask(collectionName, schemaName, options))` |
