# wordlists

Public files the vast.ai hashcat boxes download at attack time.

Vast `onstart` is capped at 16 KB, so lists and larger rules live here and are
`curl`ed from `raw.githubusercontent.com` instead of being inlined.

| Path | What |
|---|---|
| `names/country-names.txt.gz` | RU/IN/CN/JP Latin/pinyin/romaji (folded) |
| `names/world-names.txt.gz` | Worldwide given names + surnames, unique ASCII |
| `names/native-names.txt.gz` | RU Cyrillic + ZH hanzi + JA kanji (UTF-8). Not for leet rules |
| `rules/wallet-human.rule` | Compact wallet.dat rules |
| `rules/wallet-human-v2.rule` | Brutal v2 |
| `rules/wallet-human-v2-min10.rule` | Brutal v2 + reject `>A` (keep length ≥ 10) |
| `rules/wallet-complement.rule` | Case / leet / `!` only |
