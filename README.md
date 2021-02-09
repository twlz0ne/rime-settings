# 自用 Rime 配置

![demo](./demo.jpg)



## 基本套路：

-   Squirrel 0.15.0 简中全拼
-   0.15.0 后  `charset_filter@gb2312` 失效，放弃了朙月拼音方案，改用袖珍简化字方案 [rime](https://github.com/rime)/**[rime-pinyin-simp](https://github.com/rime/rime-pinyin-simp)**
-   精简字典
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

-   `pinyin_simp_3500` 《通用规范汉字表（2013）》的第一级 3500 常用字
-   `pinyin_simp_gb2312` GB2312 6763个字
-   `pinyin_simp_8105` [placeless](https://github.com/placeless)/**[squirrel_config](https://github.com/placeless/squirrel_config)** 的《通用规范汉字表》 8105 字
-   `aurora_pinyin` [hosxy](https://github.com/hosxy)/**[rime-aurora-pinyin](https://github.com/hosxy/rime-aurora-pinyin)** 的《通用规范汉字表》8105 字 + 一些在网络中常用的字/字符。
-   `dicts/pinyin_simp` 原版袖珍简化字词库，大约一万七千个字左右

我一点生僻字都不想要，就又弄了一个 GB2312 的精简版，干脆再弄了一个 3500 常用字。

偶尔发现有打不出来的，但不是特别生僻的，会手动加进来。

<br>

生僻字没了，选字方便了许多，但是偶尔偶尔遇到的生僻字无法打出来。

切换字典要重新部署才行，不知道要怎么样才能像以前切换字符集那样切换字库，谁要知道求告知。

把这些词库都放上了，可以自己选择。  

<br>

精简字库比较方便的地方：

比如「丞」字不在 3500 里面，但是扩展词库里有「丞相」这个词，也是可以打出来的。

这个需要扩展词库带拼音。（不带拼音打不出来）  

<br>


## 详细说明

[我的 Rime 配置 2021](https://dvel.xyz/post/30/)

