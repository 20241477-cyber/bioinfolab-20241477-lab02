# Codespace 사용 확인 답안
 
학번 : 20241477
이름 : 이성연
 
## 2-1. 아이콘 정리
 
| 순서  |   아이콘 이름  |     모양         |                         하는 일                       |
|------|----------------|------------------|------------------------------------------------------|
| 1    |     탐색기     |  파일 모양         | 파일과 폴더를 관리하고, 확인하는 역할을 한다.           |
| 2    |      검색      |  돋보기 모양       | 파일 안에 있는 단어 및 내용을 검색하는 역할을 한다.      |
| 3    |   소스 제어     |  가지 모양        | 파일 변경 사항을 확인하고 commit, push하는 역할을 한다.  |
| 4    |  실행 및 디버그 |  파일 모양        | 프로그램을 실행하고 오류를 찾아보는 역할을 한다.          |
| 5    |      확장      | 네모 블록 4개 모양 | VS code의 확장프로그램을 설치하고 관리한다.             |
 
## 2-2. 가. 파일 탐색기

'ls lab02' 실행결과 : data  doc  src  test

이 작업으로 알 수 있는 점 :
Explorer에서 만든 test 폴더가 실제로 lab02폴더 안에 생성된 것을 확인할 수 있다.
 
## 2-2. 나. 검색
 
대소문자 구분을 껐을 때 : 400 results in 2 files
대소문자 구분을 켰을 때 : 399 results in 1 files

완전한 단어 검색을 껐을 때 : 400 results in 2 files
완전한 단어 검색을 켰을 때 : 386 results in 2 files

$ grep -o -i "Alice" lab02/data/alice.txt | wc -l 결과 : 399

검색 결과 중 grep 결과와 대소문자 구분을 켰을 때의 결과가 동일하였다.
따라서 대소문자 구분을 킨 것으로 grep에서 검색한 것 같다고 생각된다.

## 2-2. 다. 소스 제어

소스제어 아이콘 위에 쓰여있는 숫자는 변경된 파일의 수를 의미한다.

변경된 파일 수 : 2 (answers.md와 README)

git log -1의 결과 :

Author: lee seongyeon <20241477@sungshin.ac.kr>
Date:   Tue Sep 8 05:53:21 2026 +0000

    answer
 
나는 terminal로 commit하는 것보다 화면에서 commit하는 것이 더욱 편했다.
terminal은 실행 후에 따로 commit을 하지만 화면에서 하는 경우 파일의 변경 사항을 눈으로 확인하면서 commit할 수 있기 때문에
더욱 보기쉽고 편리하다고 느꼈다.

## 2-2. 라. 확장

Python의 확장 이름 : ms-python.python
Python의 버전 번호  : 2026.4.0

Jupyter의 확장 이름 : ms-toolsai.jupyter
Jupyter의 버전 번호 : 2025.9.1

두 확장은 강의자가 미리 넣어둔 것이라고 생각한다.
그 이유는 .devcontainer/json에 ms-python.python과 ms-toolsal.jupyter가 미리 지정되어 있으므로,
학생이 직접 설치한 것이 아니라 강의에서 제공한 Codespace 환경에 미리 설정되어있던 것이라고 생각한다.