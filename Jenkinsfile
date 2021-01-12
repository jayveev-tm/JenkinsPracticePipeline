pipeline{
    agent any
    stages{
        stage("LogIn"){
            steps{
                sh './login.sh'
            }
        }
        stage("Query"){
            steps{
                sh './query.sh'
            }
        }
        stage("LogOut"){
            steps{
                sh './logout.sh'
            }
        }
    }
}
