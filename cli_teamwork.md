# 생활코딩 GIT - CLI협업

## 1. Git == 협업의 도구

* Branch의 개념 필수



## 2. A와 B가 협업

### 2-1. A가 먼저 작업을 한다.

	##### 1. A가 work.txt 파일을 만들고 '1'이라고 문서 작성

##### 2. work.txt 파일을 `add` -> `commit`

##### 3. Github 활용 시작

##### 4. 원격 저장소 생성 -> 원격 저장소와 연결

```
git remote add origin [저장소 주소]
```

###### 	origin : 저장소 별명  __->이걸 까먹었다면? 다시 알아내는 방법은 뭘까?__

##### 5. `push`하여 저장소에 파일 백업

```
git push origin master
```



### 2-2.  동료 B가 합류한다.

##### 1. 권한 설정

###### 	`Settings` -> `Collaborators & teams` -> 동료 B의 github ID 추가 -> e-mail 인증 -> 협업 시작

`permission level` 설정 : Admin / Write / Read

##### 2. 동료B의 환경 세팅

```
git clone [협업 원격 저장소 주소]
```

######	`clone`은 맨 처음에 저장소를 가져올 때만 사용. 그 이후에는 `pull`.



### 2-3. 협업 시작

##### 1. 같은 시간에 같은 파일의 같은 부분을 수정하는 __conflict(충돌)__이 발생한다면?

##### 	`git push`를 거절당한다면, 다시 `git pull`을 하여 충돌이 생기지 않도록 다시 정리해야한다.

##### 2. `git merge`를 하거나 파일을 열어 엉킨 부분을 수정해야 한다.

##### 3. 고쳐진 파일을 다시 `git add` -> `git commit`을 한다.

##### 4. 다시 `git push`한다.

##### __5. 결론 : 최대한 작업을 빨리 끝내고, `push`를 자주 해야 서로 충돌이 일어나지 않는다. 작업을 하기 전에 무조건 먼저 `git pull`을 해야한다.__



## 3. 

* git pull -> git commit -> git push
* git fetch -> git merge FETCH_HEAD -> git commit -> git push



## 4. 





