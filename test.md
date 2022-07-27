## Git 실습 - 문제풀기
> 아래에 있는 각각의 문제에 대해 답과 이유를 작성하시오.
> 함께 PR을 날리면서 집단지성을 통해 문제를 풀어 봅시다.

1. git은 무엇인가요?   
   - 답 : 분산 버전 관리 시스템
  
2. Staging Area의 역할은 무엇일까요?
   - 답 :  커밋을 위한 파일 및 폴더가 추가되는 곳

3. 변경사항을 기록하는 과정을 아래 코드 블록에 작성해 주세요.
   - 답
   ```bash

   git add .
   git commit -m ""
  
        git add .
        git commit -m "수정되었습니다."
   ```

4. 아래와 같은 메시지가 발생했을 때, 무엇을 해야 할까요?
![image](https://user-images.githubusercontent.com/98133984/181182281-4d01a374-62fe-4957-9a07-1efc005e35d3.png)
   - 답
   ```bash

   git config --global user.name "이름"
   git config --global user.email "메일 주소"
   
   ```
        git config --global user.name '이름'
        git config --global user.email '이메일'
   ```

5. clone과 pull의 차이는 무엇인가요?
   - 답 : clone은  로컬 저장소를 만드는 역할,
Github에서 저장소를 복제해서 내 컴퓨터에 똑같은 복제본을 만든다.pull은 g로컬 저장소와 원격 저장소의 내용을 동기화, 원격 저장소의 변경 내용을 로컬 저장소에 반영하는 것

6. branch를 만드는 목적은 무엇인가요?
    - 답 : 브랜치를 통해 별도의 작업 공간을 만들고, 그곳에서 되돌리거나 삭제를 한다.브랜치는 완전하게 독립이 되어있어서 master대해 안전하다. 그러므로 에러 발생시 원본을 지키며 해결이 가능하다.

7. branch를 생성하는 동시에 이동하는 명령어는 무엇인가요?
    - 답 : 
```bash
git switch -c
```

8. 다음과 같은 상황이 나타났을 때 어떻게 해야 하나요?
   ![image](https://user-images.githubusercontent.com/98133984/181183354-df42d325-b839-48e1-a4c6-667c20b33d5c.png)
    - 답 :git pull을 먼저 해서 동기화 시키고 새로운 커밋을 쌓아 나간다.


9.  소유권이 없는 협업을 하기 위해서 가장 먼저 해야 할 것은 무엇일까요?

fork를 통해 내 원격 저장소로 복제한다.

10. 소유권이 없는 협업의 경우, `git push origin master`로 원격 저장소에 변경사항을 반영할 수 있다.
    - 답 : X
    - 이유 :pull Request를 통해 원본 원격 저장소의 master에 반영해달라는 요청을 보내야 한다.
   - 답 : remote 설정을 자동으로 하나 안하나의 차이.
    - clone은 remote 설정을 자동으로 해주지만, pull의 경우 remote 설정 후 사용해야함
   
6. branch를 만드는 목적은 무엇인가요?
    - 답 : 여러 사람이 각자의 독립된 공간에서 동시에 다양한 작업을 할 수 있게 하기 위해서

7. branch를 생성하는 동시에 이동하는 명령어는 무엇인가요?
    - 답 : git switch -c '브랜치명'

8. 다음과 같은 상황이 나타났을 때 어떻게 해야 하나요?
   ![image](https://user-images.githubusercontent.com/98133984/181183354-df42d325-b839-48e1-a4c6-667c20b33d5c.png)
    - 답 : 원격저장소에는 있으나 로컬저장소에는 없는 파일로 인해 발생한 것이기에, 먼저 원격저장소를 pull한 후 다시 push한다.

9.  소유권이 없는 협업을 하기 위해서 가장 먼저 해야 할 것은 무엇일까요?
    - 답 : 소유권이 없는 원격 저장소를 'fork'를 통해 내 원격 저장소로 복제한다.

10. 소유권이 없는 협업의 경우, `git push origin master`로 원격 저장소에 변경사항을 반영할 수 있다.
    - 답 : X
    - 이유 : branch를 생성하여 작업을 진행하였기에 'git push origin branch명'으로 변경사항 반영해야한다.
 
11. git reset 명령어의 옵션 중, staging area 상태로 돌아가는 옵션은 ______이다.
    - 답 : --soft

12. 바로 직전 커밋을 수정하기 위해서 필요한 명령어를 작성하세요.
    - 답
    ```
    git commit --amend
    ```

13. merge와 rebase의 차이점은 무엇일까요? 
     - 답 : merge : branch를 통합/ rebase : base를 옮기는 것
        git commit --amend
    ```

13. merge와 rebase의 차이점은 무엇일까요? 
     - 답 : merge는 branch를 통합하는 것이고, rebase는 branch의 base를 옮기는 것
