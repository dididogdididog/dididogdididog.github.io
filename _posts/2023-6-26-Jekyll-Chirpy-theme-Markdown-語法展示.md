---
title: Jekyll Chirpy-theme Markdown 語法展示
date: 2023-06-26 +0800
categories: [Notes,Jekyll]
tags: [jekyll,chirpy,markdown]     # TAG names should always be lowercase
math: true
img_path: /assets/img/20230626/
---

## 標題(Headings)
---

## 主標題

```markdown
## 主標題
```

### 副標題

```markdown
### 副標題
```
## 段落(Paragraph)
---
Quisque egestas convallis ipsum, ut sollicitudin risus tincidunt a. Maecenas interdum malesuada egestas. Duis consectetur porta risus, sit amet vulputate urna facilisis ac. Phasellus semper dui non purus ultrices sodales. Aliquam ante lorem, ornare a feugiat ac, finibus nec mauris. Vivamus ut tristique nisi. Sed vel leo vulputate, efficitur risus non, posuere mi.

這是中文的段落，我不知道要寫什麼所以隨便亂打。這是中文的段落，我不知道要寫什麼所以隨便亂打。這是中文的段落，我不知道要寫什麼所以隨便亂打。這是中文的段落，我不知道要寫什麼所以隨便亂打。

## 分隔線(Divider)
---
用`---`表示分隔線。

## 清單(Lists)
---
### 有序清單(Ordered List)
1. 第一項
2. 第二項
3. 第三項

```markdown
1. 第一項
2. 第二項
3. 第三項
```

### 無序清單(Unordered List)
- First item
- Second item
- Third item
  - Indented item
  - Indented item
- Fourth item

```markdown
- First item
- Second item
- Third item
  - Indented item
  - Indented item
- Fourth item
```

### 待辦清單(Todo List)
---
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

```markdown
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```

### 定義清單(Definition List)
---
Sun
: the star around which the earth orbits

Moon
: the natural satellite of the earth, visible by reflected light from the sun

```markdown
Sun
: the star around which the earth orbits

Moon
: the natural satellite of the earth, visible by reflected light from the sun
```

## 跳脫字元(Escape Character)
>在要插入的符號前加入反斜線\\。

## 換行(Line Break)
>換行最常見的有兩種方法，第一種是在句尾加上兩個以上的空格，第二種方法是在句尾加上\<br>標籤。

這是一行文字。  
這是下一行文字。

這是一行文字。<br>
這是下一行文字。

```markdown
這是一行文字。  
這是下一行文字。

這是一行文字。<br>
這是下一行文字。
```

## 引用(Block Quote)
---
>This line shows the block quote.  
>這行繼續

>This line shows the block quote.
>
>這行繼續

```markdown
>This line shows the block quote.  
>這行繼續

>This line shows the block quote.
>
>這行繼續
```

## 字體(Texts)
---
*斜體字*   
**粗體字**  
***斜粗體***  
_斜體字2_  
__粗體字2__  
___斜粗體2___  
~~刪除線~~  
正常<sup>上標</sup>  
正常<sub>下標</sub>  
<u>底線++</u>  
<mark>螢光標記</mark>  
<mark style="background-color: lightblue">螢光標記</mark>  
<span style="color:red">紅色的字</span>  
`Inline block`

```markdown
*斜體字*   
**粗體字**  
***斜粗體***  
_斜體字2_  
__粗體字2__  
___斜粗體2___  
~~刪除線~~  
正常<sup>上標</sup>  
正常<sub>下標</sub>  
<u>底線++</u>  
<mark>螢光標記</mark>  
<mark style="background-color: lightblue">螢光標記</mark>  
<span style="color:red">紅色的字</span>  
`Inline block`
```

## 提示(Prompts)
---
> An example showing the `tip` type prompt.
{: .prompt-tip }

> An example showing the `info` type prompt.
{: .prompt-info }

> An example showing the `warning` type prompt.
{: .prompt-warning }

> An example showing the `danger` type prompt.
{: .prompt-danger }

```markdown
> An example showing the `tip` type prompt.
{: .prompt-tip }

> An example showing the `info` type prompt.
{: .prompt-info }

> An example showing the `warning` type prompt.
{: .prompt-warning }

> An example showing the `danger` type prompt.
{: .prompt-danger }
```

## 表格(Tables)
---

| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

```markdown
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |
```

## 連結(Links)
---
<https://www.youtube.com/>

