# fe-w4-martian

![](https://images.theconversation.com/files/96726/original/image-20150930-19533-1by0fu3.jpg?ixlib=rb-1.1.0&rect=0%2C0%2C2000%2C970&q=45&auto=format&w=1356&h=668&fit=crop)

## 학습 키워드

- ES Module방식 개발
- 함수형 프로그래밍
- Promise

## 해야할 것

- [ ] 1. myPromise 객체 만들기
- [ ] 2. 미션 구현

## 동작 순서도

**지구 -> 마션 (수신)**

1. 문자를 입력한다 (O)
2. 16진수로 변환한다 (O)
3. 수신기가 5초 간격으로 해석한 문자를 하나씩 읽어온다 (0)
4. 문자를 [송수신정보]에 띄우고(0), 2초간 가르키고, 그동안 애니메이션을 진행한다
5. 다 받아오면, [해석하기] 버튼이 활성화된다(0)
6. 버튼을 누르면, [해석본]에 띄운다(0)

**마션 -> 지구**

1. [발신정보입력]에 문자를 입력한다 (0)
2. 실시간으로 번역되는 내용을 [발신정보]에 띄운다(0)
3. [지구로보내기] 버튼을 누르면, [발신정보]에 있는 내용을 하나씩 [송수신정보]에 띄우고 수신기가 2초간 가르키면서 애니메이션 진행한다

**3월4일(목)**

- 현재 버그 사항

1. innerHTML을 참고하면 비동기로 innerHTML을 넣기 때문에
   실행되면 innerHTML이 없어서 해석이 안된다.
   문제점 해결방안 : innerHTML이 채워지면, 이 함수를 실행한다.
2. [지구로 보내기]를 하면, undefined가 뜨고 PrintData가 된다.
   이것도 비동기 문제인 것 같다.

- 고칠사항

1. js로 반복해서 dom templating
2. 캔버스 22.5 매직넘버 고치기
3. 캔버스 함수 나누기
4. 캔버스 scss for문으로 구현해보기
5. forEach말고 map혹은 reduce로 구현해보기 6.ㅇㅇㄴㅇㄴ
