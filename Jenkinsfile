node {
  /* Requires the Docker Pipeline plugin to be installed */
  docker.image('node:8-alpine').inside {
    stage('Checkout') {
      def scmInfo = checkout scm
      echo $scmInfo
    }

    stage('Node info') {
      sh 'node --version'
    }
  }
}