This site was built using [GitHub Pages](https://pages.github.com/).

```markdown
<https://www.youtube.com/>

This site was built using [GitHub Pages](https://pages.github.com/).
```

## 註腳(Footnote)
---
Click the hook will locate the footnote[^1], and here is another footnote[^2].

[^1]: The footnote source
[^2]: The 2nd footnote source

```
Click the hook will locate the footnote[^1], and here is another footnote[^2].

[^1]: The footnote source
[^2]: The 2nd footnote source
```
## 檔案路徑(Filepath)
---
Here is the `/path/to/the/file.extend`{: .filepath}.

```markdown
Here is the `/path/to/the/file.extend`{: .filepath}.
```

## 程式碼(Code Block)
---
### 指定程式碼

rouge支援的程式碼[有這些](https://rouge-ruby.github.io/docs/file.Languages.html)。

```bash
if [ $? -ne 0 ]; then
  echo "The command was not successful.";
  #do the needful / exit
fi;
```

````markdown
```bash
程式碼
```
````
### 指定檔案路徑

```sass
@import
  "colors/light-typography",
  "colors/dark-typography";
```
{: file='_sass/jekyll-theme-chirpy.scss'}

````markdown
```sass
程式碼
```
{: file='_sass/jekyll-theme-chirpy.scss'}
````

## 數學(Mathematics)

The mathematics powered by [**MathJax**](https://www.mathjax.org/):

$$ \sum_{n=1}^\infty 1/n^2 = \frac{\pi^2}{6} $$

When $a \ne 0$, there are two solutions to $ax^2 + bx + c = 0$ and they are

$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$

> 記得在front matter加上 `math: true`
{: .prompt-tip }

## 圖片(Images)
---
### Default

![dididog](didi.jpg){: w="1108" h="1477" .w-50}
_This is a caption. 這是圖片說明_

```markdown
![dididog](didi.jpg){: w="1108" h="1477" .w-50}
_This is a caption. 這是圖片說明_
```

### Left aligned

![dididog](didi.jpg){: w="1108" h="1477" .w-75 .normal}

```markdown
![dididog](didi.jpg){: w="1108" h="1477" .w-75 .normal}
```

### Float to left

![dididog](didi.jpg){: w="1108" h="1477" .w-25 .left}
Praesent maximus aliquam sapien. Sed vel neque in dolor pulvinar auctor. Maecenas pharetra, sem sit amet interdum posuere, tellus lacus eleifend magna, ac lobortis felis ipsum id sapien. Proin ornare rutrum metus, ac convallis diam volutpat sit amet. Phasellus volutpat, elit sit amet tincidunt mollis, felis mi scelerisque mauris, ut facilisis leo magna accumsan sapien. In rutrum vehicula nisl eget tempor. Nullam maximus ullamcorper libero non maximus. Integer ultricies velit id convallis varius. Praesent eu nisl eu urna finibus ultrices id nec ex. Mauris ac mattis quam. Fusce aliquam est nec sapien bibendum, vitae malesuada ligula condimentum.
Praesent maximus aliquam sapien. Sed vel neque in dolor pulvinar auctor. Maecenas pharetra, sem sit amet interdum posuere, tellus lacus eleifend magna, ac lobortis felis ipsum id sapien. Proin ornare rutrum metus, ac convallis diam volutpat sit amet. Phasellus volutpat, elit sit amet tincidunt mollis, felis mi scelerisque mauris, ut facilisis leo magna accumsan sapien. In rutrum vehicula nisl eget tempor. Nullam maximus ullamcorper libero non maximus. Integer ultricies velit id convallis varius. Praesent eu nisl eu urna finibus ultrices id nec ex. Mauris ac mattis quam. Fusce aliquam est nec sapien bibendum, vitae malesuada ligula condimentum.

```markdown
![dididog](didi.jpg){: w="1108" h="1477" .w-25 .left}
Praesent maximus aliquam sapien. Sed vel neque in dolor pulvinar auctor. Maecenas pharetra, sem sit amet interdum posuere, tellus lacus eleifend magna, ac lobortis felis ipsum id sapien. Proin ornare rutrum metus, ac convallis diam volutpat sit amet. Phasellus volutpat, elit sit amet tincidunt mollis, felis mi scelerisque mauris, ut facilisis leo magna accumsan sapien. In rutrum vehicula nisl eget tempor. Nullam maximus ullamcorper libero non maximus. Integer ultricies velit id convallis varius. Praesent eu nisl eu urna finibus ultrices id nec ex. Mauris ac mattis quam. Fusce aliquam est nec sapien bibendum, vitae malesuada ligula condimentum.
Praesent maximus aliquam sapien. Sed vel neque in dolor pulvinar auctor. Maecenas pharetra, sem sit amet interdum posuere, tellus lacus eleifend magna, ac lobortis felis ipsum id sapien. Proin ornare rutrum metus, ac convallis diam volutpat sit amet. Phasellus volutpat, elit sit amet tincidunt mollis, felis mi scelerisque mauris, ut facilisis leo magna accumsan sapien. In rutrum vehicula nisl eget tempor. Nullam maximus ullamcorper libero non maximus. Integer ultricies velit id convallis varius. Praesent eu nisl eu urna finibus ultrices id nec ex. Mauris ac mattis quam. Fusce aliquam est nec sapien bibendum, vitae malesuada ligula condimentum.
```


### Float to right

![dididog](didi.jpg){: w="1108" h="1477" .w-25 .right}
Praesent maximus aliquam sapien. Sed vel neque in dolor pulvinar auctor. Maecenas pharetra, sem sit amet interdum posuere, tellus lacus eleifend magna, ac lobortis felis ipsum id sapien. Proin ornare rutrum metus, ac convallis diam volutpat sit amet. Phasellus volutpat, elit sit amet tincidunt mollis, felis mi scelerisque mauris, ut facilisis leo magna accumsan sapien. In rutrum vehicula nisl eget tempor. Nullam maximus ullamcorper libero non maximus. Integer ultricies velit id convallis varius. Praesent eu nisl eu urna finibus ultrices id nec ex. Mauris ac mattis quam. Fusce aliquam est nec sapien bibendum, vitae malesuada ligula condimentum.
Praesent maximus aliquam sapien. Sed vel neque in dolor pulvinar auctor. Maecenas pharetra, sem sit amet interdum posuere, tellus lacus eleifend magna, ac lobortis felis ipsum id sapien. Proin ornare rutrum metus, ac convallis diam volutpat sit amet. Phasellus volutpat, elit sit amet tincidunt mollis, felis mi scelerisque mauris, ut facilisis leo magna accumsan sapien. In rutrum vehicula nisl eget tempor. Nullam maximus ullamcorper libero non maximus. Integer ultricies velit id convallis varius. Praesent eu nisl eu urna finibus ultrices id nec ex. Mauris ac mattis quam. Fusce aliquam est nec sapien bibendum, vitae malesuada ligula condimentum.

```markdown
![dididog](didi.jpg){: w="1108" h="1477" .w-25 .right}
Praesent maximus aliquam sapien. Sed vel neque in dolor pulvinar auctor. Maecenas pharetra, sem sit amet interdum posuere, tellus lacus eleifend magna, ac lobortis felis ipsum id sapien. Proin ornare rutrum metus, ac convallis diam volutpat sit amet. Phasellus volutpat, elit sit amet tincidunt mollis, felis mi scelerisque mauris, ut facilisis leo magna accumsan sapien. In rutrum vehicula nisl eget tempor. Nullam maximus ullamcorper libero non maximus. Integer ultricies velit id convallis varius. Praesent eu nisl eu urna finibus ultrices id nec ex. Mauris ac mattis quam. Fusce aliquam est nec sapien bibendum, vitae malesuada ligula condimentum.
Praesent maximus aliquam sapien. Sed vel neque in dolor pulvinar auctor. Maecenas pharetra, sem sit amet interdum posuere, tellus lacus eleifend magna, ac lobortis felis ipsum id sapien. Proin ornare rutrum metus, ac convallis diam volutpat sit amet. Phasellus volutpat, elit sit amet tincidunt mollis, felis mi scelerisque mauris, ut facilisis leo magna accumsan sapien. In rutrum vehicula nisl eget tempor. Nullam maximus ullamcorper libero non maximus. Integer ultricies velit id convallis varius. Praesent eu nisl eu urna finibus ultrices id nec ex. Mauris ac mattis quam. Fusce aliquam est nec sapien bibendum, vitae malesuada ligula condimentum.
```

## 影片(Video)
---
{% include embed/youtube.html id='6zbsUtQL4nY' %}

{% raw %}
```markdown
{% include embed/youtube.html id='6zbsUtQL4nY' %}
```
{% endraw %}

## 參考資料
1. https://chirpy.cotes.page/posts/text-and-typography/
2. https://github.com/cotes2020/jekyll-theme-chirpy/blob/master/_posts/2019-08-08-text-and-typography.md?plain=1
3. https://markdown.com.cn/basic-syntax/
4. https://www.markdownguide.org/cheat-sheet/


#### 註：