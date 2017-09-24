---
layout: post
title:  "dlog - jekyll theme"
date:   2017-09-24 22:06:14 +0900
tags: [jekyll]
author: ChangHa Choi
---
DLOG 첫번째 포스팅은 jekyll blog theme 입니다.

brunch에서 언급([https://brunch.co.kr/@alklid/12](https://brunch.co.kr/@alklid/12))한데로 github pages에 기술블로그를 만들어 보기위해 jekyll을 올렸습니다.  
github pages에 jekyll을 올리는 방법에 대해서는 워낙 다양한 자료가 이미 있어서 따로 정리하지는 않았습니다.  
[jekyll 공식 사이트](https://jekyllrb.com), [한글번역사이트](https://jekyllrb-ko.github.io/) 공식사이트가 있긴 하지만, 만든 사람보다 써본사람이 초기에 이해하기 쉽게 설명해주는 편인것 같습니다.
[xho96's Swift Lift](https://xho95.github.io/blog/github/jekyll/git/2016/01/11/Make-a-blog-with-Jekyll.html), [Nolboo's Blog](https://nolboo.kim/blog/2013/10/15/free-blog-with-github-jekyll/) 정도 보시면 도움될 것 같습니다.  

깔끔한게 좋아서 [http://jekyllthemes.org](http://jekyllthemes.org) 이곳에서 테마를 찾아 보았지만, 취향저격 테마가 없어서  
그중 제일 깔끔해보이는 Adam Blog Theme [https://github.com/artemsheludko/adam-blog](https://github.com/artemsheludko/adam-blog)를 기반으로 조금 변경해 보았습니다.

이미 Adam Blog Theme 에 여러가지 plugin이 지원되도록 설정되어 있습니다.
* Google Fonts
* Font Awesome
* Disqus
* MailChimp
* Analytics
* Search  
  
  
  
추가로 변경한 사항은 아래와 같습니다.
* post-card to post-list
    * 사진위주의 포스팅목록의 배치가 카드형식으로 되어 있어, 이를 리스트 형식으로 변경했습니다.
* Analytics
    * Google Analytics의 추적코드를 기존 analytics.js에서 gtag.js기반으로 변경했습니다.
* _site directory structure
    * 빌드시 _site폴더 하위에 post 생성이 분류가 안되고 있어 yyyy/mm/dd순으로 생성되도록 설정을 변경했습니다.
* _sass auto compile
    * 따로 compile 해야했던 assets/sass들을 빌드시 자동으로 compile되도록 폴더구성과 설정을 변경했습니다.
* code highlight
    * code highlight monokai theme로 변경했습니다.
* baseurl 설정시 pagenation 링크 오류 수정
    * pagenation 링크에 baseurl 설정값이 표현되어 있지 않아, 링크주소가 잘못 설정되는 오류를 수정했습니다.
    

변경한 사항에 대한 Theme는 준비되는데로 github repo에 올려놓겠습니다.