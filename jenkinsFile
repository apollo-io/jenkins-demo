#!groovy

node('node') {
   currentBuild.result = "SUCCESS"
   
   stage('Build'){
     echo 'compile code, run unit tests, code analysis, package software'
   }
   stage('Acceptance'){
     echo 'verify dependencies are installed on CI server, deploy to CI server, run acceptance tests for this module'
   }
   stage('Staging'){
     echo 'Deploy to the relevat SIT server'
   }
}
