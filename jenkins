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
                git add .
                git config --global user.email "vanshsharma8502@gmail.com"
                git config --global user.name "vansh-8502"
                git commit -m "push from Jenkins"
                git push https://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@github.com/vansh-8502/sample_rep.git '''
            }
        }
    }
}
