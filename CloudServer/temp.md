##scp를 이용한 파일업로드
scp -i D:\cosmos\Key\booksplus.pem C:\Users\schiz\Downloads\triangle03.py ubuntu@ec2-52-79-235-4.ap-northeast-2.compute.amazonaws.com:/home/ubuntu

(아래는 구조 분해분석)

scp -i

 D:\cosmos\Key\booksplus.pem

 C:\Users\schiz\Downloads\triangle03.py

 ubuntu@ec2-52-79-235-4.ap-northeast-2.compute.amazonaws.com:/home/ubuntu

##scp를 이용한 파일 다운로드
scp -i D:\cosmos\Key\booksplus.pem ubuntu@ec2-52-79-235-4.ap-northeast-2.compute.amazonaws.com:/home/ubuntu/triangle03.py C:\Users\schiz\Downloads


##root디렉토리 접근
처음 로긴후 들어갈때 생성한 유저로 들어가기 때문에 root 폴더에 접근을 할 수 없다.

이럴 경우엔

sudo passwd root 라고 치고 계정 비밀번호를 만들게 되면 root 계정을 사용할 수 있다.

Enter new UNIX password : [root의 비밀번호로 하고싶은 것을 입력] 

(여기서 root 계정은 리눅스의 관리자 계정을 말한다) 

root계정 들어가고 싶을 경우 su - 또는 su - root를 입력하고

나올때는 Ctrl + D를 입력하면 된다. 

(password fintech)

출처: https://psh85a.tistory.com/entry/Linux-우분투에서-root-계정으로-들어가기 [Don't lose faith]

-참고 명령어들
https://blockdmask.tistory.com/25