pipeline {
    agent {
        dockerfile{
          label 'slave'
        }
    }

    stages {
        stage('Build') { 
            steps { 
               sh 'echo Build'
               sh 'hostname'
            }
        }
        stage('Test'){
            steps {
                sh 'echo Test'
                sh 'hostname'
            }
        }
        stage('Deploy') {
            steps {
               sh 'echo Deploy'
               sh 'cat /var/www/html/index.html'
            }
        }
    }
}
