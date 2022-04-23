# 병행성 Concurrency
### 병행성이란 무엇인가?
### 병행성이 왜 필요한가?
### 어떻게 병행성을 구현하는가? 

## 용어정리
  #### 1. 공유자원 shared data
  #### 2. 경쟁상태 race condition
  #### 3. 상호배제 
  #### 4. 임계영역 



## Thread 쓰레드
  #### 1. 쓰레드의 정의
  #### 2. 쓰레드를 사용하는 이유
  #### 3. 쓰레드의 장점
  #### 4. 쓰레드 관리
  #### 5. 쓰레드 api
  - pthread_create(), pthread_join()

## Lock 락
  #### 1. 락의 정의
  #### 2. 락 매커니즘의 평가기준 3가지
  - correct 정확한가?(= 상호배제를 잘 보장해주는가?)
  - fair 공평한가?(= 오랫동안 수행되지 않는 기아상태의 쓰레드나 프로세스는 없는가?)
  - performance 성능은 좋은가?
  #### 3. 성능 이슈 from lock size : coarse-grained lock vs fine-grained lock
  #### 4. 락/언락 api를 실제로 구현하는 3가지 방법
  - interrupt를 disable하는 방법
  - software적인 방법
  - hardware적인 atomic operation을 활용하는 방법
  #### 5. 락의 종류 2가지 : spin lock vs sleep lock
  

## Condition variable 조건변수
  #### 1. SQMS(Single-Queue Multiprocessor Scheduling)
  #### 2. MQMS(Multi-Queue Multiprocessor Scheduling)
  
  
## Mutex 뮤텍스
  #### 1. SQMS(Single-Queue Multiprocessor Scheduling)
  #### 2. MQMS(Multi-Queue Multiprocessor Scheduling)
  

## Semaphore 세마포어
  #### 1. SQMS(Single-Queue Multiprocessor Scheduling)
  #### 2. MQMS(Multi-Queue Multiprocessor Scheduling)
  
## Deadlock 교착상태
  #### 1. SQMS(Single-Queue Multiprocessor Scheduling)
  #### 2. MQMS(Multi-Queue Multiprocessor Scheduling)
  
