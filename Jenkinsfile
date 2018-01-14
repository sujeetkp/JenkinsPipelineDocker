pipeline {
    agent {
        docker{
          image 'ubuntu'
          label 'slave'
          args '--name UbuntuContainer'
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
            }
        }
        stage('Deploy') {
            steps {
               sh 'echo Deploy'
            }
        }
    }
}
