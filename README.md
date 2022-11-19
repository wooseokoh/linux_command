리눅스 명령어

- SHELL
- 사용자 - OS : 컴퓨터와 대화하기 위해서 필요한 언어

pwd - 현재 작업중인 디렉토리 정보 출력

```
$ pwd
/d/linux
```

ls - 디렉토리 목록 확인

```
$ ls
testfile1  testfile2  testfile3


$ ls -l
total 0
-rw-r--r-- 1 root 197121 0 11월  6 22:08 testfile1
-rw-r--r-- 1 root 197121 0 11월  6 22:08 testfile2
-rw-r--r-- 1 root 197121 0 11월  6 22:08 testfile3


$ ls -a
./  ../  testfile1  testfile2  testfile3


$ ls -al
total 4
drwxr-xr-x 1 root 197121 0 11월  6 22:08 ./
drwxr-xr-x 1 root 197121 0 11월  6 22:08 ../
-rw-r--r-- 1 root 197121 0 11월  6 22:08 testfile1
-rw-r--r-- 1 root 197121 0 11월  6 22:08 testfile2
-rw-r--r-- 1 root 197121 0 11월  6 22:08 testfile3

d : 폴터
- : 파일
```

cd - 경로 이동

```
$ cd was/

$ pwd
/d/was
```
