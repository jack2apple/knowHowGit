1. ???置（?字体?大，和word的??意思一?）
在Markdown当中?置??，有??方式：
第一?：通?在文字下方添加“=”和“-”，他?分?表示一???和二???。
第二?：在文字??加上 “#”，通?“#”数量表示几???。（一共只有1~6???，1???字体最大）
# H1
## H2
###### H6

2. ?注?（blockquote）
通?在文字??添加“>”表示?注?。（当>和文字之?添加五个blank?，?注?的文字会有?化。）
> Blockquotes
> Blockquotes

> This is a long 
blockquotes

3. 斜体
将需要?置?斜体的文字?端使用1个“*”或者“_”?起来
* Red *
+ Green +
- Blue -

4. 粗体
将需要?置?斜体的文字?端使用2个“*”或者“_”?起来
** Red **
++ Green ++
-- Blue --

5. 无序列表
在文字??添加(*, +, and -)??无序列表。但是要注意在(*, +, and -)和文字之?需要添加空格。（建?：一个文档中只是用一?无序列表的表示方式）
* Red
* Green
* Blue

+ Red
+ Green
+ Blue

- Red
- Green
- Blue

6. 有序列表
使用数字后面跟上句号。（?要有空格）
1. Bird
2. McHale
3. Parish

7. ?接（Links）
Markdown中有??方式，???接，分??内?方式和引用方式。

内?方式：This is an [example link](http://example.com/).
引用方式：
I get 10 times more traffic from [Google][1] than from [Yahoo][2] or [MSN][3].  

[1]: http://google.com/        "Google" 
[2]: http://search.yahoo.com/  "Yahoo Search" 
[3]: http://search.msn.com/    "MSN Search"

8. ?片（Images）
?片的?理方式和?接的?理方式，非常的?似。
内?方式：![alt text](/path/to/img.jpg "Title")
引用方式：
![alt text][id]
[id]: /path/to/img.jpg "Title"

9. 代?（HTML中所?的Code）
??方式有??：
第一?：??文字出?一个代?框。使用`<blockquote>`。（`不是?引号而是左上角的ESC下面~中的`）
第二?：大片文字需要??代?框。使用Tab和四个空格。

10. 脚注（footnote）
??方式如下：
hello[^hello]


[^hello]: hi

11. 下??
在空白行下方添加三条“-”横?。（前面??在文字下方添加“-”，??的2???）
