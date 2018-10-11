# REAME.md
#####test scala build 
bash '''
sbt compile test 
'''
or 

bash '''
sbt "test:testOnly *JsonModelSpec"
'''

#####test gitlab ci process
use .gitlab-ci.yml in project and it triggers CI process every time while someone push to repository

#####test gitlab push trigger jenkins project
setup webhooks in gitlab(push events) and also in jenkins project(trigger by push to gitlab repo)
