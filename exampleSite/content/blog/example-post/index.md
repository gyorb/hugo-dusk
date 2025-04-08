---
title: "Test post"
description: "example post to show all the features of the theme"
tags:
  - test
  - example
  - markdown
  - theme
  - hugo
date: "2014-04-02"
publishDate: "2014-04-02"
categories:
  - markdown
  - test
series:
  - hugo
syndicate:
  - "https://example.org"
audio: []
videos: []
images: []
---

Markdown test post for the theme.


Nisi aliquid ratione aut. Et laborum est et qui distinctio nemo et nobis. Cumque ab suscipit ad labore nesciunt dolore quo molestias. Enim perferendis et sunt.

Beatae odio et adipisci ullam aperiam recusandae. Occaecati non aspernatur harum in delectus vero facere. Similique aut ea animi. Possimus distinctio et qui.

<!--more-->

# Heading 1

**This text is bold** and __this is too__.  

{{< details summary="See the details" >}}

Beatae odio et adipisci ullam aperiam recusandae. Occaecati non aspernatur harum in delectus vero facere. Similique aut ea animi. Possimus distinctio et qui.

> Blockquote.


```toml
baseurl = "/"
title = "Hugo Theme"
languageCode = "en-US"
canonifyurls = true
pagination.pagerSize = 3
theme = "hugo-dusk"
themesDir = "../.."
enableRobotsTXT = true
```

> [!NOTE]
> some note

{{< /details >}}

## Heading 2

*This text is italic* and  _this is too_.  

### Heading 3

**_Bold and italic_?**  

#### Heading 4

~~strikethrough~~

##### Heading 5

---

## Blockquote

> Blockquote.
>
> > Nested.
> >
> > > **bold** and _italic_

---

## Callouts

> [!NOTE]
> some note

> [!TIP]
> tip

> [!WARNING]
> warning

> [!TODO]
> todo

> [!CAUTION]
> caution

> [!IMPORTANT]
> important

---

## Lists

### Ordered

1. Go
2. Linux
3. Security
4. Privacy


### Unordered

- Go
+ Linux
* Security
- Privacy

### Mixed

1. Programming languages
   1. Go
   2. Rust
   3. Zig
2. Standard libraries
   - Go
     - bufio
     - context
     - os
     - ...

---

## Tables {#tables-id}

| Left Align (default) | Center Align | Right Align |
| :------------------- | :----------: | ----------: |
| Go                   | bufio        | PostgreSQL  |
| Rust                 | context      | valkey      |
| Zig                  | os           | SQLite      |

[Jump to section](#jump-id)

---

## Task Lists

- [x] Learn Go
- [ ] Improve Security

---


## Images


![Image from pexels containing data codes through eyeglasses](images/pexels-kevin-ku-92347-577585.jpg "https://www.pexels.com/photo/data-codes-through-eyeglasses-577585/")


### missing image

[missing]: images/missing-image.png "missing image"
![Alt text for a missing image][missing]


---

## Footnote

A simple footnote[^1] and a longer one[^longnote].

[^1]: This is the first.

[^longnote]: Longer footnote with multiple lines.

    Indent paragraphs to add to the footnote and use any markdown elements like, `code`

    > blockquotes

    and even callouts

    > [!tip]
    > some tip



## Links

[link with title](https://www.example.com "example.com")

Reference style link: [example][example]

[example]: https://www.example.com

---

## Code


```toml
baseurl = "/"
title = "Hugo Theme"
languageCode = "en-US"
canonifyurls = true
pagination.pagerSize = 3
theme = "hugo-dusk"
themesDir = "../.."
enableRobotsTXT = true

```



## Jump to section {#jump-id}

[Jump to a section with custom ID](#tables-id)

