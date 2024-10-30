# Encoding

In modern computers, text (or string) can be saved in different methods.

Fluxion also supports storing text in the name of the each node and or in the value.

However, not all Fluxion libraries support all of the encodings.

All encodings supported by Fluxion are Little Endian with No Byte Order Mark.

Here's a table for all official Fluxion ports and the encodings they support:

| ID | Encoding  | libFluxion (C++)       | FluxionSharp (.NET)     |
|----|-----------|------------------------|-------------------------|
| 0  | UTF-8     | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0  |
| 1  | UTF-16    | :heavy_check_mark: 1.0 | :heavy_check_mark: 1.0  |
| 2  | UTF-32    | :x:                    | :heavy_check_mark: 1.0  |
