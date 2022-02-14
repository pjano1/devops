pipeline {
    agent {
        label 'tester'
    }
    stages {
        stage('build') {
            steps {
                sh 'uname -a'
                sh 'echo main branch!'
            }
        }
    }
}
