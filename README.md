# tokens

## 명명법에 부쳐
### 문제의 발생
- 색상의 위계를 light & dark로 표현하는 경우 테마의 변경에 대응하기 위해 해당 토큰이 사용된 컴포넌트의 값을 변경해야 함. weak & strong을 쓰면 variables의 변경으로 테마에 대응. 기존의 dark light / night day 뿐 아니라 OS 맥락에서의 커스텀 UI를 위해서도.
- 역할에 기반하지 않아야 함. 가령 --font-size-subhead는 tokens에서 정의해야 하는 수준의 추상화가 아니다. subhead는 단순 font-size의 변경을 통해 정의할 수 없음.
