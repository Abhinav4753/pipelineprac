pipeline{

    agent any
    stages{
        stage("Compile"){
            sh 'javac Test.java'
        }
        stage("run"){
            sh "java Test"
        }
    }
}