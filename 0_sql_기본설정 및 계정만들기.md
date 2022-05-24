# 기본설정 및 계정만들기


###  주석
```
-- 주석
/*
블럭주석
control + /
*/
show databases;  -- ; : 명령어종료, 실행 : control +enter
use mysql;
```

### 데이터베이스를 생성
```
create database hr;
```
### 데이터베이스 확인
```
show databases;  # mysql명령어
```
### 데이터베이스 삭제
```
drop database hr;
```
### hr 데이터베이스를 사용
```
use hr; # mysql 명령어
```

### 계정 생성 - scott - tiger
```
create user scott@localhost identified by 'tiger'; -- 로컬에서 접속할 수 있는 계정
create user scott@'%' identified by 'tiger'; -- 원격 접속 계정
```

### scott 계정에 모든 권한을 부여
```
grant all privileges on *.* to scott@localhost;
grant all privileges on *.* to scott@'%';


show databases;
use mysql;
select host, user from user;

use mysql;
show tables;
```
