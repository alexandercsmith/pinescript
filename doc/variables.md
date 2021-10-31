# 🌲 PineScript

> 📈 Trading View - PineScript Programming Language

---

## Variables

[PineScript Variables Reference](https://www.tradingview.com/pine-script-reference/v5)

| __Variable__ | __Type__ | __Description__ | __Value__ |
|:------------:|:--------:|:----------------|:---------:|
| `adjustment.dividends` | `String` | Dividends adjustment type | |
| `adjustment.none` | `String` |
| `adjustment.splits` | `String` |
| `alert.freq_all` | `String` |
| `alert.freq_once_per_bar` | `String` |
| `alert.freq_once_per_bar_close` | `String` |
| `bar_index` | `Integer` |
| `barmerge.gaps_off` | `barmerge_gaps` |
| `barmerge.gaps_on` | `barmerge_gaps` |
| `barmerge.lookahead_off` | `barmerge_lookahead` |
| `barmerge.lookahead_on` | `barmerge_lookahead` |
| `barstate.isconfirmed` | `Boolean` |
| `barstate.isfirst` | `Boolean` |
| `barstate.ishistory` | `Boolean` |
| `barstate.islast` | `Boolean` |
| `barstate.islastconfirmedhistory` | `Boolean` |
| `barstate.isnew` | `Boolean` |
| `barstate.isrealtime` | `Boolean` |
| `box.all` | `box[]` |
| `chart.bg_color` |
| `chart.fg_color` |
| `close` |
| `color.aqua` |
| `color.black` |
| `color.blue` |
| `color.fuchsia` |
| `color.gray` |
| `color.green` |
| `color.lime` |
| `color.maroon` |
| `color.navy` |
| `color.olive` |
| `color.orange` |
| `color.purple` |
| `color.red` |
| `color.silver` |
| `color.teal` |
| `color.white` |
| `color.yellow` |
| `currency.AUD` |
| `currency.CAD` |
| `currency.CHF` |
| `currency.EUR` |
| `currency.GBP` |
| `currency.HKD` |
| `currency.JPY` |
| `currency.NOK` |
| `currency.NONE` |
| `currency.NZD` |
| `currency.RUB` |
| `currency.SEK` |
| `currency.SGD` |
| `currency.TRY` |
| `currency.USD` |
| `currency.ZAR` |
| `dayofmonth` |
| `dayofweek` |
| `dayofweek.friday` |
| `dayofweek.monday` |
| `dayofweek.saturday` |
| `dayofweek.sunday` |
| `dayofweek.thursday` |
| `dayofweek.tuesday` |
| `dayofweek.wednesday` |
| `display.all` |
| `display.none` |
| `dividends.gross` |
| `dividends.net` |
| `earnings.actual` |
| `earnings.estimate` |
| `earnings.standardized` |
| `extend.both` |
| `extend.left` |
| `extend.none` |
| `extend.right` |
| `format.inherit` |
| `format.mintick` |
| `format.percent` |
| `format.price` |
| `format.volume` |
| `high` |
| `hl2` |
| `hlc3` |
| `hline.style_dashed` |
| `hline.style_dotted` |
| `hline.style_solid` |
| `hour` |
| `label.all` |
| `label.style_arrowdown` |
| `label.style_arrowup` |
| `label.style_circle` |
| `label.style_cross` |
| `label.style_diamond` |
| `label.style_flag` |
| `label.style_label_center` |
| `label.style_label_down` |
| `label.style_label_left` |
| `label.style_label_lower_left` |
| `label.style_label_lower_right` |
| `label.style_label_right` |
| `label.style_label_up` |
| `label.style_label_upper_left` |
| `label.style_label_upper_right` |
| `label.style_none` |
| `label.style_square` |
| `label.style_triangledown` |
| `label.style_triangleup` |
| `label.style_xcross` |
| `line.all` |
| `line.style_arrow_both` |
| `line.style_arrow_left` |
| `line.style_arrow_right` |
| `line.style_dashed` |
| `line.style_dotted` |
| `line.style_solid` |
| `location.abovebar` |
| `location.absolute` |
| `location.belowbar` |
| `location.bottom` |
| `location.top` |
| `low` |
| `math.e` |
| `math.phi` |
| `math.pi` |
| `math.rphi` |
| `minute` |
| `month` |
| `na` |
| `ohlc4` |
| `open` |
| `order.ascending` |
| `order.descending` |
| `plot.style_area` |
| `plot.style_areabr` |
| `plot.style_circles` |
| `plot.style_columns` |
| `plot.style_cross` |
| `plot.style_histogram` |
| `plot.style_line` |
| `plot.style_linebr` |
| `plot.style_stepline` |
| `plot.style_stepline_diamond` |
| `position.bottom_center` |
| `position.bottom_left` |
| `position.bottom_right` |
| `position.middle_center` |
| `position.middle_left` |
| `position.middle_right` |
| `position.top_center` |
| `position.top_left` |
| `position.top_right` |
| `scale.left` |
| `scale.none` |
| `scale.right` |
| `second` |
| `session.extended` |
| `session.ismarket` |
| `session.ispostmarket` |
| `session.ispremarket` |
| `session.regular` |
| `shape.arrowdown` |
| `shape.arrowup` |
| `shape.circle` |
| `shape.cross` |
| `shape.diamond` |
| `shape.flag` |
| `shape.labeldown` |
| `shape.labelup` |
| `shape.square` |
| `shape.triangledown` |
| `shape.triangleup` |
| `shape.xcross` |
| `size.auto` |
| `size.huge` |
| `size.large` |
| `size.normal` |
| `size.small` |
| `size.tiny` |
| `splits.denominator` |
| `splits.numerator` |
| `strategy.account_currency` |
| `strategy.cash` |
| `strategy.closedtrades` |
| `strategy.commission.cash_per_contract` |
| `strategy.commission.cash_per_order` |
| `strategy.commission.percent` |
| `strategy.direction.all` |
| `strategy.direction.long` |
| `strategy.direction.short` |
| `strategy.equity` |
| `strategy.eventrades` |
| `strategy.fixed` |
| `strategy.grossloss` |
| `strategy.grossprofit` |
| `strategy.initial_capital` |
| `strategy.long` |
| `strategy.losstrades` |
| `strategy.max_contracts_held_all` |
| `strategy.max_contracts_held_long` |
| `strategy.max_contracts_held_short` |
| `strategy.max_drawdown` |
| `strategy.netprofit` |
| `strategy.oca.cancel` |
| `strategy.oca.none` |
| `strategy.oca.reduce` |
| `strategy.openprofit` |
| `strategy.opentrades` |
| `strategy.percent_of_equity` |
| `strategy.position_avg_price` |
| `strategy.position_entry_name` |
| `strategy.position_size` |
| `strategy.short` |
| `strategy.wintrades` |
| `syminfo.basecurrency` |
| `syminfo.currency` |
| `syminfo.description` |
| `syminfo.mintick` |
| `syminfo.pointvalue` |
| `syminfo.prefix` |
| `syminfo.root` |
| `syminfo.session` |
| `syminfo.ticker` |
| `syminfo.tickerid` |
| `syminfo.timezone` |
| `syminfo.type` |
| `ta.accdist` |
| `ta.iii` |
| `ta.nvi` |
| `ta.obv` |
| `ta.pvi` |
| `ta.pvt` |
| `ta.tr` |
| `ta.vwap` |
| `ta.wad` |
| `ta.wvad` |
| `table.all` |
| `text.align_bottom` |
| `text.align_center` |
| `text.align_left` |
| `text.align_right` |
| `text.align_top` |
| `time` |
| `time_close` |
| `time_tradingday` |
| `timeframe.isdaily` |
| `timeframe.isdwm` |
| `timeframe.isintraday` |
| `timeframe.isminutes` |
| `timeframe.ismonthly` |
| `timeframe.isseconds` |
| `timeframe.isweekly` |
| `timeframe.multiplier` |
| `timeframe.period` |
| `timenow` |
| `volume` |
| `weekofyear` |
| `xloc.bar_index` |
| `xloc.bar_time` |
| `year` |
| `yloc.abovebar` |
| `yloc.belowbar` |
| `yloc.price` |