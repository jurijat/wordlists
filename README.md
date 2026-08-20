# wordlists

Public files the vast.ai hashcat boxes download at attack time.

Vast `onstart` is capped at 16 KB, so lists and larger rules live here and are
`curl`ed from `raw.githubusercontent.com` instead of being inlined.

| Path | What |
|---|---|
| `names/country-names.txt` | Russia + India + China + Japan given names and surnames (Latin / pinyin / romaji), already folded |
| `names/country-names.txt.gz` | Same, gzipped — this is what the box downloads |
| `rules/wallet-human.rule` | Compact wallet.dat rules |
| `rules/wallet-human-v2.rule` | Brutal v2 |
| `rules/wallet-human-v2-min10.rule` | Brutal v2 + `--pw-min 10` |
| `rules/wallet-complement.rule` | Case / leet / `!` only |
