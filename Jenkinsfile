pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build completed'
            }
        }
        stage('Test') {
            steps {
                echo 'Test completed'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment completed'
            }
        }
    }
}
post {
        always {
           
           emailext body: 'pipeline status', subject: 'failed build', to: 'ravirajmcet@gmail.com'
    }
}
