# CloneYoutube
클론코딩 반응형 유투브 사이트 따라만들기

동영상 삽입 방법은 video 태그에 controls를 넣어서 삽입했다.

```html
<video controls src="video/WIN_20220112_22_54_52_Pro.mp4"></video>
```

여러 아이콘들은 [Font Awesome](https://fontawesome.com/) 에서 무료로 가져와서 사용하였다.

처음에는 모바일 환경 즉 화면이 작은 상태에서 볼때로 사이트를 만들었고 

창 크기가 주어 진 값보다 커지면 그거에 맞게 아이템들을 배치하기 위해서 info 와UpNext를 묶어서 infoAndUpNext로 만들어서 @media screen을 통해서 창 크기가 768px 보다 커지면 flex-direction: row;  주어서 배치하였다. 

자바스크립에서 구현한 기능은 제목(title)에 들어가는 글의 길이가 3줄 이상 일때는 2줄로 보이게 하다가 moreBtn을 클릭시 글의 길이가 끝까지 보이게 구현하였다. 이렇게 하기 위해서 css를 이렇게 작성해야 한다.

```css
.info .metadata .titleAndButton .title.clamp {
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 2;
    overflow: hidden;
}
```

## 실행 화면

- 창 크기가 크거나 컴퓨터로 볼 때 

  

![화면 캡처 2022-01-14 155720](../images/README/화면 캡처 2022-01-14 155720.png)

- 창 크기가 작거나 모바일로 볼 때





![화면 캡처 2022-01-14 155641](../images/README/화면 캡처 2022-01-14 155641.png)
