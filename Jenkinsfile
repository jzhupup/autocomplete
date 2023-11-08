pipeline {
  agent any
  stages {
    stage('阶段 1-1') {
      steps {
        junit 'target/surefire-reports/*.xml'
        useCustomStepPlugin(key: 'SYSTEM:artifact_maven_push', version: '1.1', params: [deployFile:true,repoUrl:'https://replace123-maven.pkg.coding.net/repository/demo/test-maven'])
      }
    }
  }
}