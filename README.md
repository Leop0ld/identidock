Docker Practice
===

마지막으로 실행한 컨테이너를 중지 및 삭제하는 방법
```
$ docker stop $(docker ps -lq)
$ docker rm $(docker ps -lq)
```

노출된 포트로 자동 매핑시키는 방법
```
$ docker run -d -P --name port-test NAME
```

자동 매핑된 포트를 확인하는 방법
```
$ docker port port-test
```
