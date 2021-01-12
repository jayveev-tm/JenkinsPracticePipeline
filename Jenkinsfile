pipeline{
    agent any
    stages{
        environment{
            ACCESS_KEY  = credentials('AWS_AK')
            SECRET_KEY  = credentials('AWS_SK')
            REGION      = credentials('AWS_REGION')
        }
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
