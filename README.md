README
===========================
This repo is a translation of [https://github.com/guodongxiaren/README](https://github.com/guodongxiaren/README). Thanks a lot for the original author's effort.
This file is used to demonstrate the markdown syntax for writing README files. The markdown syntax is extended on Github, which is called `GitHub Flavored Markdown`, i.e. `GFM`. GFM is widely used on GitHub. Issues and wiki also support GFM syntax.

****
	
|Translator|Yaoyao Liu|
|---|---
|E-mail|yliu@yliu.tech


****
## Index
* [Lines](#lines)
* [Headers](#headers)
* [Texts](#texts)
    * [Normal text](#normal-text)
    * [Single-line text](#single-line-text)
    * [Multi-line text](#multi-line-text)
    * [Text highlighting](#text-highlighting)
    * [Wrap](#wrap)
    * [Emphasis and strikethrough](#emphasis-and-strikethrough)
* [Images](#images)
    * [Images from the Internet](#images-from-the-internet)
    * [Images from the GitHub repository](#images-from-the-github-repository)
* [Links](#links) 
    * [Text hyperlink](#text-hyperlink)
        *  [Links to external URLs](#links-to-external-urls)
        *  [Links to the URLs in this repository](#links-to-the-urls-in-this-repository)
    * [Anchor](#anchor)
    * [Image links](#image-links)
* [Lists](#lists)
    * [Unordered](#unordered)
    * [Ordered](#ordered)
    * [Task Lists](#task-lists)
* [Blockquotes](#blockquotes)
* [Fenced code blocks](#fenced-code-blocks)
* [Tables](#tables) 
* [Emoji](#emoji)
* [diff syntax](#diff-syntax)

### Lines
-----------
***、---、___can display the line effect

***
---
___



Headers
------

# This is an h1 tag
## This is an h2 tag  
### This is an h3 tag 
#### This is an h4 tag 
##### This is an h5 tag
###### This is an h6 tag


Texts
------
### Normal text
This is a example of normal text.
### Single-line text
    Hello, world!
Add 1 tab or 4 spaces at the beginning of the line.
### Multi-line text
#### Syntax 1
Add 1 tab or 4 spaces at the beginning of several lines of text.

    Sons of Gondor,
    of Rohan,
    my brothers!

#### Syntax 1
Use three backticks:
```
Sons of Gondor,
of Rohan,
my brothers!
```
This syntax can also be used for code highlighting，See [Code-highlighting](#Code-highlighting)
### Text highlighting
Using a pair of backquotes.
Syntax：
```
`linux` `ubuntu` `socket` `epoll` 
```
Look like: `linux` `ubuntu` `socket` `epoll`

Also suitable for making tags for articles.
#### Wrap
Directly inputing return cannot wrap.  
You may add two spaces after the previous line of text.
Then the text of the next line is wrapped.

You may also add a blank line directly to the two lines of text.

This operation can also be used to wrap, except the line spacing is a bit large.
#### Emphasis and strikethrough

|Syntax|Look like|
|----|-----|
|`*Italic1*`|*Italic1*|
|`_Italic2_`| _Italic2_|
|`**Bold1**`|**Bold1**|
|`__Bold2__`|__Bold2__|
|`This is a ~~strikethrough~~`|This is a ~~strikethrough~~|
|`***Italic plus bold1***`|***Italic plus bold1***|
|`___Italic plus bold2___`|___Italic plus bold2___|
|`***~~Italic, bold, and strikethrough1~~***`|***~~Italic, bold, and strikethrough1~~***|
|`~~***Italic, bold, and strikethrough2***~~`|~~***Italic, bold, and strikethrough2***~~|

    Italic, bold, strikethrough is able to be used together.

Images
------
Basic syntax：
```
![alt](URL title)
```
alt and title are corresponding to the alt and title attributes in the HTML (all can be omitted)：
- alt indicates the replacement text when the image fails to display
- title indicates the text to display when the mouse hovers over the image (note that it should be quoted here)

The URL is the url address of the image. If you refer to the image in this repository, you can use the **relative path** directly. If you refer to the images in other github repositories, you should pay attention to the format, ie: `repository address/raw/branch_name/image_path `, e.g.
```
https://github.com/username/reponame/raw/master/folder/imagename.gif
```

|#|Syntax|Look like|
|---|---|----
|1|`![Google](https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Google logo")`|![Google](https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Google logo")
|2|`![][foryou]`|![][foryou]

Note that the syntax of Example 2 uses the form of the **URL identifier**, which has been described in the [Link](#link) section.
>foryou is defined at the end of the page like this:
```
[foryou]:https://github.com/guodongxiaren/ImageCache/raw/master/Logo/foryou.gif
```

Link
------
### Links to external URLs

|#|Syntax|Look like|
|---|----|-----|
|1|`[My blog](http://www.cnblogs.com/yaoyaoliu "Hover display")`|My blog](http://www.cnblogs.com/yaoyaoliu "Hover display")|
|2|`[My GitHub][GitHubLink] `|[My GitHub][GitHubLink]|

This syntax consists of two parts:：
- The label in [ ] (in this case is GitHubLink). It can be a combination of numbers, letters, etc.
- The actual URL.

>You may define your link label anywhere in the document.

### Links to the URLs in this repository

|Syntax|Look like|
|----|-----|
|`[Example document](/example/example.md)`|[Example document](/example/example.md)|
|`[example](./example)`|[example](./example)|

### Image links
The essence of adding links to images is mixing image display syntax with the normal link syntax. In the normal link, [ ] is the text to be displayed inside the link, and the image link [ ] is the image to be displayed.
It's ok to mix the two syntaxes directly, but it's awkward, so we can use the form of the link label.

|#|Syntax|Look like|
|---|----|:---:|
|1|`[![weibo-logo]](http://weibo.com/linpiaochen)`|[![weibo-logo]](http://weibo.com/linpiaochen)|
|2|`[![](/img/zhihu.png "This is the Zhihu link")][zhihu]`|[![](/img/zhihu.png "This is the Zhihu link")][zhihu]|
|3|`[![csdn-logo]][csdn]`|[![csdn-logo]][csdn]|

As the image and the link both support link label, the image link can be very simple (see Example 3).
Note that the text displayed when the mouse hovers there is the title of the image, not the title of the link.
> All the link labels in the documents is placed at the end of the document.

### Anchor
In fact, each title is an anchor, similar to the HTML anchor (`#`), e.g.

|Syntax|Look like|
|---|---|
|`[Back to top](#readme)`|[Back to top](#readme)|

Note that all the letters in the title are converted to **lowercase letters**.

## Lists
### Unordered
#### Syntax
```
* First name: Yaoyao
- Last name: Liu
* Title: Mr.
```
#### Look like
* First name: Yaoyao
- Last name: Liu
* Title: Mr.

### Multi-level unordered
#### Syntax
```
* Python
    * Tensorflow
        * slim
```
#### Look like
* Python
    * Tensorflow
        * slim

### Ordered
#### Syntax
Just add a dot and a space after the number. However it may not seem obvious enough. 
```
Famous social media:

1. FB
2. IG
3. WeChat
```

#### Look like
Famous social media:

1. FB
2. IG
3. WeChat


### Multi-level ordered
Like unordered lists, ordered lists also have a multi-level structure.
#### Syntax
```
1. First
   1. Second
      1. Third
```

#### Look like

1. First
   1. Second
      1. Third
	 

### Task Lists
#### Syntax
```
- [x] item 1
- [x] item 2
- [x] item 3
- [ ] itme 4
- [ ] item 5
- [ ] item 6
```
#### Look like

- [x] item 1
- [x] item 2
- [x] item 3
- [ ] itme 4
- [ ] item 5
- [ ] item 6

> Tip:
>> You may use this syntax in GitHub's **issue** to check or uncheck the checkbox in real time without having to modify the original version of the issue.

## Blockquotes
#### Syntax
```
As Grace Hopper said:
> I’ve always been more interested
> in the future than in the past.
```
#### Look like
As Grace Hopper said:
> I’ve always been more interested
> in the future than in the past.

### Multi-level blockquotes
#### Syntax
```
> Asia
>> China
>>> Beijing
>>>> Haidian
>>>>> Tsinghua
```
#### Look like
> Asia
>> China
>>> Beijing
>>>> Haidian
>>>>> Tsinghua

Fenced code blocks
----------

### Syntax
With GFM you can wrap your code with three back quotes to create a code block without the leading spaces. Add annoptional language identifier and your code will get syntax highlighting.

### Look like
```Java
public static void main(String[]args){} //Java
```
```c
int main(int argc, char *argv[]) //C
```
```Bash
echo "hello GitHub" #Bash
```
```javascript
document.getElementById("myH1").innerHTML="Welcome to my Homepage"; //javascipt
```
```cpp
string &operator+(const string& A,const string& B) //cpp
```
Tables
--------

First Header | Second Header
------------ | -------------
Content cell 1 | Content cell 2
Content column 1 | Content column 2

### Align
You may specify alignment like this:

| Align left | Centered  | Align right |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |

### Mix with other syntax
Most GFM syntax can be applied in the contents of the table cell, e.g.  
#### Use strikethrough, italic, etc.

| Name | Content |
| ------------- | ----------- |
| Help      | ~~Display the~~ help window.|
| Close     | _Closes_ a window     |

#### Embed an image (link) in the table

| Img | Text |
| ---- | ---- |
|![baidu][baidu-logo] | Baidu |

Emoji
----------
GFM syntax supports adding emojis, and entering different symbol codes (characters surrounded by two colons) can display different emoticons.

e.g.`:blush:`，look like:blush:。

You may check the codes for different emojis using this link: [http://www.emoji-cheat-sheet.com](http://www.emoji-cheat-sheet.com)。

But this page is loaded **very slowly** every time. So I sorted it into this repo, you can view it directly here.[emoji](./emoji.md)。

diff syntax
---------
版本控制的系统中都少不了diff的功能，即展示一个文件内容的增加与删除。
GFM中可以显示的展示diff效果。使用绿色表示新增，红色表示删除。
In the version control system, the function of diff is indispensable, i.e., the addition and deletion of a file content is displayed.
The diff effect that can be displayed in GFM. Green is for new, while red is for deleted.
#### Syntax
The syntax is similar to code [fenced code blocks](#fenced-code-blocks), except that the diff is written after the three backticks.
And in the content, the beginning of `+ ` indicates the addition, and the beginning of `- ` indicates the deletion.

#### Look like

```diff
+ Hello world!
- This is useless.
```



--------------------------------
[csdn]:http://www.csdn.net/ "This is CSDN"
[zhihu]:https://www.zhihu.com/ "This is Zhihu"
[GitHubLink]:https://github.com/y2l "This is my GitHub"
[weibo]:http://weibo.com/linpiaochen
[baidu-logo]:http://www.baidu.com/img/bdlogo.gif "Baidu logo"
[weibo-logo]:/img/weibo.png "Weibo!"
[csdn-logo]:/img/csdn.png "CSDN!"
[foryou]:https://github.com/guodongxiaren/ImageCache/raw/master/Logo/foryou.gif
