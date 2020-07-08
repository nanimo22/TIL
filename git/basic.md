

# Git basic command

> git 명령어 기초 정리



### init 

- 초기에 폴더를 깃으로 관리하겠다 라고 선언하는 명령어
- 현재 폴더에 `.git/`폴더가 생성된다.
- 그렇다면 init 을 취소하기 위해서는? `rm -r`을 이용해서 `.git`폴더를 삭제한다.  



### add

- 중간(임시) 저장 (working directory area에 있는 것을 stage area로 올려주는 것)

- `git.add .` 명령어를 통해 전체 파일을 한번에 add 할 수 있다.

  ![add](basic.assets/add.png)

### commit

- add 되어 있는 파일을 하나의 버전으로 묶어주는 명령어
- `-m`옵션으로 커밋메시지를 입력할 수 있다. (말이 옵션이지 거의 필수)



### push

- 로컬에 있는 커밋기록을 원격저장소로 업로드한다. 

```shell
$ git push origin master			
```

-> "야 깃! origin 위치로 master를 옮겨주라~ "

### remote

- 내가 `git init` 으로 git과 연결하겠다고 작정한 폴더와 인터넷 상의 내 git을 연결해 주는 것

```shell
$ git remote add origin https://github.com/nanimo22/...git
```

-> "야 깃! 원격 저장소를 추가해줘. origin이라는 이름으로. 근데 https:// ... 이곳에 있는 것을 "



### config 알아서 정리하샘)



### clone

- 원격 저장소에 있는 프로젝트를 복제하는 명령어
- 맨 처음 아예 한번도 한 적 없을 때는 clone을 사용하고, 그 이후에는 pull 사용하면 되겠지요

```shell
$ git clone <원격저장소 주소>
```



### pull

![여러대의 컴퓨터와 Git 연결](basic.assets/a.PNG)

- 원격 저장소에서 최근 커밋을 불러오는 명령어: Github -> my home 으로 가져오는게 pull

