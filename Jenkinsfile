pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                sh '''
                sudo -S apt update -y
                cd Deploy-Angular-App-using-Jenkins-to-AWS-EC2
                sudo npm install
                sudo npm install -g @angular/cli
                sudo ng serve --host 0.0.0.0 --disable-host-check

            '''
            }
        }
    }