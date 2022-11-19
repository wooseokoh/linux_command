## 리눅스 명령어

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

mkdir - 디렉토리 생성 - p 옵션을 주면 하위 디렉토리까지 한 번에 생성 가능

```
$ mkdir test
$ ls
test/  testfolder


$ mkdir -p a/b/c/d/e/
$ ls -R a/
a/:
b/

a/b:
c/

a/b/c:
d/

a/b/c/d:
e/

a/b/c/d/e:
```

touch - 파일이나 디렉토리가 존재하지 않으면 빈 파일을 생성

```
$ touch test
$ ls -l
total 0
-rw-r--r-- 1 itholic 197121 0 11월  20 01:04 test
```

rm - 파일이나 디렉토리를 삭제

- 디렉토리를 삭제할때는 r 옵션을 주어야 한다.
- -f 옵션을 주면 사용자에게 삭제 여부를 묻지 않고 바로 삭제

```
$ ls
testdir/  test1  test2


$ rm -f test1
$ ls
testdir/  test2


$ rm -rf testdir/
$ ls
test2
```
