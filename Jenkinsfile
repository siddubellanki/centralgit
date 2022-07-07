pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'build application'
            }
        }
         stage('test') {
            steps {
                echo 'test application'
            }
        }
         stage('deploy') {
            steps {
                echo 'deploy application'
            }
        }
    }
    post
   {
       always
       {
           emailext body: 'summary', subject: 'pipeline status', to: 'cddumb111@gmail.com'
       }
   }
}
