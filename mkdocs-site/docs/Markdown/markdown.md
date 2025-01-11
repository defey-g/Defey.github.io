#**<font color = 'green'>Markdown 笔记</font>**

##**<font color = 'purple'>语法:</font>**
- **标题:**

    !!! note "书写方法:"

            # 一级标题
            ## 二级标题
            ### 三级标题
            #### 四级标题
            ##### 五级标题
            ###### 六级标题

- **字体样式:** 

	1. *斜体*

	    !!! note "书写方法:"

				*斜体*

	2. **文字加粗**

		!!! note "书写方法:"
				
				**文字加粗**

- **链接:** 

	[<u>**这是百度链接**</u>](https://www.baidu.com/)
    [Baidu](https://www.baidu.com/){ .md-button }
    [:fontawesome-solid-paper-plane:](https://www.baidu.com/){ .md-button }
    [:fontawesome-solid-paper-plane:](https://www.baidu.com/){ .md-button .md-button--primary }

	!!! note "书写方法:"

		    [<u>**这是百度链接**</u>](https://www.baidu.com/)
            [百度链接](https://www.baidu.com/){ .md-button }
            [:fontawesome-solid-paper-plane:](https://www.baidu.com/){ .md-button }
            [:fontawesome-solid-paper-plane:](https://www.baidu.com/){ .md-button .md-button--primary }


- **图标样式 Icon:**

    :simple-animalplanet:
    :material-animation-play:
    :simple-fox:
    :fontawesome-solid-box:
    :fontawesome-brands-xbox:
    :material-firefox:
    :material-mouse:
    :material-lighthouse:
    :material-pig:
    :material-pig-variant:
    :material-login:
    :material-form-textbox-password:
    :material-deathly-hallows:
    :octicons-heart-fill-24:{ .heart }
    :smile:{ .heart }
    :material-rabbit:{ .heart }
    :fontawesome-solid-piggy-bank:{ .heart }
    :clown:{ .heart }


- **无序列表:**

	- 无序列表1
	- 无序列表2
	- 无序列表3

	!!! note "书写方法:"

            - 无序列表1
            - 无序列表2
            - 无序列表3

- **有序列表:**
	1. 有序列表1
	2. 有序列表2
	3. 有序列表3

	!!! note "书写方法:"

            1. 有序列表1
            2. 有序列表2
            3. 有序列表3

- **表格:**

	|表格1|表格2|
	|:-:|:-:|
	|内容1|内容2|
	|内容3|内容4|

    !!! note "书写方法"
        ```
        |表格1|表格2|
        |:-:|:-:|
        |内容1|内容2|
        |内容3|内容4|
        ```

---

##<font color = purple >辅助内容 :octicons-heart-fill-24: :</font>

- **引入文字**
 > 引入文字

	    > 引入文字


- **特殊标记:**

    `特殊标记`

		`特殊标记`

- **代码块区域**

    ```yaml { .yaml .no-copy .annotate }
    nav:
        - Home: index.md
        - Learning Note: 
        # - Markdown: Markdown/markdown.md
        # - HTML: HTML/html.md

    ```

    ```json
    {
    "key": "value "
    }
    ```

    ``` py title="bubble_sort.py" linenums="1" hl_lines="2 3"
    def bubble_sort(items):
        for i in range(len(items)):
            for j in range(len(items) - 1 - i): #注释
                if items[j] > items[j + 1]:
                    items[j], items[j + 1] = items[j + 1], items[j]
    ```
    The `#!python range()` function is used to generate a sequence of numbers.


- **脚注[^1]**

    !!! note "脚注的使用方法:"

        脚注内容必须使用与引用相同的标识符声明。它可以插入到文档中的任意位置，并且始终呈现在页面底部。此外，会自动添加指向脚注参考的反向链接。[^2]

    [^1]: 这是一个短脚注，短脚注可以写在同一行.
    [^2]: 
        这是一个段落脚注
        段落可以写在下一行，并且必须缩进四个空格

- **格式化  "^、==、~ "**

    ^^This was inserted^^

    ==This was marked==

    ~~This was deleted~~

    H~2~0

    A^T^A

    Text can be ~~deleted~~ and replacement text ^^added^^. This can also be
    combined into ~~one~~ ==a single== operation. ==Highlighting== is also
    possible and comments can be added inline.

        Formatting can also be applied to blocks by putting the opening and closing
        tags on separate lines and adding new lines between the tags and the content.

    ++ctrl+alt+del++

- **各种提示框:**

    !!! note "注意"

        这里面的>这五个只是为了不让代码生效，在写代码块区域的时候不需要写，写法是去掉>这五个之后剩下的内容。这六个小点(`)也是英文状态下的Tab键上面的那个按钮.
        网页显示未生效，实际效果与显示不同

    ???+ note "可以折叠提示"
        这是一个可折叠的提示

    !!! tip
        tip 提示框书写方法 : "!!! tip".

        这是一个在css 修改过的 提示框

    !!! abstract
        abstract 提示框书写方法 : "!!! abstract".

    !!! success
        success 提示框书写方法 : "!!! success".

    !!! warning
        warning 提示框书写方法 : "!!! warning".

    !!! pied-piper "Pied Piper"

        === "Tip1"
            ```
            css 中自定义的 Pied Piper 提示框
            ```
        === "Tip2"
            ```
            css 中自定义的 Pied Piper 提示框2
            ```
    === "C"

        ``` c
        #include <stdio.h>

        int main(void) {
        printf("Hello world!\n");
        return 0;
        }
        ```

    === "C++"

        ``` c++
        #include <iostream>

        int main(void) {
        std::cout << "Hello world!" << std::endl;
        return 0;
        }
        ```

    !!! info 
        这是一个info 提示框

        其他可用类型还有 "question","failure","danger","bug","example","quote"

    !!! info inline
        提示框书写方法 : "!!! info inline".

    !!! info inline end "Lorem ipsum end"
        提示框书写方法 : "!!! info inline end".

    > 中间内容