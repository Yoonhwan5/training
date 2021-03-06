## Basic Command  

##### 

[뒤로가기](/linux/README.md)

이번 시간에는 리눅스의 디렉터리 명령어를 살펴볼 것이다. 여기서 소개하는 명령어가 리눅스 디렉터리 명령어의 전부는 아니니 더 많은 명령어에 대해서는 따로 학습할 것을 권장한다.

---

#### 현재 디렉터리 확인하기 - pwd

```
// 형식  

pwd
```
  
```
// 사용 예  

[user1@localhost ~]$ pwd
/home/user1
[user1@localhost ~]$
```
  
#### 디렉터리 이동하기 - cd  

```
// 형식  

cd {디렉터리 명}
```
  
```
// 사용 예  

[user1@localhost ~]$ cd /tmp
[user1@localhost tmp]$ pwd
/tmp
[user1@localhost tmp]$ cd
[user1@localhost ~]$ cd lib
[user1@localhost lib]$ cd ..
[user1@localhost ~]$
```
  
#### 디렉터리 내용 보기 - ls  

```
// 형식  

ls {옵션} {서브디렉터리 or 파일명}
```

```
// 옵션  

-a : 숨김 파일을 포함하여 모든 파일 목록을 출력한다.
-d : 지정한 디렉터리 자체의 정보를 출력한다.
-i : 첫 번째 행에 inode 번호를 출력한다.
-l : 파일의 상세 정보를 출력한다.
-A : .와 ..을 제외한 모든 파일 목록을 출력한다.
-F : 파일의 종류를 표시한다(*: 실행파일, /: 디렉터리, @: 심벌릭 링크).
-L : 심벌릭 링크 파일의 경우 원본 파일의 정보를 출력한다.
-R : 하위 디렉터리 목록까지 출력한다.
```
  
```
// 사용 예  

[user1@localhost ~]$ ls
공개 다운로드 문서 바탕화면 비디오 사진 서식 음악
```
  
#### 디렉터리 만들기 - mkdir  

```
//형식  

mkdir [옵션] 디렉터리명
```
  
```
// 옵션  

-p : 하위 디렉터리를 계층적으로 생성할 때 중간 단계의 디렉터리가 없으면 자동으로 중간 단계 디렉터리를 생성하면서 전체 디렉터리를 구성한다.  
```
  
```
사용 예  

[user1@localhost ~]$ ls
공개 다운로드 문서 바탕화면 비디오 사진 서식 음악
[user1@localhost ~]$ mkdir temp
[user1@localhost ~]$ ls
공개 다운로드 문서 바탕화면 비디오 사진 서식 음악 temp
```
  
#### 디렉터리 삭제하기 - rmdir  

```
// 형식  

rmdir [옵션] 디렉터리명
```
  
```
// 옵션  

-p : 지정한 디렉터리를 삭제한 뒤, 그 디렉터리의 부모 디렉터리가 빈 디렉터리일 경우 부모 디렉터리도 자동으로 삭제한다.
```
  
```
// 사용 예  

[user1@localhost ~]$ ls
공개 다운로드 문서 바탕화면 비디오 사진 서식 음악 temp
[user1@localhost ~]$ rmdir temp
[user1@localhost ~]$ ls
공개 다운로드 문서 바탕화면 비디오 사진 서식 음악
```

