pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG20CS472.cpp'
                sh 'g++ -o PES1UG20CS472 PES1UG20CS472.cpp'
                echo 'Build Stage worked Successfully'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS472'
                echo 'Test Stage Successfully Executed '
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployment was Successfull'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline Failed'
        }
    }
}
