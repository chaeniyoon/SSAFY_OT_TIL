# **SSAFY 240111_수업**

## ! What to Study? !
- 현업에서 내가 만든 코드를 공유할 때 어떻게 하면 정리할 수 있을까? -> "Markdown"
- 여러 사람들과 공동 프로젝트를 진행할 때 어떻게 같이 진행할 수 있을까? -> "Git"

---

## Markdown ?
> **0. 관련 링크**
- [Markdown 실습 링크](https://www.markdownguide.org/basic-syntax/)
    
- 일반 텍스트로 문서를 작성하는 간단한 방법
- 주로 개발자들이 텍스트와 코드를 작성해 문서화하기 위해 사용 --> 1시간안에 배울 수 있을 만큼 간단하다.
- 즉, 개발자들의 나의 코드를 다른 사람들과 공유할 때 좀 더 쉽게 공유하고자 만든 방법이라고 생각
- 작성된 마크다운 문서는 다른 프로그램에 의해 변환되어 출력됨


> **1. Markdown 실습 정리**

- 1-1. 바탕화면에 markdown_pratice 파일 만들고 > 하단에 READ.md 파일 new file 만들기
    
    ![관련 이미지](./image_1.PNG)

- 1-2. READ.md 우클릭 > open preview 클릭 > 다음과 같은 꾸며진 text 구조 확인 가능

    ![관련 이미지](./image_2.PNG)

- 1-3. # 수에 따라서 제목의 size 변환 가능 > 최대 6개까지 가능

    ![관련 이미지](./image_3.PNG)

- 1-4. 리스트 관련, 아래로 들여쓰기 > 원하면 tab 누르기

    ![관련 이미지](./image_4.PNG)

- 1-5. Code block & Inline code block
    - code block? 
        
        : 일반 텍스트와 달리 해당 프로그래밍 언어에 맞춰서 텍스트 스타일을 변환

        : 개발에서 마크다운을 사용하는 가장 큰 이유

        ![관련 이미지](./image_5.PNG)

    - Inline?   
       
        : 한 줄 안에 뭐가 들어갈 때 이야기 함.

        ![관련 이미지](./image_6.PNG)

- 1-6. 링크(link) & 이미지(Image)   
    
    : 특정 주소를 사용해 다른 페이지로 이동하는 링크 혹은 이미지 출력
        
    : 단, 이미지의 너비와 높이는 마크다운으로 조절할 수 없음(HTML 필요)

    : markdown의 파란 글씨의 구글을 클릭하면, 해당 사이트로 연결됨

    ![관련 이미지](./image_7.PNG)

    : ! 와 이미지를 통해 사진을 불러올 수 있음

    ![관련 이미지](./image_8.PNG)

- 1-7. 글자의 형식
    
    : **, *, ~~ 활용해서 변형 가능하다.

    ![관련 이미지](./image_9.PNG)

- 1-8. 문단의 형식

    : ---를 통해 문단을 나눌 수 있다.

    ![관련 이미지](./image_10.PNG)

    ---
## CLI?

> **1. CLI란?**
   
- Command LineInterface로, 명령어를 통해 사용자와 컴퓨터가 상호 작용하는 방식

> **2. CLI와 GUI의 비교**

- CLI는 only text로만 가능(왼 - GUI, 오 - CLI)

    ![관련 이미지](./image_11.PNG)

    : CLI 창에서  "touch" 함수를 통해 새로운 파일을 만들어낼 수 있음

    - 왜 사용해야 할까?

        :  GUI는 CLI에 비해 사용하기 쉽지만 단계가 많고 성능을 상대적으로 더 많이 소모

        : 수 많은 서버/개발 시스템이 CLI를 통한 조작 환경을 제공함
    
        : 아마 비용 측면에 있어서도  CLI가 더 큰 장점을 가지고 있다고 들음

> **3. CLI 실습 정리**

- pwd --> 현재 작업 중인 디렉토리 확인(print working directory)

- mkdir --> 새 디렉토리 형성

- ls --> 현재 작업 중인 디렉토리 내부의 폴더/파일 목록을 출력 

- cd --> 현재 작업 중인 디렉토리를 변경(위치 이동)(change directory)

- start --> 폴더/파일 열기(Mac에서는 open 사용)

- rm --> 파일 삭제(-r 옵션을 사용해 디렉토리 삭제)

- ls - a --> 보이지 않는 디렉토리 내부의 폴더/파일 목록을 보여줌

- rm - r --> 폴더 삭제

    ![관련 이미지](image_12.png)

    : CLI를 통한 삭제는 영구적으로 바로 삭제되는 것, 즉 휴지통에도 없다는 것을 볼 수 있음

## Git?

> **1. Git 이란?**
- 분산 버전 관리 시스템으로, 변화를 기록하고 추적하는 것

> **2. 중앙 vs 분산?**
- 중앙집중식? 

    :  중앙 서버에 저장되고 중앙 서버에서 파일을 가져와 다시 중앙에 업로드

- 분산식? 

    : 버전을 여러 개의 복제된 저장소에 저장 및 관리

> **3. 장점은?**

- 중앙 서버에 의존하지 않고도 동시에 다양한 작업을 수행할 수 있음

- 개발자들 간의 작업 충돌을 줄여주고 개발 생산성을 향상

- 중앙 서버의 장애나 손실에 대비하여 백업과 복구가 용이

- 인터넷에 연결하지 않고도 가능하다?

> **4. Git의 역할은?**
- 코드의 버전(히스토리)를 관리 개발되어 온 과정 파악하여 이전 버전과의 변경 사항 비교 가능

> **5. Git의 3가지 영역은?**
- working directory, staging area, repository

    1. working directory

        : 실제 작업을 하는 공간

     2. staging area

        : working directory에서 변경된 파일 중, 다음 버전에 포함시킬 파일들을 선택적으로 추가하거나 제외할 수 있는 중간 준비 영역
    
     3. repository

        : 버전 이력과 파일들이 영구적으로 저장되는 영역으로 모든 버전과 변경 이력이 기록
    
> **6. Git과 관련된 용어로는?**
- commit, Git init, Git add, Git commit

    - commit
    
        : 변경된 파일들을 저장하는 행위이며, 마치 사진을 찍듯이 기록한다 하여 'snapshot'이라고도 함 (= version)

    - Git init

        : 로컬 저장소 설정(초기화). git의 버전 관리를 시작할 디렉토리에서 진행

    - Git add

        : 변경 사항이 있는 것들을  staging area

    - Git commit

        : staging area에 있는 파일들을 저장소에 기록, 해당 시점의 버전을 생성하고 변경 이력을 남기는 것

     - 버전 업데이트 유사 예시는?
    
        : Google Docs

        ![관련 이미지](image_13.png)

> **7. Git 실습 정리**

- 7-0. 입력 후 저장(Ctrl+s)

    ![관련 이미지](image_git1.png)

- 7-1. git add .

    ![관련 이미지](image_g_1.png)

- 7-2. git status를 통해 확인

    ![관련 이미지](image_g_2.png)

- 7-3. git commit -m 'third commit' > 3번째 커밋을 했다는 문구 추가

    ![관련 이미지](image_g_3.png)

- 7-4. git log --oneline > 하나의 line으로 정리해줘

    ![관련 이미지](image_g_4.png)

- 7-5. git log --oneline --graph > 하나의 line으로 정리해주고 앞에 graph 표시해줘?

    ![관련 이미지](image_g_5.png)

- 7-6. commit을 작성하기 위해서는 저자의 이름과 메일 입력해야 함 > 사용자 정보 입력

    ![관련 이미지](image_g_61.png)

    ![관련 이미지](image_g_62.png)


> **8. Git의 순서**
- workingdirectory --> git add sample.txt (Untracked, Modified)

- staging area -->  git commit -m 'commit 메시지' (New file, modified)

- repository --> (Nothing to commit, working tree clean)

    : 즉, git은 다음과 같은 과정을 통해 로컬 저장소 내 모든 변경사항들을 변경하고 있음

> **9. Git 과정 최종 정리**

    9-1. 바탕화면에 파일 만들기
    9-2. git init > 
    9-3. touch a.txt > 코드를 통한 txt 파일 생성
    9-4. git status > 
    9-5. git add . >
    9-6. git status >
    9-7. git commit -m 'first commit' > 첫번째 commit 반영
    9-8. git log --oneline

> **10. Git의 추가 기능 설명**

- 추후,  txt파일을 수정을 하고 저장을 했다면? --> 이를 반영하기 위한 --> 또 다시 commit 필요

- 이때, 모든 파일이 아닌 하나의 파일만 수정을 했다면 add . 이 아니라 해당 파일명 넣으면 됨(ex. add a.txt)

- commit 을 올릴 때 설명한 내용을 바꾸고 싶을 때는? >  git commit --amend-->  insert 모드로 전환(i) 누르기 --> 수정하고 싶은 부분 수정 --> esc 누르고 + :wq 하기

- git init?
    - git 로컬 저장소 내에 또다른 git 로컬 저장소를 만들지 말 것 

    - 즉, 이미 git로컬 저장소인 디렉토리 내부 하단에서 git init 명령어를 다시 입력하지 말것

    - git 저장소 안에 git 저장소가 있을 경우 가장 바깥 쪽의 git 저장소가 안쪽의 git 저장소의 변경사항을 추적할 수 없기 때문

    - 만약에, 저장소가 위와 같은 주의사항처럼 2개가 형성되었다면?

    - 하나를 없애면 OK --> rm -rf .git