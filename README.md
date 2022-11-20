# tokens

## 명명법에 부쳐
### 문제의 발생
- 색상의 위계를 light & dark로 표현하는 경우 테마의 변경에 대응하기 위해 해당 토큰이 사용된 컴포넌트의 값을 변경해야 함. weak & strong을 쓰면 variables의 변경으로 테마에 대응. 기존의 dark light / night day 뿐 아니라 OS 맥락에서의 커스텀 UI를 위해서도.
- 역할에 기반하지 않아야 함. 가령 --font-size-subhead는 tokens에서 정의해야 하는 수준의 추상화가 아니다. subhead는 단순 font-size의 변경을 통해 정의할 수 없음.
-
-
- 
- 하나의 구조를 위해 레이아웃의 변경을 염두하여 top, bottom, left, right 등의 방향으로 props를 명명해서는 안 됨. 결국 돌고 돌아 역할 기반으로.



## line-height의 best practices
- 하나의 서비스에 필요한 line-height tokens은 최소 2개
### length - px / em / rem
### percentage - % / number
### size tokens
### figma와 연계되는 문제

## line-height와 rem 단위

## 기타
- 구조, 표현, 동작을 구분한다는 과거의 패러다임은 React 등으로 요원. 플랫폼과 콘텐츠의 시대에 웹서비스를 구성하는 컴포넌트나 구조는 굉장히 보편적이고 일반화.
- 후려치면 표현은 tokens과 utilites의 조합으로 모두 가능. 이것들을 망라한 것이 디자인 시스템 문서에 포함되어야.
- native CSS의 발전을 CSS-in-JS가 따라갈 수 있나. 왜 CSS-in-JS ? 표준에 가까운 기술 학습에 투자하라.
- 결국 컴포넌트의 구조를 변경할 일은 없어야 한다. 또는 없어도 되지 않나. 하지만 접근성과 관련된 속성까지 미리 정의하기는 어렵다. 속성은 동작에도 종속. 동작까지도 utilization.
- 구조를 변경할 일이 없다는 말은 다시 말해, 모든 웹서비스가 하나의 html 구조의 컴포넌트 조합으로 만들어 질 수 있다. 유아이 라이브러리를 만든다면 이게 대원칙이 되어야 할 것.



- 컴포넌트의 상태를 custom hooks으로 관리.
