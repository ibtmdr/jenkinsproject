pipeline {
    agent any
    triggers {
        pollSCM('H/2 * * * *') 
    }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World 1'
            }
        }
        stage('Example2') {
            steps {
                echo 'Hello World 2'
            }
        }
        stage('Example3') {
            steps {
                echo 'Hello World 3'
            }
        }
        stage('Example4') {
            steps {
                echo 'Hello World 4'
            }
        }
    }
}
