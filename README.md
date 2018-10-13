# How to use CI to fasten your project?
## what happened after "git push" ?

> GitLab has integrated CI/CD pipelines to build, test, deploy, and monitor your code.
                
One of the available gitlab-runners will be captured to run CI script(compile/package/test/deploy). These gitlab-runners are placed on separate users, servers, containers and even on your local machine.

These are two kinds of gitlab runner. One is Shared Runners which are free to use for public open source projects and limited to 2000 CI minutes per month per group for private project on [gitlab.com](https://gitlab.com) and another one is Specific Runners which are specific for group projects.

![Alt text](/Users/sunyao/workspace/pwc-workspace/Other/used/runners.png)



```
sbt compile test 
```
or 

```
sbt "test:testOnly *JsonModelSpec"
```

## test gitlab ci process
> use .gitlab-ci.yml in project and it triggers CI process every time while someone push to repository
In this project use docker image to set up sbt build environment and use local host directory to store liberies project needed in order to save time from downloading libs everytime while building.
> trying to make everything in docker!!
![Image of Yaktocat](http://article.fd.zol-img.com.cn/t_s640x2000/g5/M00/03/03/ChMkJ1XRn7qIVAbsAAF-AuKsabEAAAMxQMXeB0AAX4a192.png)

##### test gitlab push trigger jenkins project
> setup webhooks in gitlab(push events) and also in jenkins project(trigger by push to gitlab repo)

