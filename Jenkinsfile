pipeline{
    agent any
    stages{
        stage('checkout'){
            steps{
                deleteDir()
                sh '''
                    git clone https://github.com/shemil-fahad/git-action-sample.git
                    ls -l
                '''
            }
        }
        stage('deploy'){
            steps{
                sh '''
                    cp -r git-action-sample/* /var/www/html
                    ls -l /var/www/html
                '''
                    
            }
        }
        
    }
}
