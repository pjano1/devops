
podTemplate(containers: [
    containerTemplate(
        name: 'maven', 
        image: 'maven:3.8.1-jdk-8', 
        command: 'sleep', 
        args: '30d'
        )
  ],

  volumes: [
  persistentVolumeClaim(
      mountPath: '/root/.m2/repository', 
      claimName: 'jenkins-pv-claim', 
      readOnly: false
      )
  ])
 
  {
    node(POD_LABEL) {
    stages {
        stage('build') {
            steps {
                sh 'uname -a'
                sh 'echo main branch!'
            }
        }

    }
  }