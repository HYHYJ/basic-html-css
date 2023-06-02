## HTML 정리

23.06.01

---

### dialog, details 인터렉티브 요소 -19

---

```html
<body>
  <h1>가입안내</h1>
  <!-- 다이얼로그 예시 -->
  <dialog open aria-label="가입안내">
    <p>차별화된 회원가입 혜택</p>
    <a href="/">지금 바로 만나보세요!</a>
    <div>
      <button type="button">오늘 하루 안 보기</button>
      <button type="button">닫기</button>
    </div>
  </dialog>

  <!-- 상세 및 요약 정보 제공 예시 -->
  <div>
    <details open>
      <summary>국민 내일배움카드</summary>
      <figure>
        <img src="images/learn-card.png" alt="" />
      </figure>
      <p>
        급격한 기술 발전 및 노동시장 변화에 대응하는 사회안전망 차원에서 국민
        스스로 직업능력개발훈련을 실시할 수 있도록 훈련비 등을 지원받을 수 있는
        카드를 의미한다.
      </p>
    </details>
  </div>
</body>
```

### Scripting 요소 -20

---

```html
<link rel="stylesheet" href="./style/card.css" />
<script src="./js/card.js" defer></script>
<noscript>
  <p>Javascript를 지원하지 않은 환경에서는 서비스를 이용할 수 없습니다.</p>
</noscript>
```

### style 내부시트 -23

---

```html
<title>내부 스타일 시트(Embedded Style Sheet)</title>
<style>
  body {
    margin: 40px;
    background: #000;
    color: #fff;
  }
  p {
    text-shadow: 1px 1px 0 #ff0;
  }
</style>
```

### inline style -24

---

```html
<p>
  style 속성에 직접
  <span style="text-decoration: underline; font-weight: bold; color: #f00;"
    >CSS</span
  >
  코드를 작성하여 스타일을 적용합니다.
</p>
```

### font 추가 방법 학습

---

<https://fonts.google.com/>

```html
<title>font family 관련 속성</title>
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link
  href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300;700&display=swap"
  rel="stylesheet"
/>
```

```css
html {
  font-size: 0.625em;
}
body {
  font-size: 1rem;
  font-family: "Noto Sans KR", sans-serif;
  font-weight: 700;
}
```
