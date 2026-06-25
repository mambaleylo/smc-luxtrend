# smc-trendlines

SMC Optimizer v3.51 -- SMC + LuxAlgo Trendline Breaks filter.

## New vs smc-optimizer v3.50.2

Three new optimizer params:

| Param | Range | Description |
|---|---|---|
| `tl_mult` | 0.5-3.0 | Slope multiplier |
| `tl_method` | atr/stdev/linreg | Slope calculation (LuxAlgo port) |
| `tl_filter` | False/True | Enable trendline breakout filter |

When `tl_filter=True`:
- Long OB entry: only when price broke the lower trendline upward (tl_upos=1)
- Short OB entry: only when price broke the upper trendline downward (tl_dnos=1)

When `tl_filter=False`: identical to smc-optimizer v3.50.2.

## Base repo

https://github.com/mambaleylo/smc-optimizer
