pipeline {
    agent any

    stages {
        stage('Development') {
            steps {
              bat 'echo "Hello World"'
            }
        }
        
        stage('QA') {
            steps {
                bat 'git clone https://github.com/vansh-8502/sample_rep.git'
            }
        }
        
        stage('UAT') {
            steps {
                bat '''
                cd sample_rep
                echo hello > newtextfile3.txt
                '''
            }
        }
    }
}
