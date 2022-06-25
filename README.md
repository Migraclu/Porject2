|# Markdown| |:----:|

Markdown là một ngôn ngữ đánh dấu với cú pháp văn bản thô, được thiết kế để có thể dễ dàng chuyển thành HTML và nhiều định dạng khác, được dùng để tạo các tập tin Readme.md trên các diễn đàn

Thanks for visiting [The Markdown Guide](https://www.markdownguide.org)!

This Markdown cheat sheet provides a quick overview of all the Markdown syntax elements. It can’t cover every edge case, so if you need more information about any of these elements, refer to the reference guides for [basic syntax](https://www.markdownguide.org/basic-syntax) and [extended syntax](https://www.markdownguide.org/extended-syntax).

---

## Basic Syntax

These are the elements outlined in John Gruber’s original design document. All Markdown applications support these elements.


### Heading

`Use: #H1, ##H2, ..., ######H6`

   # H1
   ## H2
   ...
   ###### H6


### Code
dùng để hiển thị code của Markdown, nó sẽ kế thừa các thuộc tính của thẻ trước nếu ko cách dòng

``Use: `code` ``

   `code`


### Horizontal Rule
tạo 1 đường gạch ngang

`Use: --- `

   ---


### Font


 `Use: **Bold  Text** `

   **Bold text**  

 `Use: *Italic text* `

   *Italic text* 

 `Use: **_Bold and Italic_** `
   
   **_Bold and Italic_**


### Blockquote
Dùng cho trích dẫn câu nói 
> blockquote


### Ordered List
 
 ```
  Use:
   1. First item
   2. Second item
   3. Third item
 ``` 

   1. First item
   2. Second item
   3. Third item


### Unordered List

 ```
  Use:
   - First item
   - Second item
   - Third item
 ``` 

   - First item
   - Second item
   - Third item

##### Khi dùng list, có thể tạo sub list = cách lùi 3 space:
 Trình tự các dấu:

###### - Ordered List: 1 --> i. --> a. --> a.

```
  Use:
1. First item
   1. Second item
      1. Third item
         1. Four item 
```

1. First item
   1. Second item
      1. Third item
         1. Four item

###### - Unordered List: black dot --> white dot --> black square dot --> black square dot

```
  Use:
- First item
   - Second item
      - Third item
         - Four item
```

- First item
   - Second item
      - Third item
         - Four item


### Link
   
   `Use: [Text](url) `   

   [Markdown Guide](https://www.markdownguide.org)


### Image

   `Use: ![alt text](url) ` 

   ![alt text](https://www.markdownguide.org/assets/images/tux.png)


---

## Extended Syntax

These elements extend the basic syntax by adding additional features. Not all Markdown applications support these elements.

### Table

| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

```
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |
```


### Fenced Code Block

` Use: ``` Code ``` `

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### Footnote
 Sẽ được hiện thị dưới footer dù để ở bất kỳ đâu, thường dùng cho chú thích, references

Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.

```
Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.
```

### Heading ID
dùng cho việc gắn id vào cho thẻ, có thể css

```
### My Great Heading {#custom-id}

<h3 id="custom-id">My Great Heading</h3>
```

### Definition List

```
term
: definition

<dl>
  <dt>First Term</dt>
  <dd>This is the definition of the first term.</dd>
</dl>
```

### Task List
giống với select option

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

```
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```


### Emoji

```
That is so funny! :joy:
```

That is so funny! :joy:

(See also [Copying and Pasting Emoji](https://gist.github.com/rxaviers/7360908))


### Font

#### Strikethrough

`Use: ~~Text~~ `
~~The world is flat.~~

 #### Highlight

  `Use: ==Hightlight== `
  I need to highlight these ==very important words==.

 #### Subscript

  `Use: H~2~O `
  H~2~O

 #### Superscript

  `Use: X^2^`
  X^2^
 
