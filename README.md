- [1.Markdown是什么?](#1markdown是什么)
- [2.谁创造了它?](#2谁创造了它)
- [3.为什么要使用它?](#3为什么要使用它)
- [4.怎么使用?](#4怎么使用)
  - [4.1标题](#41标题)
  - [4.2段落](#42段落)
  - [4.3区块引用](#43区块引用)
  - [4.4代码区块](#44代码区块)
  - [4.5强调](#45强调)
  - [4.6列表](#46列表)
  - [4.7分割线](#47分割线)
  - [4.8链接](#48链接)
  - [4.9图片](#49图片)
  - [4.10反斜杠 `\`](#410反斜杠-)
  - [4.11符号 '`'](#411符号-)
  - [4.12表格](#412表格)
# 1.Markdown是什么?
Markdown是一种轻量级**标记语言**,它以纯文本形式(易读、易写、易更改)编写文档,并最终以HTML格式发布.
Markdown也可以理解为将以MARKDOWN语法编写的语言转换成HTML内容的工具.
# 2.谁创造了它?
它由Aaron Swartz和John Gruber共同设计,Aaron Swartz就是那位于2013年1月11日自杀,有着开挂一般人生经历的程序员.维基百科对他的介绍是:**软件工程师/作家/政治组织者/互联网活动家/维基百科人**.
![Aaron_Swartz](https://www.justyao.ga/?/images/2020/08/17/ql8WUptNJk/Aaron_Swartz.jpg)
# 3.为什么要使用它?
- 它是易读(看起来舒服)/易写(语法简单)/易更改**纯文本**.处处体现着**极简主义**的影子.
- 兼容HTML,可以转换为HTML格式发布.
- 跨平台使用.
- 越来越多的网站支持Markdown.
- 更方便清晰地组织你的电子邮件.(Markdown-here,Airmail)
# 4.怎么使用?
Markdown语法主要分为如下几大部分:**标题/段落/区块引用/代码区块/强调/列表/分割线/链接/图片/反斜杠 \/符号'`'**.
## 4.1标题
标题有两种形式:
- 使用`=`和`-`标记一级标题和二级标题
示例:
```
一级标题
=========
二级标题
---------
```
效果:
>一级标题
>=========
>二级标题
>---------
- 使用`#`,可以表示1-6级标题.
示例:
```
# 这是一级标题
## 这是二级标题
### 这是三级标题
#### 这是四级标题
##### 这是五级标题
###### 这是六级标题
```
效果:
># 这是一级标题
>## 这是二级标题
>### 这是三级标题
>#### 这是四级标题
>##### 这是五级标题
>###### 这是六级标题

## 4.2段落
段落的前后要有空行,所谓的空行是指没有文字内容.若想在段内强制换行的方式是使用**两个以上**空格加上回车(引用中换行省略回车).

示例:
```
这里是第一段.
直接回车换行.

这里是第一段.  
段内强行换行.

这里是第一段.

空一行换行.
```
>这里是第一段.
>直接回车换行.
>
>这里是第一段.  
>段内强行换行.
>
>这里是第一段.
>
>空一行换行.
## 4.3区块引用
在段落的每行或者只在第一行使用符号`>`,还可使用多个嵌套引用.

示例:
```
>区块引用
>>嵌套引用
```
效果:
>区块引用
>>嵌套引用

## 4.4代码区块
代码之间分别用三个反引号包起来,且两边的反引号单独占一行.  
如果要使代码块支持不同代码的高亮,需要在第一行的反引号后加上标记:

示例:
```
```java
public static void main(String[] args){
    System.out.println("Hello World");
}
```-
```
效果:
>```java
>public static void main(String[] args){
>    System.out.println("Hello World");
>}
>```
## 4.5强调
在强调内容两侧分别加上`*`或者`_`.

示例:
```
*斜体*,_斜体_
**粗体**,__粗体__
```
效果:
*斜体*,_斜体_
**粗体**,__粗体__
## 4.6列表
使用`·`/`+`/`-`标记无序列表,标记后面最少有一个**空格**或者**制表符**.若不在引用区块中,必须和前方段落之间存在空行.

示例:
```
- 第一项
- 第二项
- 第三项

+ 第一项
+ 第二项
+ 第三项

1. 第一项
2. 第二项
3. 第三项
```
效果:
>- 第一项
>- 第二项
>- 第三项
>
>+ 第一项
>+ 第二项
>+ 第三项
>
>1. 第一项
>2. 第二项
>3. 第三项
## 4.7分割线
分割线最常使用就是三个或以上`*`还可以使用`-`和`_`
示例:
```
第一行
***
第二行
```
结果:
>第一行
>***
>第二行
## 4.8链接
连接可以由两种形式生成:**行内式**和**参考式**
- 行内式
示例:
```
[潜龙云博客](https://blogs.qianlongyun.cn/ "潜龙云")
```
结果:
>[潜龙云博客](https://blogs.qianlongyun.cn/ "潜龙云")
- 参考式(有的编辑器不支持)
示例:
```
[潜龙云博客][1]
[潜龙云博客][2]
[1]:https://blogs.qianlongyun.cn/ "潜龙云"
[2]:https://blogs.qianlongyun.cn/ "潜龙云"
```
结果:
>[潜龙云博客][1]
>[潜龙云博客][2]
>[1]:https://blogs.qianlongyun.cn/ "潜龙云"
>[2]:https://blogs.qianlongyun.cn/ "潜龙云"
## 4.9图片
添加图片的形式和链接相似,只需在链接的基础上前方加一个!.
示例:
```
![图片alt](图片地址 ''图片title'')

图片alt就是显示在图片下面的文字，相当于对图片内容的解释。
图片title是图片的标题，当鼠标移到图片上时显示的内容。title可加可不加

![博客官网入口](https://blogs.qianlongyun.cn/wp-content/uploads/2020/04/%E5%8D%9A%E5%AE%A2%E5%AE%98%E7%BD%91%E5%85%A5%E5%8F%A3.jpg "博客官网入口")
```
结果:
>![博客官网入口](https://blogs.qianlongyun.cn/wp-content/uploads/2020/04/%E5%8D%9A%E5%AE%A2%E5%AE%98%E7%BD%91%E5%85%A5%E5%8F%A3.jpg "博客官网入口")
## 4.10反斜杠 `\`
相当于`反转义`作用.使符号成为普通符号.
示例:
```
\*反转义测试\*
```
结果:
>\*反转义测试\*
## 4.11符号 '`'
起标记作用
示例:
```
`Alt+F4`
```
效果:
>`Alt+F4`
## 4.12表格(非traditonal markdown)但是大多都支持
用`| `表示表格纵向标记,表头和表内容用`-`隔开,并可用`:`进行对齐设置,两边都有`:`则表示居中,若不加`:`则默认左对齐
示例:
```
| 姓名| 排行| 
| --| --:| 
| 刘备| 大哥| 
| 关羽| 二哥| 
| 张飞| 三弟| 
```
结果:
>| 姓名| 排行| 
>| -| --:| 
>| 刘备| 大哥| 
>| 关羽| 二哥| 
>| 张飞| 三弟| 
# 4.13目录(非traditonal markdown)
[toc]  
许多编辑器不支持,这里不做讨论.
# 附录
MarkDown代码块高亮支持语言
| language | key | 
| :------------: | :------------: | 
| 1C | 1c |
| ActionScript| actionscript |
| Apache| apache |
| AppleScript| applescript |
| AsciiDoc| asciidoc |
| AspectJ| asciidoc |
| AutoHotkey| autohotkey |
| AVR Assembler| avrasm |
| Axapta| axapta |
| Bash| bash |
| BrainFuck| brainfuck |
| Cap’n Proto| capnproto |
| Clojure REPL| clojure |
| Clojure| clojure |
| CMake| cmake |
| CoffeeScript| coffeescript |
| C++| cpp |
| C#| cs |
| CSS| css |
| D| d |
| Dart| d |
| Delphi| delphi |
| Diff| diff |
| Django| django |
| DOS.bat| dos |
| Dust| dust |
| Elixir| elixir |
| ERB(Embedded Ruby)| erb |
| Erlang REPL| erlang-repl |
| Erlang| erlang |
| FIX| fix |
| F#| fsharp |
| G-code(ISO 6983)| gcode |
| Gherkin| gherkin |
| GLSL| glsl |
| Go| go |
| Gradle| gradle |
| Groovy| groovy |
| Haml| haml |
| Handlebars| handlebars |
| Haskell| haskell |
| Haxe| haxe |
| HTML| html |
| HTTP| http |
| Ini file| ini |
| Java| java |
| JavaScript| javascript |
| JSON| json |
| Lasso| lasso |
| Less| less |
| Lisp| lisp |
| LiveCode| livecodeserver |
| LiveScript| livescript |
| Lua| lua |
| Makefile| makefile |
| Markdown| markdown |
| Mathematica| mathematica |
| Matlab| matlab |
| MEL (Maya Embedded Language)| mel |
| Mercury| mercury |
| Mizar| mizar |
| Monkey| monkey |
| Nginx| nginx |
| Nimrod| nimrod |
| Nix| nix |
| NSIS| nsis |
| Objective C| objectivec |
| OCaml| ocaml |
| Oxygene| oxygene |
| Parser 3| parser3 |
| Perl| perl |
| PHP| php |
| PowerShell| powershell |
| Processing| processing |
| Python’s profiler output| profile |
| Protocol Buffers| protobuf |
| Puppet| puppet |
| Python| python |
| Q| q |
| R| r |
| RenderMan RIB| rib |
| Roboconf| roboconf |
| RenderMan RSL| rsl |
| Ruby| ruby |
| Oracle Rules Language| ruleslanguage |
| Rust| rust |
| Scala| scala |
| Scheme| scheme |
| Scilab| scilab |
| SCSS| scss |
| Smali| smali |
| SmallTalk| smalltalk |
| SML| sml |
| SQL| sql |
| Stata| stata |
| STEP Part21(ISO 10303-21)| step21 |
| Stylus| stylus |
| Swift| swift |
| Tcl| tcl |
| Tex| tex |
| text| text/plain |
| Thrift| thrift |
| Twig| twig |
| TypeScript| typescript |
| Vala| vala |
| VB.NET| vbnet |
| VBScript in HTML| vbscript-html |
| VBScript| vbscript |
| Verilog| verilog |
| VHDL| vhdl |
| Vim Script| vim |
| Intel x86 Assembly| x86asm |
| XL| xl |
| XML| xml |
| YAML| yml |
