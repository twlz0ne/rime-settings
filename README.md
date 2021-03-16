# 自用 Rime 配置

![demo](./demo.jpg)



## 基本套路：

-   Squirrel 0.15.2 简中全拼
-   0.15.0 后  `charset_filter@gb2312` 失效，放弃了「朙月拼音·简化字」方案，改用袖珍简化字方案 [rime](https://github.com/rime)/**[rime-pinyin-simp](https://github.com/rime/rime-pinyin-simp)**
-   在简化字词库基础上精简了字表
-   扩展词库：四叶草的基础词库（[fkxxyz](https://github.com/fkxxyz)/**[rime-cloverpinyin](https://github.com/fkxxyz/rime-cloverpinyin)**），搜狗的成语俗语、古诗词、医药名称、中文维基词库
-   英文输入方案 Easy English Nano [mityliu](https://github.com/mityliu)/**[rime-custom](https://github.com/mityliu/rime-custom)**
-   袖珍方案输出繁体，参考了五笔的简入繁出 [rime/home/issues#388](https://github.com/rime/home/issues/388#issuecomment-504572224) 
-   动态日期、时间、星期 [KyleBing](https://github.com/KyleBing)/**[rime-wubi86-jidian](https://github.com/KyleBing/rime-wubi86-jidian)**
-   所有标点符号直接上屏
-   「/」模式改为「v」模式，「/」直接上屏
-   在 `opencc/` 增加了一些符号映射，如 「⌘」「⌥」「⌃」
-   没有 emoji 候选，`symbols` 里有一点点，如需要 emoji 可参考  [liuour](https://github.com/liuour)/**[rime](https://github.com/liuour/rime)**、[fkxxyz](https://github.com/fkxxyz)/**[rime-cloverpinyin](https://github.com/fkxxyz/rime-cloverpinyin)** 等。
-   增加了许多全拼纠错

<br>

## 精简字表

-   `pinyin_simp_3500` 《通用规范汉字表》的第一级 3500 常用字
-   `pinyin_simp_gb2312` GB2312 6763个字
-   `pinyin_simp_8105` 《通用规范汉字表》 8105 字
-   `pinyin_simp` 原版袖珍简化字词库，大约一万七千个字左右

<br>

## 其他

在  `custom_phrase.txt` 中可以设置某些字词永远只出现在前 N 个候选项，但是这样设置之后，这些字词就不能与正常的字共同造词。现在不知道如何能完美的固定某些字词的候选项顺序。

