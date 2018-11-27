pipeline {
  agent any
    stages {
      stage('Build') {
        steps {
          awsCodeBuild projectName: 'kpetti-codebuild',
                       credentialsId: 'codebuild-jenkins-user',
                       credentialsType: 'jenkins',
                       region: 'us-east-1',
                       sourceControlType: 'project'

        }
      }
    }
}
