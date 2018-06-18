pipeline {
  options {
    // Keep 5 builds history
    buildDiscarder(logRotator(numToKeepStr: '5'))
  }

  agent {
    node {
      label 'c7-sphinx'
    }
  }

  stages {
    stage('Package') {
      steps {
        withMaven(
          // Maven installation declared in the Jenkins "Global Tool Configuration"
          maven: 'apache-maven-3.0.5' ) {
            sh 'mvn -B deploy'
        }
      }
    }
  }
}
