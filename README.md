# 自用 Rime 配置

![demo](./demo.jpg)



## 基本套路：

-   Squirrel 0.15.0 简中全拼
-   0.15.0 后 `charset_filter@gb2312`失效，放弃了朙月拼音方案，直接使用袖珍简化字方案 [rime](https://github.com/rime)/**[rime-pinyin-simp](https://github.com/rime/rime-pinyin-simp)**
-   8105 简体字，去除大量生僻字 [placeless](https://github.com/placeless)/**[squirrel_config](https://github.com/placeless/squirrel_config)** （太太太太感谢了！要没这个我还在用 0.14.0）
-   简型八股文模型 [lotem](https://github.com/lotem)/**[rime-octagram-data/tree/hans](https://github.com/lotem/rime-octagram-data/tree/hans)**
-   英文输入方案 Easy English Nano [mityliu](https://github.com/mityliu)/**[rime-custom](https://github.com/mityliu/rime-custom)**
-   中英混输词库 <瑾昀 <cokunhui@gmail.com>>
-   袖珍方案输出繁体，参考了五笔的简入繁出 [rime/home/issues#388](https://github.com/rime/home/issues/388#issuecomment-504572224) 
-   搜狗两百万词库 [liuour](https://github.com/liuour)/**[rime](https://github.com/liuour/rime)**
-   中文维基词库 [felixonmars](https://github.com/felixonmars)/**[fcitx5-pinyin-zhwiki](https://github.com/felixonmars/fcitx5-pinyin-zhwiki)**
-   动态日期、时间、星期 [KyleBing](https://github.com/KyleBing)/**[rime-wubi86-jidian](https://github.com/KyleBing/rime-wubi86-jidian)**
-   所有标点符号直接上屏，并将「/」模式改为「v」模式
-   增加了 `opencc/` 键盘符号映射，删除了 emoji 映射，如需要 emoji 可参考  [liuour](https://github.com/liuour)/**[rime](https://github.com/liuour/rime)**
-   symbols 改为简体字（如节气、八卦），增加一些自定义符号
-   常用全拼自动纠错：`ni tina tain do zia gna she me` → `你天天都在干什么. 

  

## 精简字库

-   `pinyin_simp_3500` 《通用规范汉字表（2013）》的第一级 3500 常用字
-   `pinyin_simp_8105` [placeless](https://github.com/placeless)/**[squirrel_config](https://github.com/placeless/squirrel_config)** 的 8105 简体字
-   `pinyin_simp_gb2312` GB2312 6763个字
-   `dicts/pinyin_simp` 原版袖珍简化字词库，大约一万七千个字左右

已经用了 [placeless](https://github.com/placeless)/**[squirrel_config](https://github.com/placeless/squirrel_config)** 的 8105 简体字了，不过生僻字比我之前用 GB2312 的时候要多，就又弄了一个 GB2312 的精简版，干脆再弄了一个 3500 常用字。  

  

### 删减字库的优缺点：

生僻字没了，选字方便了许多，但是偶尔偶尔遇到的生僻字无法打出来。

切换字库要重新部署才行，不知道要怎么样才能像以前切换字符集那样切换字库，谁要知道求告知。

把这些词库都放上了，可以自己选择。  

  

精简字库比较方便的地方：

比如「丞」字不在 3500 里面，但是扩展词库里有「丞相」这个词，也是可以打出来的。

这个需要扩展词库包含大量词汇，并且带拼音。（不带拼音打不出来）  

   


## 详细说明

[我的 Rime 配置 2021](https://dvel.xyz/post/30/)

