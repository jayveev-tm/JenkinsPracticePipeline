pipeline{
    agent any
    stages{
        stage("LogIn"){
            environment{
                ACCESS_KEY  = credentials('AWS_AK')
                SECRET_KEY  = credentials('AWS_SK')
                REGION      = credentials('AWS_REGION')
            }
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
