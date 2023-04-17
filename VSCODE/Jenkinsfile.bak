pipeline {
    agent any
    triggers {
        pollSCM('H/2 * * * *') 
    }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Example Build') {
            agent { docker 'myjenkins-blueocean:2.387.1-1' } 
            steps {
                echo 'Hello, Maven'
                sh 'mvn --version'
            }
        }
        stage('Example Test') {
            agent { docker 'myjenkins-blueocean:2.387.1-1' } 
            steps {
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
}
