pipeline {
    agent any

    stages {
        stage(' Build') {
            steps {
                echo 'Build App'
            }
        }
    
        stage('Test') {
            steps {
                echoo 'Test App'
            }
        }
    
        stage('Deploy') {
            steps {
                echo 'Deploy'
            }
        }
    }
    
    post 
    {
        always
        {
            emailext body: 'Summary', subject: 'Jenkins Pipeline', to: 'pabbakalyan008@gmail.com'
        }
    }
}
