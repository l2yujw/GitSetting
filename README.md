<!-- Heading -->
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
Paragraph

<!-- Line -->
___

<!-- Text attributes -->
This is the **bold** text and this is the *italic* text and let's do ~~strikethrough~~.

<!-- Quote -->
> Don't forget to code your dream 

<!-- Bullet list -->
Fruits:
🍎
🍋

Other fruits:
🍑
🍏

<!-- Numbered list -->
Numbers:
1. first
2. second
3. third

<!-- Link -->
Click [Here]()

<!-- Image -->
![image description](https://user-images.githubusercontent.com/61736137/102153953-b2881000-3ebb-11eb-9581-7026bc8e169e.jpg)


<!-- Table -->
|Header|Description|
|:--:|:--:|
|Cell1|Cell2|
|Cell3|Cell4|
|Cell5|Cell6|

<!-- Code -->
To print message in the console, use `console.log('your message')` and ..

```ts
console.log('hello')
```

<!-- PR Description Example -->
# What is Lorem Ipsum?
`Lorem Ipsum` is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy **text ever since the 1500s**, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

```ts
console.log('Hello World!');
```

|Feature|Description|
|--|--|
|Feature1|<img src="https://user-images.githubusercontent.com/61736137/102153953-b2881000-3ebb-11eb-9581-7026bc8e169e.jpg" width="400"><br>Feature1. Responsive Web Page|
|Feature2|<img src="https://user-images.githubusercontent.com/61736137/102153956-b451d380-3ebb-11eb-9ab7-f8bad6c05a97.png" width="400"><br>Feature2. Responsive Web Page|

## Before release
- [x] Finish my changes
- [ ] Push my commits to GitHub
- [ ] Open a pull request

## screenshot
Issues -> Write에 이미지 붙이기 -> 복사

# GitSetting

Github CRLF 문제 해결 방법
운영체제 별로 개행문자 다르게 인식
Windows 에서는 line ending으로 CR(Carriage-Return, \r) 및 LF(Line Feed, \n) 사용

1. git config --global core.autocrlf true
2. git root폴더(.git폴더 있는 곳)에 .gitattributes파일 생성
아래 코드 입력 후 저장


`.gitattributes파일

    # Auto detect text files and perform LF normalization
    *        text=auto

    *.cs     text diff=csharp
    *.java   text diff=java
    *.html   text diff=html
    *.css    text
    *.js     text
    *.sql    text

    *.csproj text merge=union
    *.sln    text merge=union eol=crlf

    *.docx   diff=astextplain
    *.DOCX   diff=astextplain

    # absolute paths are ok, as are globs
    /**/postinst* text eol-lf

    # paths that don't start with / are treated relative to the .gitattributes folder
    relative/path/*.txt text eol-lf
`




git config --global user.name ryu
git config --global user.email jeungwon28@gmail.com
git log
git commit -m '메세지'

commit을 바로 하지 않고 add를 하는 이유 -> 특정 파일만 선택적으로 commit 할 수 있도록 하기 위함

git log
commit cd344a0a67c41aec49814d5b0e248d8337596aa7 -> commit의 고유 이름
git diff cd344a0a67c41aec49814d5b0e248d8337596aa7 다른 커밋 -> 두 커밋 사이의 소스의 차이를 보여줌

git reset cd344a0a67c41aec49814d5b0e248d8337596aa7 --hard -> commit 삭제


git은 파일의 내용이 같으면 index에서는 파일명이 달라도 같게 설정됌
objects 파일 안에 commit 안에 들어감 (객체라는뜻)

git branch ->현재 branch 확인
git checkout branch명 -> 해당 branch로 이동
git branch -d exp -> 작업이 끝난 해당 브랜치 삭제
git log --branches --graph --decorate -> 시각적으로 merge commit branch 상태 보여줌

