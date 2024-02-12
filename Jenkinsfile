pipeline{
    agent any
    stages{
        stage("Compile"){
            steps{
                echo 'Compiling Test.java'
                bat 'javac Test.java' // Assuming you are running on a Windows agent, use 'sh' for Unix
            }
        }
        stage("Run"){
            steps{
                echo 'Running Test.class'
                bat 'java Test' // Assuming you are running on a Windows agent, use 'sh' for Unix
            }
        }
        stage("Test") {
            steps {
                echo 'Running Tests'
                script {
                    bat(script: 'java -cp .;path/to/test/jars org.junit.runner.JUnitCore Test', returnStatus: true)
                }
            }
        }
    }
    post{
        always{
            echo 'Always executed'
        }
        success{
            echo 'Success!'
        }
        failure{
            echo 'Failure!'
        }
    }
}
