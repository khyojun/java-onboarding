## 🚀 2번 기능 구현 목록
1. 연속으로 중복된 문자열을 제거하기 위하여서 **StringBuffer의 delete**를 활용
2. 문자열을 삭제한 이후에도 다시 중복된 문자열이 있는지 확인하기 위하여 무한루프를 활용하여
확인
  - 
  - 종료 조건 지정
     - 현재 가리키고 있는 문자열이 제일 끝 문자열이거나, 문자열의 길이가 1이고, 더이상 중복삭제를 할 수 없는 상황일 경우
  - 현재 가리키고 있는 문자열이 제일 끝 문자열이어도 중복 삭제를 한 번 실행한 경우 다시 한 번 탐색
  - 중복된 문자열을 발견하였을때 그 시점부터 판별하기 위한 기능구현
    1. 중복검사를 진행하는데 다른 문자열이 나타나면 해당 중복 문자열을 delete 그 문자열이 있던 위치로 index를 옮기고(옮기기위하여 중복이 몇번 됬는지 확인 후 index조정) 길이 문자열의 길이도 재수정
    2. 중복검사를 진행하다가 끝까지 똑같은 문자열이 일어나는 경우도 삭제 후 index를 처음 위치로 옮기고, 문자열의 길이 조정 
  - 중복된 문자열을 발견 못했다면 index증가시켜 다음 문자를 기점으로 확인


이후로 최종적으로 중복 문자열을 제거한 StringBuffer를 String으로 바꿔 정답 문자열 answer에 넣고 정답 출력