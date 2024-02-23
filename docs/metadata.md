这个文档是对 `metadata.json` 的解释性补充,文档是按照数据格式进行解释的，不必担心顺序问题。

# "generation": "Num"
| 字段 | 数据类型 |
| ---- | -------- |
| Num  | 字符串   |

解释：`Num` 是一个自增序列，初值是0，表示目前 `export.json` 数据的版本。


# "generationTypes": { ... }
表示不同账户拥有的视频类型

## "Length": [ ... ]
视频长度标记

| 类型 | 解释 |
| - | - |
| Short  | 0min < t ≤ 1min |
| Medium  | 1min < t ≤ 5min |
| Long  | 5min < t ≤ 20min |
| VeryLong | 20min < t ≤ 120min |
| TerriblyLong | 120min < t ≤ 600min |

## "Direction": [ ... ]
视频的方向，表示该账户视频有什么类型。

| 类型 | 解释 |
| - | - |
| News | 新闻相关 |
| Recreation | 娱乐相关 |
| Foods | 美食相关 |
| Sport | 运动和体育相关 |
| History | 历史相关 |
| Animal | 动物相关 |
| Movie | 电影解说 |