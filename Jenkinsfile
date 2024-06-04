pipeline{
    agent any
    environment{
        staging_server="20.198.17.30"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
                sh 'scp -r ${WORKSPACE}/* root@${staging_server}:/var/www/html/'
                   
              
            }
        }
    }
}
