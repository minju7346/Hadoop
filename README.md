# Hadoop Mapreduce 
파이썬로 작성된 맵과 리듀서 파일을 통해 e-book에 맵리듀스 동작을 테스트하였습니다.

Mapper 파일 : mapreduce/mapper.py
Reducer 파일 : mapreduce/reducer.py

# <프로젝트 과정>

1. 위 두 파일을 이용하여 다운받은 e-book.txt파일을 맵 리듀싱
2. 이를 통해 나온 output파일은 HDFS에 저장
3. 'copyToLocal'명령어를 통해 HDFS에 있는 output파일을 로컬로 복사하여, mapreduce/output에 'part00000'로 저장

출처: input 파일 - www.gutenberg.org

# <우분투 상에서 Github 연결 및 사용법>

1. 깃허브에서 Settings>Developer setiings>Personal access tokens>Generate new token클릭
2. Expiration을 'No Expration'으로 지정 및 select scopes에서 repo체크 후 generate token 선택
3. ghp_xxx로 시작하는 부분을 복사하여 저장(비밀번호 대신 사용될  access token)
4.  Repository생성
<br>
-------------------------------in Github----------------------------
<br><br>

1. 우분투를 통해 repository 연결

>git init

>git clone https://github.com/minju7346/[repo name]
<br>

2. 파일 업로드

>git add [업로드 할 파일명]

>git commit -m "커밋할 내용"

>git push

<br><br>
--------------------------- in Ubuntu--------------------------
<br><br>

+) 깃 풀리퀘스트 in Ubuntu
>git checkout master(브랜치명)

>git branch main master -f

>git checkout main

>git push origin main -f
