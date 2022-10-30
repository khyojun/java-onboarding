## 🚀 1번 기능 구현 목록
- pobi와 crong의 왼쪽 오른쪽 페이지를 분리해줘야함.
- divideNum을 통한 각자의 자릿수를 나누고 최대값 꺼내기
    - 자릿수를 나눈 것들을 각각 다 더한값, 곱하는 과정이 있어야함.
    - 그리고 두 값 중 어떤 것이 큰지 판별해야함.
- pobiMax,crongMax를 통하여 각자의 왼쪽 오른쪽 페이지를 divideNum하였을때의 최댓값 비교
- 이후 exception을 통해 예외의 경우 처리하기
    - 예외 1: 입력이 들어왔는데 연속된 페이지가 아닌 경우
    - 예외 2: 펼쳤을떄 첫 페이지, 끝 페이지가 나오는 경우