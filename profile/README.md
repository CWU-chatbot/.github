## Hi there 👋

# cwu chatbot
캡스톤디자인 대학교 전용 챗봇

**팀원: 이성원, 변장무, 이동현, 김준서, 김혜주**

## **GitHub 협업 공지사항**

### 1. **repository “Fork”**

### 2. **자신의 github repository에 복사됐는지 확인 후, local에 git clone하기**
`git clone [repository 주소]`

### 3. Organization repository 추가
- **repository 추가** </br>
    `git remote add upstream [organization 주소]`
    
- **repository 확인** </br>
    `git remote -v` </br>
      fork한 내 repository는 **origin**, organization의 repository는 **upstream**

### 4. 자신 브랜치에서 작업 후 add, commit, push, pull & request

**Commit & PR 사용법**

1. `git pull` 하기
2. 코드 수정
3. `git add .` → `git commit -m “타입: 설명”`
    - `타입:` 후 띄어쓰기 필수
    - 타입: 모두 대문자
    - 설명: 영어일 경우, 첫 글자만 대문자
        - 간단히 작성
        -  
4. `git push origin main`

5. push 이후, 자신의 github repository 확인 
    작업했던 branch로 이동→ **compare & pull request** 클릭

6. Pull Request 메세지 작성
    - 설명 가능한 상세하게 작성
    
7.  **Merge pull request는 절대 하지 말것** 
    - 현재까지 작업: **upstream -> (fork) -> origin -> (add/commit/push) -> pull&request -> upstream(merge) 요청**
    
8. 변경(merge)된 upstream을 현재 내가 작업하고 있던 fork한 origin 저장소에 반영해야함 </br>
    `git fetch upstream` → `git merge upstream/main` → `git push origin main`

**Commit 메세지 포멧**

| 타입 | 설명 | 예시 |
| --- | --- | --- |
| FEAT (추가) | 새로운 기능 구현 | FEAT: 로그인 로직 기능 추가 |
| REFACTOR | 내부 로직은 변경하지 않고 코드 개선 및 삭제 | REFACTOR: 코드 줄바꿈 수정 |
| FIX | 버그 또는 오류 해결 | FIX: 로그인 로직 오류 해결 |
| TEST | 테스트 코드 추가 및 수정 | TEST: 로그인 토큰 테스트 코드 추가 |
| COMMENT | 필요한 주석 추가 또는 변경 | COMMENT: 로그인 로직 부분 주석 추가 |
| DESIGN | 화면 디자인 수정 | DESIGN: 로그인 화면 UI 수정 |
| STYLE | 코드 스타일 혹은 포맷 관한 수정 | STYLE: 로그인 글씨체 수정 |
| REMOVE | 파일 삭제 | REMOVE: 중복 파일 삭제 |


