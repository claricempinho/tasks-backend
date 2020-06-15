pipeline {
    agent any
    stages {
        stage ('Just Test') {
            steps {
                shell 'echo Deu certo!'
            }
        }
        stage ('Unit Tests') {
           steps {
                sh 'mvn test'
           }
        }
        // stage ('Deploy Backend') {
        //     steps {
        //         deploy adapters: [tomcat8(credentialsId: 'TomcatLoginNovo', path: '', url: 'http://localhost:8001/')], contextPath: 'tasks-backend', war: 'target/tasks-backend.war'
        //     }
        // }
    }
}


