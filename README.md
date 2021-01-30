# Rime

配置基础源自：[liuour](https://github.com/liuour)/**[rime](https://github.com/liuour/rime)** （感谢！）



输入方案为 luna_pinyin_simp，使用的主要词库为 luna_pinyin。



字符集过滤使用了 GB2312，这样大大减少了生僻字的出现。

但同时也增加了切换繁体的步骤，需要先切换到扩展字符集，再切换到繁体才能输入繁体字。

不过对于很少用繁体字输入的人来说没什么影响。



## 主要功能：

-   删除了 emoji、颜文字
-   删除了如书名号等符号的候选功能，直接上屏
-   取消了 “/” 模式的各种附加功能
-   创了个落格输入法的暗色皮肤
-   扩展词库归类到文件夹里
-   快捷键与官方示例同步，主要是调出 tab 切换光标、快速切换简繁的功能 [rime](https://github.com/rime)/**[rime-prelude](https://github.com/rime/rime-prelude)** （官方示例）
-   默认使用 gb2312 字符集过滤
-   将 easy_en 替换为 Easy English Nano，参考于 [mityliu](https://github.com/mityliu)/**[rime-custom](https://github.com/mityliu/rime-custom)** （感谢！）
-   增加了常见的拼音纠错
-   保留快速输入日期时间的小功能
-   一些小细节



## 配置文件：

-   `squirrel.custom.yaml`
    -   皮肤
    -   静默中文的选项
-   `default.custom.yaml` 输入法全局基础设定
    -   方案选择
    -   候选词个数
    -   按键行为
    -   快捷键绑定
-   `luna_pinyin_simp.custom.yaml` 
    -   主要设定文件，简中全拼方案的所有设定
-   `luna_pinyin.extended.dict.yaml`
    -   词库选择，此文件于 `luna_pinyin_simp.custom.yaml` 中定义



## 用户个人文件：

-   `custom_phrase.txt` 自造词
-   `installation.yaml` 

```
# 这里需要自己加入代码来完成同步用户资料的功能，如果没有或不小心删了，部署一次自动生成。
# ...
# 默认为随机的 UUID，可以起一个好记的名字
installation_id: "my computer"
# 需要手动添加下行，设定用户同步目录
sync_dir: "/Users/<your username>/Dropbox/Rime_Sync"
# ...
```

-   `*.userdb/`  各方案的用户词库



## 关于同步功能

如果同时使用两台电脑，只要使用方案一致，不必手动去合并 `*.userdb.txt` 这个用户个人词库。

点击 [重新部署]，用户设定目录 → 同步目录，单向操作。

点击 [同步用户数据]，用户设定目录 ←→ 同步目录，双向同步，Rime 会自动合并引入所有 ID 下的个人词库。

