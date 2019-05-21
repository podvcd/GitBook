# 第2节：语法

# Gitbook 语法：标题

使用标题有两种方法，第一种是使用 "#" 开头，第二种是打完文字后在下一行加上 "==" 符号

- 使用 "#"

  ```bash
  #第一层标题
  ##第二层标题
  ###第三层标题
  ####第四层标题
  #####第五层标题
  ```

  # 第一层标题

  ## 第二层标题

  ### 第三层标题

  #### 第四层标题

  ##### 第五层标题



- 使用 "=="

  ```bash
  第一层标题
  ==
  第二层标题
  --
  ```

  # 第一层标题

  ## 第二层标题



# Gitbook 語法：強調

在這边会有三种强调的方式

- 斜体，使用 "*" 或 "_" 將文字包起来

  ```bash
  *强调，這是斜体*
  
  _强调，這也是斜体_
  ```

  *强调，這是斜体*

  *强调，這也是斜体*

- 粗体，使用 "**" 或 "__" 將文字包起起來

  ```bash
  **強調，這是粗体**
  
  __强调，這也是粗体__
  ```

  **强调，這是粗体**

  **强调，這也是粗体**

- 粗斜体，使用 "***" 或 "*_*" 将文字包起起來

  ```bash
  ***强调，這是粗斜体***
  
  ___强调，這也是粗斜体___
  ```

  **强调，這是粗斜体**

  **强调，這也是粗斜体**

# Gitbook 语法：清单

清单可分为数字清单及項目清单两种，可以使用縮排进行显示，需要注意的地方为不同层级的部份需要多空一行

- 数字清单，在前面使用 "数字. " 开头，在测试过程中发现数字清单只能到第二层，再細分下去排版会乱掉

  ```bash
  1. 這是数字清单 1
  
   1.1. 這是数字清单 1.1
  
  2. 這是数字清单 2
  3. 這是数字清单 3
  ```

  1. 这是数字清单 1

     1.1. 这是数字清单

  2. 这是数字清单 2

  3. 这是数字清单 3

- 项目清单，在前面使用 "-" 或 "+" 开头，可以混用

  ```bash
  - 這是項目清單 1
  
   - 這是項目清單 1-1
  
     - 這是項目清單 1-1-1
  
  + 這是項目清單 2
  - 這是項目清單 3
  ```

  - 這是項目清單 1
    - 這是項目清單 1-1
      - 這是項目清單 1-1-1
  - 這是項目清單 2
  - 這是項目清單 3

# Gitbook 语法：链接

在使用链接部份也有两种方法可以进行

- 使用"[显示文字](http://cowmanchiang.me/gitbook/gitbook/contents/how/链接)"进行

  ```bash
  [Link](http://cowmanchiang.me/gitbook)
  ```

  [Link](http://cowmanchiang.me/gitbook)

- 使用注解方式进行 (示范语法中以 "【 】" 取代 "[ ]" 以免发生误判)

  ```bash
  【Link】【1】
  
  【1】: http://cowmanchiang.me/gitbook
  ```

  [Link](http://cowmanchiang.me/gitbook)

# Gitbook 语法：图片

插入图片的方法会跟前一节 [链接](http://cowmanchiang.me/gitbook/gitbook/contents/how/links.html) 很像，差別只在於最前面多了一個 "!" 符号，或是可使用 HTML 內嵌的方式進行

- 使用'!【图片提示文字】(图片連結)'進行 (示范语法中以 "【 】" 取代 "[ ]" 以免发生误判)

  ```bash
  ![Cowman](../images/77326.jpg)
  ```

  ![Cowman](http://cowmanchiang.me/gitbook/gitbook/contents/images/77326.jpg)

- 使用注解方式进行 (示范语法中以 "【 】" 取代 "[ ]" 以免发生误判)

  ```bash
  !【Cowman】【1】
  
  【1】: ../images/77326.jpg
  ```

  ![Cowman](http://cowmanchiang.me/gitbook/gitbook/contents/images/77326.jpg)

- 使用 HTML 內嵌

  ```bash
  <img src="../images/77326.jpg" alt="Cowman" width="240" height="180" border="10" />
  ```

  ![Cowman](http://cowmanchiang.me/gitbook/gitbook/contents/images/77326.jpg)

# Gitbook 语法：代码

在代码语法显示部份也是有两种方式可以进行标示

- 使用"8個空格"缩排

  ```bash
         ls -al
  ```

  ```
  ls -al
  ```

- 使用 " '''[code language] " (以 " ''' " 取代 " ``` " 避免排版错乱) 推荐此标示方法，支持代码 highlight 显示，支持哪些语言请参考 [highlightjs.org](https://highlightjs.org/static/demo/)

  ```bash
  '''bash
  ls -al
  '''
  ```

  ```bash
  ls -al
  ```

# Gitbook 语法：表格

绘制表格的方式使用 "|" 进行分隔，在使用 "-" 标示出表格Title

```bash
name | id | code
- | - | -
gitbook | 1 | nodejs
wordpress | 2 | php
```

| name      | id   | code   |
| --------- | ---- | ------ |
| gitbook   | 1    | nodejs |
| wordpress | 2    | php    |

# Gitbook 语法：內嵌 HTML

可以在 Markdown 中使用 HTML 语法来辅助显示的效果，例如置中、字体颜色、iframe 等

```bash
居中
<center>居中</center>
<font color="red">红色字体</font>
```

未居中



<center>居中</center>



<font color="red">红色字体</font>

# Gitbook 语法：Youtube

在 Gitbook 官方手冊中介绍的范例是使用链接的方式导入 Youtube 网页中

```bash
<a href="http://www.youtube.com/watch?feature=player_embedded&v=YOUTUBE_VIDEO_ID_HERE
" target="_blank"><img src="../images/youtube.png" width="250"
alt="IMAGE ALT TEXT HERE" /></a>
```

[![IMAGE ALT TEXT HERE](http://cowmanchiang.me/gitbook/gitbook/contents/images/youtube.png)](http://www.youtube.com/watch?feature=player_embedded&v=YOUTUBE_VIDEO_ID_HERE)

另外也可以使用 iframe 的方式將 Youtube 影片嵌进来

```bash
<iframe width="560" height="315" src="//www.youtube.com/embed/SwrKzkRUlaw?hd=1&autoplay=1&loop=1&playli
```



其它更新语法参看官方手册



## Quiz

Here's a quiz about Gitbook

Question 1 of 2

|                  | Good | Bad  |
| ---------------- | ---- | ---- |
| What is Gitbook? |      |      |

Question 2 of 2

What does Gitbook support?

-  Table-based questions with radio buttons
-  Table-based questions with checkboxes
-  Telepathy
-  List-based questions with checkboxes
-  List-based questions with radio buttons
-  Moon-on-a-stick

[Submit](http://cowmanchiang.me/gitbook/gitbook/contents/plugin/quizzes.html#)[Solution](http://cowmanchiang.me/gitbook/gitbook/contents/plugin/quizzes.html#)