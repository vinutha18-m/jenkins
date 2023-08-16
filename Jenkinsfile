pipeline  
{
        agent any
            tools {
                    maven 'maven'
          }
        stages {
                stage('git clone') {
                        steps {
                           git 'https://github.com/vinutha18-m/jenkins.git'
                        }
                }
                stage('compile') {
                        steps {
                            sh 'mvn compile'
                        }
                }
                stage('test') {
                        steps {
                            sh 'mvn test'
                        }
                }
        }
}
