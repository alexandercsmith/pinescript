# 🌲 PineScript

> 📈 Trading View - PineScript Programming Language

---

## Operators

[PineScript Operators Reference](https://www.tradingview.com/pine-script-reference/v5)


### Arithmetic

| __Operator__ | __Usage__                | __Syntax__        | __Type__      |
|:------------:|:-------------------------|:------------------|:-------------:|
| `+`          | Addition                 | `val + val`       | `Int` `Float` |
| `+=`         | Addition Assignment      | `val += val`      | `Int` `Float` |
| `-`          | Subtraction              | `val - val`       | `Int` `Float` |
| `-=`         | Subtraction Assignment   | `val -= val`      | `Int` `Float` |
| `*`          | Multiply                 | `val * val`       | `Int` `Float` |
| `*=`         | Multiply Assignment      | `val *= val`      | `Int` `Float` |
| `/`          | Division                 | `val / val`       | `Int` `Float` |
| `/=`         | Division Assignment      | `val /= val`      | `Int` `Float` |
| `%`          | Modulo                   | `val % val`       | `Int` `Float` |
| `%=`         | Modulo Assignment        | `val %= val`      | `Int` `Float` |
| `<`          | Less Than                | `val < val`       | `Boolean`     |
| `<=`         | Less Than or Equal To    | `val <= val`      | `Boolean`     |
| `>`          | Greater Than             | `val > val`       | `Boolean`     |
| `>=`         | Greater Than or Equal To | `val >= val`      | `Boolean`     |
| `==`         | Equal To                 | `val == val`      | `Boolean`     |
| `!=`         | Not Equal To             | `val != val`      | `Boolean`     |
| `?:`         | Ternary Conditional      | `val ? val : val` | `Any`         |
| `[]`         | Series Value             | `val[val]`        | `Subscript`   |


### Symbol

| __Operator__ | __Usage__         | __Syntax__                                                            | __Type__      |
|:------------:|:------------------|:----------------------------------------------------------------------|:-------------:|
| `and`        | Logical And       | `val and val`                                                         | `Boolean`     | 
| `export`     | Script Export     | `export func1() =>`                                                   | `Library`     |
| `for`        | For Statement     | `for counter = from_num to num []`                                    | `Expression`  |
| `if`         | If Condition      | `if options...`                                                       | `Expression`  |
| `import`     | Library Import    | `import {username}/{libraryName}/{libraryVersion} as {alias}`         | `Library`     |
| `not`        | Logical Not       | `not val`                                                             | `Expression`  |
| `or`         | Logical Or        | `val or val`                                                          | `Expression`  |
| `series`     | Library Export    | `export <functionName>([[series] <type>] <arg1>[ = <default_value>])` | `Library`     |
| `simple`     | Function Keyword  | `export <functionName>([[simple] <type>] <arg1>[ = <default_value>])` | `Declaration` |
| `switch`     | Multi-Conditional | `[variable_declaration = ] switch expression`                         | `Expression`  |
| `var`        | Variable          | `var variable_name = expression`                                      | `Declaration` |
| `varip`      | Variable Intrabar | `varip variable_name = expression`                                    | `Declaration` |
| `while`      | While Condition   | `variable_declaration = while boolean_expression`                     | `Expression`  |