
# 영속성 Persistence
### 영속성이란 무엇인가?
- 컴퓨터 충돌, 디스크 장애 등에도 불구하고 정보를 지속적으로 유지
- 



## I/O Devices
- 본론(영속성)에 들어가기 전 입력/출력 장치의 개념을 알아본다.
- 운영체제가 입력/출력 장치들과 상호작용하는 방법을 알아본다.
  
  #### System Architecture 시스템구조
  #### A Canonical Device 표준장치
  #### The Canonical Protocol 표준 프로토콜
  #### Lowering CPU overhead with Interrupt 인터럽트를 이용한 CPU오버헤드 개선
  #### More Efficient Data Movement with DMA DMA를 이용한 효율적인 데이터 이동
  #### Methods of Device Interaction 디바이스와 상호작용하는 방법
  #### Fitting into the OS: The Device Driver 운영체제에 연결하기: 디바이스 드라이버
  #### Case Study: A simple IDE Disk Driver 사례연구 : 간단한 IDE 디스크 드라이버

## Hard Disk Drives
- (곧 살펴볼) 영속성을 위한 파일 시스템 기술은 하드디스크 드라이브의 동작에 기반을 두고 개발됨.
- 그러므로 하드 디스크 드라이브에 대해 자세히 알아본다.
  #### The interface 인터페이스
  #### Basic Geometry 기본 구조
  #### A Simple Disk Drive 간단한 디스크 드라이브
  #### I/O Time : Doing the Math I/O 시간 계산
  #### Disk Scheduling 디스크 스케줄링
  
## Interlude: Files and Directories
- UNIX 파일 시스템을 사용할 때 만날 수 있는 인터페이스들을 알아본다.
  #### Files and Directories 파일과 디렉토리
  #### File System Interface 파일 시스템 인터페이스
  #### Creating Files 파일의 생성
  #### Reading and Writing Files 파일의 읽기와 쓰기
  #### Reading and Writing, But Not Sequentially 비순차적 읽기와 쓰기
  #### Shared file table entries: fork() and dup() 
  #### Writing immediately with fsync() fsync()를 이용한 즉시 기록
  #### Renaming files 파일 이름 변경
  #### Getting information about files 파일 정보 추출
  #### Removing files 파일 삭제
  #### Making Directories 디렉토리 생성
  #### Reading Directories 디렉토리 읽기
  #### Deleting Directories 디렉토리 삭제
  #### Hard Links 하드링크
  #### Symbolic Links 심볼릭링크
  #### Permission Bits and Access Control Lists 
  #### Making and Mounting a file system 파일시스템 생성과 마운트

  

## File System Implementation
- vsfs라는 간단한 파일시스템을 사용하여 파일시스템의 개념에 대해 알아본다.
- 파일시스템의 실제 사례들에 대해 알아본다.
- 파일시스템이 어떻게 동작하는지 이해한다.
  #### The Way to Think 사고 방식
  #### Overall Organization 전체 구성
  #### File Organization: The inode 파일 구성: 아이노드
  #### Directory Organization 디렉토리 구조
  #### Free Space Management. 빈 공간의 관리
  #### Access Paths: Reading and Writing 실행흐름: 읽기와 쓰기
  #### Caching and Buffering 캐싱과 버퍼링
  
  
  
  
## Locality and The Fast File System (FFS)
- 
  #### Poor performance 문제: 낮은 성능
  #### FFS: Disk Awareness FFS:디스크에 대한 이해가 해답이다.
  #### Organizing Structure: The Cylinder Group 파일시스템구조: 실린더 그룹
  #### Policies: How to Allocate Files and Directories 파일과 디렉토리 할당 정책
  #### The Large-File Exception 대용량 파일 예외상황
  #### A Few Other Things about FFS FFS에 대한 기타사항
  
  
## Crash Consistency: FSCK and Journaling
  #### A Detailed Example 예제
  #### Solution #1: The File System Checker 솔루션1: 파일시스템 검사기
  #### Solution #2: Journaling (or WAL) 솔루션2: 저널링(or Write-Ahead Logging)
  #### Solution #3: Other Approaches 솔루션3: 그 외 방법
  
## Features of Various FS: Ext2/3/4, FAT, Flash FS
  #### Ext2
  #### Ext3
  #### Ext4
  #### FAT
  #### Flash-aware FS







  
