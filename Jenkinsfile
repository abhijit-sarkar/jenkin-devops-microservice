pipeline{
    agent { docker { image 'maven'}}
    stages{
        stage('Build'){
            steps{
                sh "mvn --version"
                echo "Build"
            }
        }
        stage('Test'){
            steps{
                echo "Test"
            }
        }
        stage('Integration Test'){
            steps{
                echo "Integration Test"
            }
        }
    } 
    post {
        always {
            echo 'Awesome'
        }
        success{
            echo 'Success'
        }
        failure{
            echo 'Failure'
        }
    }
}