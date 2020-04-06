# 实验2  



## 一.实验过程  

### 安装asciinema

```sudo apt-add-repository ppa:zanchey/asciinema```

```sudo apt-get update```

```sudo apt-get install asciinema```

### 操作录像

Lesson1&2 [链接](https://asciinema.org/a/3MtXKodEieCDIIaJmylgHPTCp)

Lesson3&4 [链接](https://asciinema.org/a/E1THfHOaRB9RFgcFbj0B6aTyB)

Lesson567 [链接](https://asciinema.org/a/xId1yKSlyBSPjlqhxTiXI9QVH)  



## 二.自查清单

- 你了解vim有哪几种工作模式？
  - Normal
  - Insert
  - Visual
  - Replace
  - Compatible

- Normal模式下，从当前行开始，一次向下移动光标10行的操作方法？如何快速移动到文件开始行和结束行？如何快速跳转到文件中的第N行？
  - ```10j```
  - ```gg```   ```G```
  - ```NG```

- Normal模式下，如何删除单个字符、单个单词、从当前光标位置一直删除到行尾、单行、当前行开始向下数N行？
  - ```x```
  - ```dw```
  - ```d$```
  - ```dd```
  - ```Ndd```

- 如何在vim中快速插入N个空行？如何在vim中快速输入80个-？
  - ```No```
  - ```80i-```

- 如何撤销最近一次编辑操作？如何重做最近一次被撤销的操作？
  - ```u```
  - ```Ctrl-r```

- vim中如何实现剪切粘贴单个字符？单个单词？单行？如何实现相似的复制粘贴操作呢？
  - 剪切用```d```，复制用```y```，粘贴用```p```
  - 多行先可以先用```v```选中

- 为了编辑一段文本你能想到哪几种操作方式（按键序列）？
  - ```a```
  - ```i```
  - ```ce```
  - ```cw```

- 查看当前正在编辑的文件名的方法？查看当前光标所在行的行号的方法？
  - ```Ctrl-g```

- 在文件中进行关键词搜索你会哪些方法？如何设置忽略大小写的情况下进行匹配搜索？如何将匹配的搜索结果进行高亮显示？如何对匹配到的关键词进行批量替换？
  - ```/```和```?```
  - ```:set ic```
  - ```:set hls is```
  - ```:s/old/new/g```

- 在文件中最近编辑过的位置来回快速跳转的方法？
  - ```Ctrl-i```和```Ctrl-o```

- 如何把光标定位到各种括号的匹配项？例如：找到(, [, or {对应匹配的),], or }
  - 光标移至括号处```%```

- 在不退出vim的情况下执行一个外部程序的方法？
  - ```:![external]```

- 如何使用vim的内置帮助系统来查询一个内置默认快捷键的使用方法？如何在两个不同的分屏窗口中移动光标？
  - ```help [key]```
  - ```Ctrl-w```