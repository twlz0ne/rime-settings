# 自用 Rime 配置

![demo](./demo.jpg)



## 基本套路：

-   Squirrel 0.15.0 简中全拼
-   0.15.0 后  `charset_filter@gb2312` 失效，放弃了朙月拼音方案，改用袖珍简化字方案 [rime](https://github.com/rime)/**[rime-pinyin-simp](https://github.com/rime/rime-pinyin-simp)**
-   精简字典 3500 常用字
-   扩展词库只保留了成语俗语、古诗词、医药名称，需要大量词库的可参考  [liuour](https://github.com/liuour)/**[rime](https://github.com/liuour/rime)**
-   简型八股文模型 [lotem](https://github.com/lotem)/**[rime-octagram-data/tree/hans](https://github.com/lotem/rime-octagram-data/tree/hans)**
-   英文输入方案 Easy English Nano [mityliu](https://github.com/mityliu)/**[rime-custom](https://github.com/mityliu/rime-custom)**
-   袖珍方案输出繁体，参考了五笔的简入繁出 [rime/home/issues#388](https://github.com/rime/home/issues/388#issuecomment-504572224) 
-   动态日期、时间、星期 [KyleBing](https://github.com/KyleBing)/**[rime-wubi86-jidian](https://github.com/KyleBing/rime-wubi86-jidian)**
-   所有标点符号直接上屏
-   「/」模式改为「v」模式，「/」直接上屏
-   在 `opencc/` 增加了一些符号映射，如 「⌘」「⌥」「⌃」
-   没有 emoji 候选，`symbols` 里有一点点，如需要 emoji 可参考  [liuour](https://github.com/liuour)/**[rime](https://github.com/liuour/rime)**
-   `symbols` 中都改为简体字（如节气、八卦），增加一些自定义符号
-   常用全拼自动纠错：`ni tina tain do zia gna she me` → `你天天都在干什么`

<br>

## 精简字典

-   `pinyin_simp_3500` 《通用规范汉字表》的第一级 3500 常用字 + 偶尔增加一些平时发现会用到的字词。
-   `pinyin_simp_gb2312` GB2312 6763个字
-   `pinyin_simp_8105` [placeless](https://github.com/placeless)/**[squirrel_config](https://github.com/placeless/squirrel_config)** 的《通用规范汉字表》 8105 字
-   `aurora_pinyin` [hosxy](https://github.com/hosxy)/**[rime-aurora-pinyin](https://github.com/hosxy/rime-aurora-pinyin)** 的《通用规范汉字表》8105 字 + 一些在网络中常用的字/字符。
-   `dicts/pinyin_simp` 原版袖珍简化字词库，大约一万七千个字左右

弄了个 Plan B 方案供临时切换大字符集打出生僻字。

<br>

## 遗憾

俩方案的个人词库不共享，如果能共享就好了。

如果能在同一个方案下可随时切换不同的字符集就好了。

如果 Rime 能支持不同方案使用不同皮肤就好了。

