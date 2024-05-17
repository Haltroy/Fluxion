# Flags

In Fluxion, flags and values are stored in the same byte in order to save space.

## Node Flags

In order to set a node flag, one must XOR it with the value ID.

In order to get a flag, using NAND or bit-shift operations are common.

Nodes have 3 flags:

- Node has name "Name Flag": 4th bit (16 in decimal).
- Node has no child "No Child Flag": 5th bit (32 in decimal).
- Node has no attribute "No Attribute Flag": 6th bit (64 in decimal).

## Value IDs

Nodes can have different values.

Sometimes these value types are not supported or partially supported
by an official Fluxion port. Here's a table for that:

| Index | Value Type              | libFluxion (C++)       | FluxionSharp (.NET)    |
| ----- | ----------------------- |------------------------|------------------------|
| 0     | Null                    | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 1     | Bool True               | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 2     | Bool False              | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 3     | Byte                    | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 4     | Signed Byte             | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 5     | Char (UTF-16 LE no-BOM) | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 6     | 16-bit Integer          | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 7     | 16-bit Unsigned Integer | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 8     | 32-bit Integer          | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 9     | 32-bit Unsigned Integer | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 10    | 64-bit Integer          | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 11    | 64-bit Unsigned Integer | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 12    | Float                   | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 13    | Double                  | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 14    | String                  | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
| 15    | Byte Array              | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0 |
