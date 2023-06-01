# 자주 사용하는 명령어
자주 사용되나 빈번히 헷갈리는 명령어+옵션 조합 정리

### kill : 인자로 지정한 프로세스에 시그널을 전달한다.
- 
- 기본 사용(디폴트=시그널15 SIGTERM, 정상종료) : kill [pid]

- 강제 종료(시그널9 SIGKILL) : kill -9 [pid]

### pkill :  => 추후에 추가로 내용보충/수정하기
- command 이름이 같은 것들 모두 종료 : pkill -x -9 [프로세스CMD]

- 

### rm -rf
- rm : 파일 삭제 명령어
- 옵션 r : 재귀적으로 하위에 있는 모든 파일 및 디렉토리 삭제를 의미함
- 옵션 f : 삭제할 때, 문제가 발생하면 파일을 삭제하지 않고 경고하는데 f는 경고 없이 삭제하도록 함


### wget
- wget : 'Web Get'의 약어로 웹 상의 파일을 다운로드 받을 때 사용하는 명령어
- 기본사용 : wget [download-url]
- 옵션 O : 다른이름으로 저장. ex) wget -O [파일명] [download-url]


### tar
- wget : 'Tape ARchiver'의 약어로 여러개의 파일을 하나로 묶거나 풀 때 사용하는 명령어
- 자주 사용되는 형태 : tar 
- 옵션 O : 다른이름으로 저장. ex) wget -O [파일명] [download-url]

### mkdir
- mkdir : 'Make Directory'의 약어로 디렉토리를 생성해주는 명령어
- 기본사용 : mkdir [생성할 디렉토리이름]
- 옵션 p : 존재하지 않는 중간의 디렉토리를 자동으로 생성해준다. ex) mkdir -p f1/f2/f3 -> f1,f2가 존재하지 않더라도 새로 생성해서 그 안에 f3를 만들어준다.


### mv
- mv : 'move'의 약어로 파일의 위치를 옮기면서 파일의 이름도 바꾸어주는 명령어
- 기본사용 : mv [기존파일경로/기존파일명] [옮기길원하는경로/변경파일명]









