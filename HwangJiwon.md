띠용
[티지윙 홈페이지](http://tgwing.kr)
## 글씨가 크게 나타난데



<fork, pull request>

fork 해서 다른사람의 프로젝트를 내 rep로 가져와서 작업 후
pull request 보내면 된다.

git flow : branch 통한 협업
github flow : pull request 통한 협업 (github trend)
-> 참여를 하구싶오 : master copy를 내 rep로 fork
-> 개발하는동안 다ㅣ른사람들도 개발해서 코드가 많이 다름
-> rebase


<rebase>

내 마스터 copy : upstream

git remote add upstream github.com/upstream계정/~
-> upstream의 최신을 pc에 적용하고 싶으면
-> git pull upsteam master


rebase :

1,2,3,4, /1,2, /1,2,5
git fetch upstream    
        -> upstream의 master의상태를 내 rep어딘가에 저장해놓는다.(1,2,3,4)
git rebase --interactive upstream/master

-----> 지금까지 나의 commit 들이 나온다.
       --interactive를 사용해야 나온다.
       -> p,r,e,s,,f,x,d 사용해서 rebase 진행
          squash : 커밋 5를 커밋4에 녹임->새로운 -m
          (fix up은 squash에서 4의 커밋메세지로 적용)
[준영오빠rebase블로그](https://sungjunyoung.github.io/git-rebase)
