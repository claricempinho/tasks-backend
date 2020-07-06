pipeline {
    agent any
    stages {
        stage ('Just Test') {
            steps {
                shell 'echo Deu certo!'
            }
        }
        stage ('Build Backend') {
            steps {
                shell 'mvn clean package -DskipTests=true'
            }
        }        
        stage ('Unit Tests') {
           steps {
                shell 'mvn test'
           }
        }
 
    }
}


