pipeline {
    agent any
     stages {
     stage('Deploy') { 
           steps {
             sh ''' #! /bin/bash 
             
              aws deploy create-deployment --application-name chatappjenkins --deployment-group-name ChatappJenkinsDBGroup --deployment-config-name CodeDeployDefault.AllAtOnce --github-location repository=Shashanksingh17/ChatApplication,commitId=${GIT_COMMIT}
             '''
            }
        }
      }
    }
