
| -------------- | ---------------------------------------- |
| 空值(Null)     | `nothing`                                |
| 缺失数据        | `missing`                                |
| 浮点数的非数值  | `NaN`                                    |
| 滤除缺失值      | `collect(skipmissing([1, 2, missing])) == [1,2]` |
| 替换缺失值      | `collect((df[:col], 1))`                 |
| 检查是否有缺失值 | `ismissing(x)` **而不是** `x == missing` |
