pipeline{

    agent any
    stages{
        stage("Compile"){
            steps{
                sh 'javac Test.java'
            }
        }
        stage("run"){
            steps{
                sh "java Test"
            }
        }
    }
}