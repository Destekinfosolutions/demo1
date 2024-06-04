pipeline{
    agent any
    environment{
        staging_server="10.0.0.25"
    }
    stages{
        stage('Deploy to Remote'){
            steps{
                sh 'scp -r ${WORKSPACE}/* root@${staging_server}:/var/www/html/'
                   
              
            }
        }
    }
}
