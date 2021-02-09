# 自用 Rime 配置

![demo](./demo.jpg)



## 基本套路：

-   Squirrel 0.15.0 简中全拼
-   0.15.0 后  `charset_filter@gb2312` 失效，放弃了朙月拼音方案，改用袖珍简化字方案 [rime](https://github.com/rime)/**[rime-pinyin-simp](https://github.com/rime/rime-pinyin-simp)**
-   精简字典 3500 常用字
-   扩展词库只保留了成语俗语与古诗词，需要大量词库的可参考  [liuour](https://github.com/liuour)/**[rime](https://github.com/liuour/rime)**
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

-   `pinyin_simp_3500` 《通用规范汉字表》的第一级 3500 常用字
-   `pinyin_simp_gb2312` GB2312 6763个字
-   `pinyin_simp_8105` [placeless](https://github.com/placeless)/**[squirrel_config](https://github.com/placeless/squirrel_config)** 的《通用规范汉字表》 8105 字
-   `aurora_pinyin` [hosxy](https://github.com/hosxy)/**[rime-aurora-pinyin](https://github.com/hosxy/rime-aurora-pinyin)** 的《通用规范汉字表》8105 字 + 一些在网络中常用的字/字符。
-   `dicts/pinyin_simp` 原版袖珍简化字词库，大约一万七千个字左右

我一点生僻字都不想要，就又弄了一个 GB2312 的精简版，干脆再弄了一个 3500 常用字。

将 3500 字典精心调教了一下，注释掉了约 300 多个不常用的字，主要是多音字，增加了一些常用的字词。

调教原则：

-   「参差 cen ci」只有在这个词中，这两个字才会发这个音，所以注释掉这两个音，平常直接打词语就可以了。
-   「蚯蚓」很常用，但是一般不会单独打出两个字中的其中一个，所以注释掉。
-   「大 dai」基本只有「大夫」「大王」，增加词汇，注释单字，节约候选项。
-   「龟 qiu」闻所未闻也永远不会使用的多音字，直接注释掉。

<br>

精简字库比较方便的地方：

比如「丞」字不在 3500 里面，但是扩展词库里有「丞相」这个词，也是可以打出来的。

这个需要词库带拼音才行。（如果字典里没有这个字，扩展词库里没有拼音，则打不出来）  

注意增加的扩展词库有没有拼音，像古诗词之类的里面有很多字都不在 3500 字里面，但只要词库带拼音的话就可以打出来。

<br>

生僻字没了，选字方便了许多，日常使用倍儿舒服。

但是偶尔偶尔遇到的生僻字无法打出来，需要切换字典要重新部署才行。

所以创建一个 Plan B 方案供临时使用大字符集之用，默认设定了为 `aurora_pinyin` 的词库并改名为 `plan_b` 了。

<br>

## 遗憾

俩方案的个人词库不共享，如果能共享就好了。

如果能在同一个方案下可随时切换不同的字符集就好了。

如果 Rime 能支持不同方案使用不同皮肤就好了。

