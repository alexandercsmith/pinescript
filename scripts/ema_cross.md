# 🌲 PineScript

> 📈 Trading View - PineScript Programming Language

---

## EMA Cross

* Simple Exponential Moving Average __EMA__ crossover and crossunder strategy.

```
//@version=5
strategy("EMA Cross")

ema50 = ta.ema(close, 50)
ema200 = ta.ema(close, 200)

if ta.crossover(ema50, ema200)
    strategy.entry("buy", strategy.long, 10, when = strategy.position_size <= 0)

if ta.crossunder(ema200, ema50)
    strategy.entry("sell", strategy.short, 10, when = strategy.position_size > 0)
    
plot(strategy.equity)
```