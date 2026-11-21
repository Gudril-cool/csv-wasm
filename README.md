# csv-wasm

[![make.fun · csv-reader-speed-01-run-20261121](https://make.fun/badge/csv-reader-speed-01-run-20261121.svg)](https://make.fun/bounty/csv-reader-speed-01-run-20261121?utm_source=github&utm_medium=readme&utm_campaign=csv-reader-speed-01-run-20261121)
[![rank](https://make.fun/badge/csv-reader-speed-01-run-20261121/Gudril-cool/csv-wasm/rank.svg)](https://make.fun/bounty/csv-reader-speed-01-run-20261121/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=csv-reader-speed-01-run-20261121)
[![reward](https://make.fun/badge/csv-reader-speed-01-run-20261121/Gudril-cool/csv-wasm/reward.svg)](https://make.fun/bounty/csv-reader-speed-01-run-20261121?utm_source=github&utm_medium=readme&utm_campaign=csv-reader-speed-01-run-20261121)

A WebAssembly SIMD drop-in replacement for csv-reader 1.0.0, entered in the make.fun csv-reader speed competition. The parsing core is Rust compiled to wasm32 with v128 SIMD scanning over UTF-16 code units; fields are returned as spans of the input wherever possible, so results are identical to the reference parser on every input — including broken rows, stray CRs, quote junk and unterminated quotes — at several times the speed.

## Run it

```sh
node main.ts
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=x6sa47yh&utm_source=github&utm_medium=readme&utm_campaign=csv-reader-speed-01-run-20261121)</sub>
