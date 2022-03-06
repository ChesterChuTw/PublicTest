在 MARKDOWN 中直接寫 html 是可以的

### 標題

# H1

This is an H1
=============
`任何數量的 = 都可以`

## H2

This is an H2
-------------
`任何數量的 - 都可以`

### H3 
#### H4
##### H5
###### H6

---

### REMARK
\<!-- remark -->

---

### NORMAL LINE
連續兩個 breakline 即為 \<p>

---

### 文字樣式
注意: 中間不能有空白

#### Emoji - https://gist.github.com/rxaviers/7360908
:joy:

#### highlight, github not work
I need to highlight these ==very important words==.

#### \<sub> 刪除線
~DeleteLine~

~~The world is flat.~~

#### \<sup> 次方, github not work
X^2^

#### \<code>
`printf()`

``printf()``

A single backtick in a code span: `` ` ``

A backtick-delimited string in a code span: `` `foo` ``

#### \<em>\<i> 
*single asterisks*

_single underscores_

#### \<strong>
**double asterisks**

__double underscores__

---

### 分隔線 
可以在一行中用三個或以上的星號、減號、底線來建立一個分隔線

* * *

***

*****

- - -

---------------------------------------

---

### CODE 

#### 寫法1 （2 tab or 4 space）
    const x = () => {
  
        return 0;
    }

#### 寫法2 

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```
---
### 特殊符號 

#### &copy; - copyright 
#### &amp; - &
#### &lt; - <
#### &gt; - >

---
### 區塊引言 

`幾個 > 決定 引言層級`

#### 寫法 1 
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
> 
> > Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> > id sem consectetuer libero luctus adipiscing.
> > > thrid

#### 寫法 2 
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> > Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.
> > > thrid

---

### 無序清單 

#### 寫法1 
* Red
* Green
* Blue

#### 寫法2 
+ Red
+ Green
+ Blue

#### 寫法3 
- Red
- Green
- Blue

#### 清單段落引言 
*  A list item with a blockquote:

    > This is a blockquote
    > 
    > inside a list item.

#### 清單放程式碼(因為在 list 中，需要含 list 項目 2 tab or 4 space + 程式碼 2 tab or 4 space，共 4 tab or 8 space) 
*  A list item with a blockquote:

        code start here...
        return 0;
        
---

### 有序清單 

#### 寫法1 
1.  Bird
2.  McHale
3.  Parish

#### 寫法2（輸出1.2.3.） 
1.  Bird
1.  McHale
1.  Parish

#### 寫法3（輸出3.4.5.） 
3. Bird
1. McHale
8. Parish

#### 清單段落（每個項目下的段落都必須縮排4個空白或是2個tab） 
1.  This is a list item with two paragraphs. Lorem ipsum dolor
    sit amet, consectetuer adipiscing elit. Aliquam hendrerit
    mi posuere lectus.

    Vestibulum enim wisi, viverra nec, fringilla in, laoreet
    vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
    sit amet velit.

2.  Suspendisse id sem consectetuer libero luctus adipiscing.

---
### 跳脫字元 

1996\. NICE YEAR

---
### LINK 

#### 寫法 1 `[Link 文字](LINK_URL "a tag title")`

This is [an example](http://example.com/ "Title") inline link.

[This link](http://example.net/) has no title attribute.

#### 寫法 2 `[Link 文字][Link ID]，中間不能有空白、Link ID 不分大小寫`

This is [an example][link_id1] reference-style link.

This is [an example][link_id2] reference-style link.

This is [an example][link_id3] reference-style link.

[link_id1]: http://example.com/ "Optional Title Here"

`Markdown.pl 1.0.1會忽略單引號包起來的連結title`
[link_id2]: http://example.com/ 'Optional Title Here' 

`連結網址也可以用<>包起來`
[link_ID3]: <http://example.com/> (Optional Title Here)

#### 寫法 3 `第二個 [] 空白，則會把第一個當 id`
[Google url][]

[Google url]: http://google.com/

#### 寫法 4 (推薦使用) 
I get 10 times more traffic from [Google][1] than from [Yahoo][2] or [MSN][3].

  [1]: http://google.com/        "Google"
  [2]: http://search.yahoo.com/  "Yahoo Search"
  [3]: http://search.msn.com/    "MSN Search"
  
#### 寫法 5 - 自動連結 
http://example.com/

<http://example.com/>

#### Disabling Automatic URL Linking

`http://example.com/`

---
### 圖片 

#### 寫法 1 
![Alt text](/path/to/img.jpg)

#### 寫法 2 
![Alt text](/path/to/img.jpg "Optional title")

#### 寫法 3 
![Alt text][id]

[id]: https://avatars.githubusercontent.com/u/76250269?s=96&v=4  "Optional title attribute"


#### 寫法 4 
<img  src="https://avatars.githubusercontent.com/u/76250269?s=96&v=4" alt="img" title="img_title" />

---
### CHECKBOX 

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

---
### TABLE 
`use pipes (|) to separate each column`
`three or more hyphens (---) to create each column’s header`

#### General 
| Syntax | Description |
| --- | --- |
| Header | Title |
| Paragraph | Text |
| Line3 | Line3 |
| Paragraph | Text |

#### Align 
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this oneeeee   |
| Paragraph   | Text        | And more      |

---
### Footnote(注釋) 
Here's a sentence with a footnote. [^1]
Here's a sentence with a footnote2. [^2]
Here's a sentence with a footnote3. [^3]

[^1]: This is the footnote.
[^2]: [LINK_FOOTNOTE][]
[^3]: https://www.markdownguide.org

[LINK_FOOTNOTE]: https://www.markdownguide.org "markdownguide.org"


