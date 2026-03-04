# Transformers

Transformers let you automatically convert field values as data moves between your connected services. You can chain multiple transformers together into a **pipeline** — each step takes the output of the previous step and applies its own transformation.

#### How it works

When you open the transformer configuration for a field mapping, you can add one or more **steps**. Each step applies a specific transformation to the value before it reaches the destination.

Steps run in order — Step 1 runs first, and its result is passed to Step 2, and so on. If any step fails, the entire pipeline stops and reports an error.

#### Available transformers

| Transformer              | What it does                                                                                                                                                                                                                                                                                                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Auto Convert**         | Converts a value to a specific data type (string, number, integer, boolean, or array).                                                                                                                                                                                                                                                                                         |
| **String to Number**     | Converts text to a number. Optionally strips currency symbols ($, €, £, etc.) or truncates decimals to produce a                                                                                                                                                                                                                                                               |
| **Source FK to Dest FK** | Translates foreign key references from the source service to the corresponding IDs in the destination. You select which folder contains the referenced records, and choose whether to output multiple values or just the first match. You can also decide what happens when a referenced record isn't found — either stop the sync or skip the missing reference and continue. |
| **Lookup Field**         | Follows a foreign key reference to pull a specific field value from the referenced record. You select the folder and specify the field path (e.g., `name` or `company.displayName`).                                                                                                                                                                                           |
| **JSONPath**             | Extracts values from structured data using a JSONPath expression (e.g., `$.store.book[0].title`). When the expression matches multiple values, you can choose to take the first, return them as an array, concatenate them, or join them with spaces or commas.                                                                                                                |

#### Example

Suppose your source service stores prices as text like `"$1,299.99"` and your destination expects a plain number. You could set up a two-step pipeline:

1. **String to Number** with "Strip currency symbols" enabled — converts `"$1,299.99"` to `1299.99`
2. **Auto Convert** with target type "integer" — converts `1299.99` to `1299`

#### Warnings and errors

If a step encounters something unexpected but can still produce a result, it will generate a **warning** — these are collected across all steps and reported at the end. If a step cannot produce a result at all, it generates an **error** and the pipeline stops immediately.
