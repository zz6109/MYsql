#### MYsql
### 오늘 수업 내용 정리
## 개요
# - DBMS: DataBase Management System
# - IP: 127.0.0.1은 자기 자신을 뜻한다.
# - 서버에 따른 port번호는 정해져 있다.
# - well known port를 검색하면 각 포트번호에 대한 정보를 알수있다.
# - 터미널에서 netstat -tnlp 명령으로 연결된 포트번호를 볼수 있다.
# - 같은 아이피에서 포트넘버만 달라지는것은 포트포워딩 방식이다.
# - 리눅스에서는 mysql에 root에 접근할수 없다.(할수 있긴한데 오류남)

## 데이터 베이스 및 유저 추가
# - create database 데이터베이스;
# - create user 이름@localhost identified by '이름';
# - grant all privileges on 데이터베이스. * to 이름@localhost;
# - commit;

## mysql 명령어
# - show (databases, help...); 	목록을 볼수 있다.
# - create (database, user...);	새롭게 생성할 수 있다.

## 터미널 mysql관련 명령어
# - sudo mysql -u root -p : mysql 프롬프트 접근
# - sudo systemctl start/stop/restart mysql : 프로그램 실행 및 종료
# - sudo ufw allow 프로그램명 : 방화벽에서 프로그램을 예외로 지정
# - sudo ufw enable/disable : 방화벽 켜기/끄기
# - sudo apt-get remove --purge mysql* : mysql에 관련된 파일들을 환경변수에 상관없이 삭제
# - --purge : 환경변수 무시

## mysql 삭제관련 기타사항
# - sudo rm -rf /etc/mysql /var/lib/mysql	: 하위폴더 삭제
# - sudo rm -rf /var/log/mysql			: 하위폴더 삭제
# - sudo rm -rf /var/log/mysql.*		: 하위폴더 삭제
# - sudo rm /var/lib/dpkg/info/*		: 하위폴더 삭제
# - sudo apt-get autoremove			: 관련된 쓰레기 파일 자동 삭제
# - sudo apt-get autoclean			: 자동 최적화
