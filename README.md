# 自用 Rime 配置

![demo](./demo.jpg)



## 基本套路：

-   Squirrel 0.15.2 简中全拼
-   0.15.0 后  `charset_filter@gb2312` 失效了，放弃了「朙月拼音·简化字」方案，改用「袖珍简化字方案」 [rime](https://github.com/rime)/**[rime-pinyin-simp](https://github.com/rime/rime-pinyin-simp)**
-   精简了字表
-   华宇拼音（紫光拼音）的系统词库 http://unispim.com/wordlib/wordlib_detail.php?id=8
-   英文输入方案 Easy English Nano [mityliu](https://github.com/mityliu)/**[rime-custom](https://github.com/mityliu/rime-custom)**
-   袖珍方案输出繁体，参考了五笔的简入繁出 [rime/home/issues#388](https://github.com/rime/home/issues/388#issuecomment-504572224) 
-   动态日期、时间、星期 [KyleBing](https://github.com/KyleBing)/**[rime-wubi86-jidian](https://github.com/KyleBing/rime-wubi86-jidian)**
-   所有标点符号直接上屏，「/」模式改为「v」模式，「/」直接上屏
-   没有 emoji，只在 `symbols` 里保留了不到 10 个常用的，如需要可参考 [maomiui](https://github.com/maomiui)/**[rime](https://github.com/maomiui/rime)** 、[fkxxyz](https://github.com/fkxxyz)/**[rime-cloverpinyin](https://github.com/fkxxyz/rime-cloverpinyin)** 等。
-   增加了许多全拼纠错（手速太快经常按错😅）
-   参考谷歌、《现代汉语规范词典》、[异形词整理表](https://wucuozi.com/cuobiezi/yixingzi/)、[错别字辨析](https://wucuozi.com/bian/ ) 修正了大量的异形词、错别字。

<br>

## 精简字表

原版字表 17K+ 的字，而《通用规范汉字表》才只收录了 8K 多个字。

如果不是文字工作者，其实 3500 字就够用了。

-   `pinyin_simp_3500` 《通用规范汉字表》的第一级 3500 常用字
-   `pinyin_simp_gb2312` GB2312 6763个字
-   `pinyin_simp_8105` 《通用规范汉字表》 8105 字
-   `pinyin_simp` 原版袖珍简化字词库，大约一万七千个字左右

<br>

## 其他

在  `custom_phrase.txt` 中可以设置某些字词永远只出现在前 N 个候选项，但是这样设置之后，这些字词就不能与正常的字共同造词。现在不知道如何能完美的固定某些字词的候选项顺序。  



