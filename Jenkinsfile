node {

  /* Requires the Docker Pipeline plugin to be installed */
  docker.image('node:8-alpine').inside {

    def scmInfo

    stage('Checkout') {
      scmInfo = checkout scm
    }

    stage('Node info') {
      echo scmInfo
      sh 'node --version'
    }

  }

}