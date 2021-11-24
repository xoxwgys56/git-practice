# Remove commit

[stackoverflow](https://stackoverflow.com/questions/1338728/delete-commits-from-a-branch-in-git)  
많은 생략이 포함되어 있으니, 원본 글을 참조하자.   

## remove local commit

1개의 커밋 지우기

```shell
git reset --hard HEAD~1
```

혹은 1개 이상의 커밋을 지울 수 있다.  
*hash id*는 `git log` 명령으로 커밋 로그 중에서 확인할 수 있다.  

```shell
git reset --hard <sha1-commit-id>
```

## apply to remote repo

```shell
git push origin HEAD --force
```

