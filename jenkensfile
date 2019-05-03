pipeline {
    agent any
    tools {
        maven 'maven3'
    }
    stages {
        stage (checkout) {
            steps {
                git  branch: 'develop', credentialsId: '70ecb8f7-b239-431a-af07-c9049a10d012', url: 'https://github.com/di-amine/PR-MAVEN.git'
            }
        }
        stage ('stage 1') {
            environment {
                JAVA_HOME = '/usr/lib/jvm/jre-openjdk/'
            }
            
            steps {
                echo 'hello World1'brach
                echo JAVA_HOME
            }
        }
        stage ('stage 2') {
            environment {
                MAVEN_HOME = '/opt/maven'
            }
            steps {
                echo 'hello world'
                echo MAVEN_HOME
            }

        }
    }
}
