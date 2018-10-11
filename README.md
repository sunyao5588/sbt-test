# README.md
##### test scala build 
```
sbt compile test 
```
or 

```
sbt "test:testOnly *JsonModelSpec"
```

##### test gitlab ci process
> use .gitlab-ci.yml in project and it triggers CI process every time while someone push to repository
In this project use docker image to set up sbt build environment and use local host directory to store liberies project needed in order to save time from downloading libs everytime while building.
> trying to make everything in docker!!
![Image of Yaktocat](http://article.fd.zol-img.com.cn/t_s640x2000/g5/M00/03/03/ChMkJ1XRn7qIVAbsAAF-AuKsabEAAAMxQMXeB0AAX4a192.png)

##### test gitlab push trigger jenkins project
> setup webhooks in gitlab(push events) and also in jenkins project(trigger by push to gitlab repo)

