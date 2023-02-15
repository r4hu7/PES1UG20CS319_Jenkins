pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ pes1ug20cs319.cpp -o pes1ug20cs319'
                 build job: 'PES1UG20CS319-1', wait: false
                 echo 'Build successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat pes1ug20cs319.cpp'
                echo 'Test successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
