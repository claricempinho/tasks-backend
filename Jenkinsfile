pipeline {
    agent any
    stages {
<<<<<<< HEAD
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
    //    stage ('Deploy Backend') {
    //        steps {
    //             deploy adapters: [tomcat8(credentialsId: 'TomcatLoginNovo', path: '', url: 'http://localhost:8001/')], contextPath: 'tasks-backend', war: 'target/tasks-backend.war'
    //         }
    //      }
    //     stage ('API Test') {
    //         steps { 
    //             dir('api-test') {                
    //               git credentialsId: 'GitHubLogin', url: 'https://github.com/claricempinho/tasks-api-test'
    //               shell 'mvn test'
    //             }
    //         }
    //    }
    //    stage ('Deploy Frontend') {
    //        steps {
    //            dir('frontend'){
    //                git credentialsId: 'GitHubLogin', url: 'https://github.com/claricempinho/tasks-frontend'
    //                shell 'mvn clean package'
    //                deploy adapters: [tomcat8(credentialsId: 'TomcatLoginNovo', path: '', url: 'http://localhost:8001/')], contextPath: 'tasks', war: 'target/tasks.war'
    //            }
                
    //         }
    //     }
    //     stage ('Functional Test') {
    //        steps {
    //            dir('functional-test'){
    //                git credentialsId: 'GitHubLogin', url: 'https://github.com/claricempinho/tasks-functional-test'
    //                shell 'mvn test'
    //            }
                
    //         }
    //     }
    
=======
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
           stage ('Deploy Backend') {
               steps {
                    deploy adapters: [tomcat8(credentialsId: 'TomcatLoginNovo', path: '', url: 'http://localhost:8001/')], contextPath: 'tasks-backend', war: 'target/tasks-backend.war'
                }
             }
           stage ('API Test') {
               steps {                 
                      dir('api-test') {                
                      git credentialsId: 'GitHubLogin', url: 'https://github.com/claricempinho/tasks-api-test'
                      shell 'mvn test'
                    }
                }
           }
        stage ('Deploy Frontend') {
               steps {
                       dir('frontend'){
                       git credentialsId: 'GitHubLogin', url: 'https://github.com/claricempinho/tasks-frontend'
                       shell 'mvn clean package'
                       deploy adapters: [tomcat8(credentialsId: 'TomcatLoginNovo', path: '', url: 'http://localhost:8001/')], contextPath: 'tasks', war: 'target/tasks.war'
                     }
              }
        }
            stage ('Functional Test') {
               steps {
                   dir('functional-test'){
                       git credentialsId: 'GitHubLogin', url: 'https://github.com/claricempinho/tasks-functional-test'
                       shell 'mvn test'
                   }

                }
            }
>>>>>>> 1219e5f4d835e02dc5efed50596621370bbc2493
    }
}


