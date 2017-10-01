---
layout: post
title:  "markdown syntax"
date:   2017-10-01 20:58:01 +0900
tags: [markdown, md]
author: ChangHa Choi
img: 2017-10-01-markdown-syntax.png
---
이미 markdown 문법에 대해서는 'markdown' 단어로 검색만 해도 무수히 많이 나옵니다.  
가장 대표적으로 참고할 수 있는 사이트로는 github에서 제공하는 사이트를 참조하는게 좋겠습니다.

* [https://guides.github.com/features/mastering-markdown/](https://guides.github.com/features/mastering-markdown/)
* [https://help.github.com/articles/basic-writing-and-formatting-syntax/](https://help.github.com/articles/basic-writing-and-formatting-syntax/)

markdown 문법을 자주 사용하게 될텐데, 
매번 찾아보기가 어려운 상황이 많을수도 있어 본 포스팅에서 연습할 겸 사용해봅니다.  
역시나 익숙해지기 위해서는 자주 써봐야합니다.


> <h{n}> 태그와 같이 헤더를 적용하는 방법입니다. 앞에 #의 갯수를 {n}만큼 적으면 됩니다.
```
# This is an <h1> tag
## This is an <h2> tag
###### This is an <h6> tag
```
# # This is an <h1> tag
## ## This is an <h2> tag
###### ###### This is an <h6> tag


> italic 적용은 앞뒤로 [\*] 또는 [\_]를 붙이면 됩니다.  
```
*This text will be italic*  
_This will also be italic_
```
*\*This text will be italic\**  
_\_This will also be italic\__


> bold 적용은 앞뒤로 [\*] 또는 [\_]를 두번 연속해서 붙이면 됩니다.  
```markdown
**This text will be italic**  
__This will also be italic__
```
**\*\*This text will be bold\*\***  
__\_\_This will also be bold\_\___


> unordered 목록입니다.
```md
* Item a
    * Item a-1
* Item b
    * Item b-1
```
* Item a
    * Item a-1
* Item b
    * Item b-1  


> ordered 목록입니다.
```mkd
1. Item 1
    1. Item 1-1
1. Item 2
    1. Item 2-1
    1. Item 2-2
```
1. Item 1
    1. Item 1-1
1. Item 2
    1. Item 2-1
    1. Item 2-2
 
    
> 문장안에서 코드를 표현하는 inline code를 사용할때에는 앞뒤로 backticks(`)를 붙이면 됩니다.  
```
I think you should use an `<addr>` element here instead.  
Use `git status` to list all new or modified files that haven't yet been committed.
```
I think you should use an `<addr>` element here instead.  
Use `git status` to list all new or modified files that haven't yet been committed.


> 취소선은 앞뒤로 [~]를 두번 연속해서 붙이면 됩니다.
```
~~show me the money~~
```
~~show me the money~~

> 링크는 \[링크걸릴문장\]\(링크주소\) 로 표현합니다. 다만 '_blank' target 지정과 같이 새창으로 띄우는 설정은 따로 없습니다.
```
[facebook url](https://fb.com/changhachoi)
```
[facebook url](https://fb.com/changhachoi)

> code highlight는 두가지 방법이 있습니다.  
[jekyll template 문법](https://jekyllrb.com/docs/templates/#code-snippet-highlighting)의 경우 linenos를 통해 line number 표현까지 가능하며,
{% highlight ruby linenos %}
def foo
  puts 'foo'
end
{% endhighlight %}  
> [markdown 문법](https://help.github.com/articles/creating-and-highlighting-code-blocks/)의 경우는 line number 표현은 불가능합니다.  
```ruby
def foo
  puts 'foo'
end
```

> 