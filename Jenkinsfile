pipeline{

    agent any
    stages{
        stage("Compile"){
            steps{
                echo 'javac Test.java'
            }
        }
        stage("run"){
            steps{
                echo "java Test"
            }
        }
    }
    post{
        always{
            echo"always"
        }
        success{
            echo "success"
        }
        failure{
            echo"failure"
        }
    }
}