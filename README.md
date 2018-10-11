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
![Image of Yaktocat](https://www.google.com/url?sa=i&rct=j&q=&esrc=s&source=imgres&cd=&cad=rja&uact=8&ved=2ahUKEwiHmovw5P3dAhW-ITQIHQZAC48QjRx6BAgBEAU&url=http%3A%2F%2Fwww.docker.org.cn%2Fdocker%2F71.html&psig=AOvVaw0ImbFYkRPXsz3A2gy1LZI0&ust=1539326673902288)

##### test gitlab push trigger jenkins project
> setup webhooks in gitlab(push events) and also in jenkins project(trigger by push to gitlab repo)

