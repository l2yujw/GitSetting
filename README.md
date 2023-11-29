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

<!-- Numbered list -->
Numbers:
1. first
2. second
3. third

<!-- Link -->
Click [Here]()


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

```ts
console.log('Hello World!');
```

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

git config --global user.name ryu </br>
git config --global user.email jeungwon28@gmail.com </br>
git log </br>
git commit -m '메세지' </br>

commit을 바로 하지 않고 add를 하는 이유 -> 특정 파일만 선택적으로 commit 할 수 있도록 하기 위함 </br></br>

git log </br>
commit cd344a0a67c41aec49814d5b0e248d8337596aa7 -> commit의 고유 이름 </br>
git diff cd344a0a67c41aec49814d5b0e248d8337596aa7 다른 커밋 -> 두 커밋 사이의 소스의 차이를 보여줌 </br>

git reset cd344a0a67c41aec49814d5b0e248d8337596aa7 --hard -> commit 삭제 </br>

git은 파일의 내용이 같으면 index에서는 파일명이 달라도 같게 설정됌  </br>
objects 파일 안에 commit 안에 들어감 (객체라는뜻) </br>


## 팀 프로젝트 복사
git clone --mirror [원본 저장소 경로] <또는 이름> 
그 다음

cd [원본 저장소 이름].git
클론받아온 파일로 cd 해서 들어가준다 .git 꼭해야함

그다음
git remote set-url --push origin [이동할 원격 저장소]
이렇게 해준다음.

git push --mirror
해주면 끝!
git branch ->현재 branch 확인 </br>
git checkout branch명 -> 해당 branch로 이동 </br>
git branch -d exp -> 작업이 끝난 해당 브랜치 삭제 </br>
git log --branches --graph --decorate -> 시각적으로 merge commit branch 상태 보여줌 </br>
