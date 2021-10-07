## Assignment 1

기존 상황

![image](https://user-images.githubusercontent.com/68385605/136369992-2b5a50a1-c7e9-4feb-aee9-a63b34bd6bec.png)

rebase 를 통해 test 브랜치 커밋을 master 브랜치 뒤로 붙인다.
```json
git checkout test
git rebase master
``` 
로컬과 remote 를 동기화한다. 
```json
git push origin test --force
```
여기까지 작업하면 해당 그림이다.


![image](https://user-images.githubusercontent.com/68385605/136370039-33f930a7-57f2-49de-a03a-b6439361baed.png)

test 의 내용을 쫒아가기 위해 merge 한다.

```json
git merge test
```

![image](https://user-images.githubusercontent.com/68385605/136370241-b012fec9-4065-48a3-9a1e-708ecc684155.png)

origin 과 동기화 한다. 

```json
git push origin master
```
![image](https://user-images.githubusercontent.com/68385605/136370406-27bc9e1e-0665-4382-b31b-68cce1412fed.png)

assignment 1 완료.
