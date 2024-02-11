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
}