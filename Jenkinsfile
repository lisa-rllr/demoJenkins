pipeline {
   
    agent any
   
    stages {

        stage('get code from bitbucket') {
            steps {
                echo 'Pulling...';
                git branch: 'master',
                url : 'https://lisa-rllr@bitbucket.org/lisa-rllr/linktojenkins.git';
            }

            post {
                success {
                    echo "====++++success++++===="
                }
               
                failure {
                    echo "====++++failed++++===="
                }
            }
           
        }
           
    }
}
