pipeline {
  volumes: [
  persistentVolumeClaim(
      mountPath: '/root/.m2/repository', 
      claimName: 'jenkins-pv-claim', 
      readOnly: false
      )
  ])
 
  {
    stages {
        stage('Get a Maven project') {
            steps {
                sh 'uname -a'
                sh 'echo Getting maven!'
            }
        }
    }
  }
}