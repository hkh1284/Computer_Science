# 병행성 Concurrency
### 병행성이란 무엇인가?
- 여러 프로세스/쓰레드들을 동시에 처리해야하는 상황이 존재한다.
- 여러 프로세스/쓰레드들을 동시에 처리하는 것은 운영체제가 관리해야한다. 즉, 운영체제는 cncurrency 병행성(동시성)을 가져야한다.

### 병행성 제어는 무엇이고, 왜 필요한가?
- 공유자원이 있으면, 경쟁상태가 발생하고, 잘못된 결과가 발생할 수 있다.
- 잘못된 결과가 발생하지 않도록 병행성제어가 필요하다.
- 병행성 제어 : 공유자원들을 잘 약속된(동기화된) 방법으로 접근할 수 있도록 강제하는 것

### 병행성 이슈들은 어떤 것인가?
- ex) 생산자/소비자 문제, 기록자/판독자 문제, 식사하는 철학자 문제, ....

## 용어정리
  #### 1. 공유자원 shared data
  #### 2. 경쟁상태 race condition
  #### 3. 상호배제 mutual exclusion
  #### 4. 임계영역 critical section



## Thread 쓰레드
  #### 1. 쓰레드의 정의
  - 어떤 프로그램이 수행하기 위해서는 크게 3가지의 컴퓨팅 리소스가 필요
  : cpu 관련 리소스, address space 관련 리소스, file 관련 리소스
  - 컴퓨팅 리소스를 어떻게 관리하느냐에 따라 프로세스모델, 쓰레드모델로 구분.
  - 프로세스 : 하나의 프로세스는 3가지 컴퓨팅 리소스를 독립적으로 가지도록 구성.
  - 프로세스 -> code, data, files, register stack등을 모두 독립적으로 가짐
  - 쓰레드 : 하나의 쓰레드는 cpu관련 리소스는 독점적으로 가지고, 나머지는 다른 쓰레드와 공유.
  - 쓰레드 -> code, data, files, heap은 모든 쓰레드들이 공유, register, stack은 독점적으로 가짐
  - 스케줄러입장 : 프로세스나 쓰레드나 똑같은 스케줄링 객체
  - '공유냐 아니냐' : 프로세스와 쓰레드는 완전히 다른 객체
   
  #### 2. 쓰레드의 장점
  - 빠르다 : 생성할 때 레지스터와 스택만 새로 만들면 되므로 프로세스에 비해 빠르다.
  - 병행처리가 좋다 : 규모가 큰 작업을 여러개의 쓰레드가 나누어서 처리 후 합치는 방식의 작업가능
  - I/O와 컴퓨팅을 오버랩시키는 것에 쓰레드가 더 유용하다.
  - 데이터 쉐어링이 잘 된다
  
  #### 3. 쓰레드 관리
  #### 4. 쓰레드 api
  - pthread_create()
  - pthread_join()

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
  #### 1. Deadlock의 정의
  #### 2. Deadlock의 처리를 위한 3가지 접근방법 
  - Prevention예방
  - Avoidance회피
  - Detection and Recovery감지&복구
  
## 잘 알려진 병행성 문제
  #### 1. Producer생산자/Consumer소비자 문제
  #### 2. Reader기록자/Writer판독자 문제
  #### 3. Dining Philosopher 식사하는 철학자 문제
  
## Concurrency bugs 병행성 버그
  #### 1. non-deadlock bug
  #### 2. deadlock bug
  
