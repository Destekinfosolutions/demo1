pipeline{
    agent any
    environment{
        staging_server="10.128.0.2"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
                sh 'scp -r ${WORKSPACE}/* root@${staging_server}:/var/www/html/'
                   
              
            }
        }
    }
}
