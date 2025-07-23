pipeline {
  agent none
  stages {
    stage('Back-end') {
      agent {
        docker { image 'maven:3.8.1-adoptopenjdk-11' }
      }
      steps {
        sh 'mvn --version'
      }
    }

    stage('Front-end') {
      agent {
        docker { image 'node:16-alpine' }  // ❗ fixed space issue here
      }
      steps {
        sh 'node --version'
      }
    }
  }
}


}
}


}
