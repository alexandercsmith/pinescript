# 🌲 PineScript

> 📈 Trading View - PineScript Programming Language

---

* [`strategy()`](#strategy)
* [`strategy.entry()`](#strategy.entry)
* [`strategy.close()`](#strategy.close)
* [`strategy.exit()`](#strategy.exit)

---

## `strategy()`

[PineScript Strategy Reference](https://www.tradingview.com/pine-script-docs/en/v5/concepts/Strategies.html)

```
strategy(
    title, 
    shorttitle, 
    overlay, 
    format, 
    precision, 
    scale, 
    pyramiding, 
    calc_on_order_fills, 
    calc_on_every_tick, 
    max_bars_back, 
    backtest_fill_limits_assumption, 
    default_qty_type, 
    default_qty_value, 
    initial_capital, 
    currency, 
    slippage, 
    commission_type, 
    commission_value, 
    process_orders_on_close, 
    close_entries_rule, 
    margin_long, 
    margin_short, 
    explicit_plot_zorder, 
    max_lines_count, 
    max_labels_count, 
    max_boxes_count
) → void
```

### Arguments

| __Declaration__ | __Type__ | __Default__      | __Description__ |
|:---------------:|:--------:|:----------------:|:----------------|
| `title` | String | _Required_ | Indicator title that would be seen in Indicators/Strategies widget |
| `shorttitle` | String | _Optional_ | Indicator short title that would be seen in the chart legend |
| `overlay` | Boolean | `false` | True: Indicator added as overlay; False: added on separate chart |
| `format` | String | `format.inherit` | Type of formatting indicator values on the price axis |
| `precision` | Integer | | Number of digits after the floating point for indicator values on the price axis |
| `scale` | scale_type | | Price scale that the indicator should be attached to |
| `pyramiding` | Integer | `0` | The maximum number of entries allowed in the same direction |
| `calc_on_order_fills` | Boolean | `false` | Additional one time intrabar order calculation. Strategy is recalculated once intrabar after an order is filled |
| `calc_on_every_tick` | Boolean | `false` | Additional intrabar strategy calculations. Strategy will calculate on every tick in real-time, rather than on bars' closes |
| `max_bars_back` | Integer | | Maximum number of bars available for a strategy for historical reference |
| `default_qty_type` | String | `strategy.fixed` | Parameter to determine the number of contracts/shares/lots/units to trade |
| `default_qty_value` | Integer, Float | `strategy.cash` | Number of contracts/shares/lots/units |
| `initial_capital` | Integer, Float | `100000` | The amount of funds initially available for the strategy to trade |
| `currency` | String | | Account currency for this strategy. Optional. The default is the currency that the symbol on the chart is traded on |
| `commission_type` | String | | Commission type for an order |
| `commission_value` | Integer, Float | | Commission value for an order |
| `process_orders_on_close` | Boolean | `false` | When set to `true`, generates an additional attempt to execute orders after a bar closes and strategy calculations are completed. If the orders are market orders, the broker emulator executes them before the next bar's open. If the orders are conditional on price, they will only be filled if the price conditions are met |
| `close_entries_rule` | String | `FIFO` | Determines the order in which orders are closed |
| `margin_long` | Integer, Float | `100` | Margin long is the percentage of the purchase price of a security that must be covered by cash or collateral for long positions |
| `margin_short` | Integer, Float | `100` | Margin short is the percentage of the purchase price of a security that must be covered by cash or collateral for short positions |
| `explicit_plot_zorder` | Boolean | `false` | Specifies the order in which the indicator's plots, fills, and hlines are rendered |
| `max_lines_count` | Integer | `50` | The number of last line drawings displayed |
| `max_labels_count` | Integer | `50` | The number of last label drawings displayed |
| `max_boxes_count` | Integer | `50` | The number of last box drawings displayed |

---

## `strategy.entry()`

It is a command to enter market position. If an order with the same ID is already pending, it is possible to modify the order. If there is no order with the specified ID, a new order is placed.

```
strategy.entry(
    id, 
    direction, 
    qty, 
    limit, 
    stop, 
    oca_name, 
    oca_type, 
    comment, 
    when, 
    alert_message
) → void
```

### Arguments

| __Declaration__ | __Type__ | __Default__      | __Description__ |
|:---------------:|:--------:|:----------------:|:----------------|
| `id` | String | | The order identifier |
| `direction` | strategy_direction | | Market position direction: 'strategy.long' is for long, 'strategy.short' is for short |
| `qty` | Integer, Float | | Number of contracts/shares/lots/units to trade |
| `limit` | Integer, Float | | Limit price of the order. Either: `limit`, or `stop-limit` |
| `stop` | Integer, Float | | Stop price of the order. Either: `limit`, or `stop-limit` |
| `oca_name` | String | | Name of the OCA group the order belongs to |
| `oca_type` | String | | Type of the OCA group |
| `comment` | String | | Additional notes on the order |
| `when` | Boolean | | Condition of the order |
| `alert_message` | String | | Replace: `{{strategy.order.alert_message}}` |

---

## `strategy.close()`

It is a command to exit from the entry with the specified ID. If there were multiple entry orders with the same ID, all of them are exited at once. If there are no open entries with the specified ID by the moment the command is triggered, the command will not come into effect. The command uses market order. Every entry is closed by a separate market order.

```
strategy.close(
    id, 
    when, 
    comment, 
    qty, 
    qty_percent, 
    alert_message
) → void
```

### Arguments

| __Declaration__ | __Type__ | __Default__      | __Description__ |
|:---------------:|:--------:|:----------------:|:----------------|
| `id` |
| `when` |
| `comment` |
| `qty` |
| `qty_percent` |
| `alert_message` |

---

## `strategy.exit()`

It is a command to exit either a specific entry, or whole market position. If an order with the same ID is already pending, it is possible to modify the order. If an entry order was not filled, but an exit order is generated, the exit order will wait till entry order is filled and then the exit order is placed. 

```
strategy.exit(
    id, 
    from_entry, 
    qty, 
    qty_percent, 
    profit, 
    limit, 
    loss, 
    stop, 
    trail_price, 
    trail_points, 
    trail_offset, 
    oca_name, 
    comment, 
    when, 
    alert_message
) → void
```

### Arguments

| __Declaration__ | __Type__ | __Default__      | __Description__ |
|:---------------:|:--------:|:----------------:|:----------------|
| `id` |
| `from_entry` |
| `qty` |
| `qty_percent` |
| `profit` |
| `limit` |
| `loss` |
| `stop` |
| `trail_price` |
| `trail_points` |
| `trail_offset` |
| `oca_name` |
| `comment` |
| `when` |
| `alert_message` |