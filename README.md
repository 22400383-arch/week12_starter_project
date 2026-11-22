# OSS Week 12 — React Hooks Playground (Student Starter)

## 실행 방법
Node.js 20.19+ 또는 22.12+ 권장. 프로젝트 폴더에서 실행:

```bash
npm install
npm run dev
```

브라우저에 터미널의 Local URL을 열고 LAB 탭을 이동하세요. 제출 전 `npm run build`도 실행하세요.

## 수행 방법
1. `src/components/` 아래의 LAB 1~4 파일에 있는 `TODO`를 직접 완성합니다.
2. `src/App.jsx`, `src/App.css`는 공통 화면이므로 가급적 수정하지 않습니다.
3. 각 LAB의 동작 화면과 콘솔 결과를 기록합니다.
4. 한 LAB에서 다른 LAB으로 탭을 전환하면 기존 컴포넌트가 언마운트됩니다. Cleanup 결과를 관찰합니다.


## 이해도 확인 질문
1. `setCount(prev => prev + 1)`은 왜 유용한가? prev는 최신 상태값이기 때문에 의미전달이 된다.
2. `useEffect(fn, [])`과 `useEffect(fn)`은 어떻게 다른가? []가 있으면 컴포넌트가 처음 마운트될때만 실행되고 없다면 렌더링 될때마다 실행된다.
3. Cleanup은 언제 실행되는가? 개발 환경 StrictMode 영향은? Cleanup은 컴포넌트가 처음 언마운트될때랑 Effect가 다시 실행되기 전에 실행된다. StrictMode에서는 타이머가 중복으로 등록 될 수도 있다.
4. `useState`와 `useRef`의 값 변경 시 렌더링 차이는? useState는 값이 변경될때 렌더링을 하지만 useRef는 렌더링을 하지않는다.
5. LAB 2와 LAB 4에서 Timer를 관리하는 방식의 차이는? Lab2에서는 useEffect를 이용하여 타이머를 생성하고 Lab4에서는 useRef를 이용해서 타이머ID를 저장하여 타이머를 관리한다.
