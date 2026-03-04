# 📘 JavaScript 기초 문법 정리

---

## 🛠 자바스크립트 환경 설정

### 1️⃣ VS Code 설치
- https://code.visualstudio.com 접속 후 다운로드
- 설치 시 바탕화면 아이콘 생성 및 PATH 추가 체크

### 2️⃣ Node.js 설치
- https://nodejs.org 접속 후 다운로드
- 설치 후 터미널에서 버전 확인

```bash
node -v
npm -v
```

### 3️⃣ VS Code 추천 확장 프로그램
- HTML CSS Support  
- HTML Snippets  
- JavaScript (ES6) Code Snippets  
- ESLint  
- Prettier - Code Formatter  
- Live Server  

#### 🔧 Prettier 설정
1. 좌측 하단 ⚙ → Settings
2. Default Formatter → Prettier 선택
3. Format On Save 체크

---

# 1️⃣ 자바스크립트란?

- 동적인 웹사이트 제작을 위한 프로그래밍 언어

## 📜 역사
- 1990년대 넷스케이프의 브랜던 아이크가 개발
- Mocha → LiveScript → JavaScript
- 1997년 ECMA 표준화
- ES6부터 모던 자바스크립트 시작

## 🍦 바닐라 자바스크립트
- 라이브러리/프레임워크 없이 순수 JavaScript
- 모든 프레임워크의 기반이 되는 핵심 기술

---

# 2️⃣ 자바스크립트 작성 위치

- 외부 파일 (권장)

```html
<script src="./js/01_js_location.js"></script>
```

- 내부 `<script>` 태그 사용
- 인라인 방식
- CSS 사용 방식과 유사

---

# 3️⃣ console 객체

```javascript
console.log("Hello JavaScript");
```

- 브라우저 개발자 도구(F12)에서 확인 가능

---

# 4️⃣ 변수 선언자

| 선언자 | 특징 |
|--------|------|
| var | 함수 스코프 |
| let | 블록 스코프 |
| const | 상수 선언 |

### 네이밍 규칙
- camelCase
- snake_case
- PascalCase
- Hungarian notation

---

# 5️⃣ 기본 데이터 타입

- String
- Number
- Boolean
- undefined
- null
- Symbol

### ⚠ 64비트 부동소수점 문제

```javascript
0.1 + 0.2 === 0.3 // false
```

---

# 6️⃣ Object

```javascript
const user = {
  name: "홍길동",
  age: 20
};
```

- key-value 구조
- 접근 방법: `user.name`
- 값 수정 및 추가 가능

---

# 7️⃣ Array

```javascript
const arr = [1, 2, 3];
```

- 순서 존재
- index 기반 접근

---

# 8️⃣ 연산자

- 할당 연산자
- 비교 연산자 (== vs ===)
- 산술 연산자
- 논리 연산자
- 문자열 연산자
- 삼항 연산자

---

# 9️⃣ 조건문

## if 문

```javascript
if (조건) {
  실행문;
}
```

## switch 문

```javascript
switch (값) {
  case 값1:
    break;
}
```

---

# 🔟 반복문

## for

```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

## while

```javascript
while (조건) {
  실행문;
}
```

## forEach

```javascript
const arr = [1, 2, 3];

arr.forEach(function(item) {
  console.log(item);
});
```

---

# 1️⃣1️⃣ 함수

## 함수 선언식

```javascript
function add(a, b) {
  return a + b;
}
```

## 함수 표현식

```javascript
const add = function(a, b) {
  return a + b;
};
```

## 화살표 함수

```javascript
const add = (a, b) => a + b;
```

## 콜백 함수 (함수가 파라미터로 전달되는 경우)

```javascript
arr.forEach(function(item) {
  console.log(item);
});
```

---

# 🎯 학습 목표

- 자바스크립트 기본 문법 완전 이해
- 바닐라 JS 기반 웹 동작 구현
- GitHub에 학습 기록 관리