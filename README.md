1. 标题设置
  * 通过在文字下方添加“=”和“-”，他们分别表示一级标题和二级标题。
  * 在文字开头加上 “#”，通过“#”数量表示几级标题。（一共只有1~6级）
# H1
## H2
###### H6

2. 块注释,通过在文字开头添加“>”表示块注释。（当>和文字之间添加五个blank时，块注释的文字会有变化。）
  >Blockquotes

  >This is a long 
  blockquotes

3. 斜体,将需要设置为斜体的文字两端使用1个“_”夹起来,_Blue_

4. 粗体,将需要设置为斜体的文字两端使用2个“_”夹起来,__Blue__

5. 无序列表,在文字开头添加(*, +, and -)实现无序列表。但是要注意在(*, +,and-)和文字之间需要添加空格。
  * Red
  + Green
  - Blue

6. 有序列表,使用数字后面跟上句号。（还要有空格）
  1. Bird
  2. McHale
  3. Parish

7. 链接（Links）
  * 内联方式：This is an [example link](http://baidu.com/).
  * 引用方式：I get 10 times more traffic from [Google][1] than from [Yahoo][2] or [MSN][3].  
    [1]: http://google.com/        "Google" 
    [2]: http://search.yahoo.com/  "Yahoo Search" 
    [3]: http://search.msn.com/    "MSN Search"

8. 图片（Images）
  *内联方式：![alt text](/path/to/img.jpg "Title")
  *引用方式：![alt text][id]
    [id]: /path/to/img.jpg "Title"

9. 代码（HTML中所谓的Code）
  * 简单文字出现一个代码框。使用`<blockquote>`。（`不是单引号而是左上角的ESC下面~中的`）
  * 大片文字需要实现代码框。使用Tab和四个空格。

10. 脚注（footnote）
  hello[^hello]
  [^hello]: hi

11. 下划线
  在空白行下方添加三条“-”横线。
