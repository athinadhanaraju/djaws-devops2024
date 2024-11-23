pipeline {
  agent any
  environment {
    JAVA_HOME = "/usr/bin/java"
  }
  parameters {
    choice choices: ['dev', 'sit', 'pt', 'prod'], name: 'ENV'
  }
  stages {
    stage('welcome note') {
      steps {
        script{
          subject="jenkinspac"
          println "value of the subject is ${subject}"
          // Working with predefined variables
          println "my workspace is ${WORKSPACE}"
          println "my build no is ${BUILD_NUMBER}"
          // environment variables
          println "my java home environment values are ${env.JAVA_HOME}"
          // parameters variables
          println "my env values is ${params.ENV}"
        }
      }
    }
  }
}
