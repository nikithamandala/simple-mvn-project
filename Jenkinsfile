pipeline {
    agent any
    tools { 
        maven 'MAVEN_HOME' 
        jdk 'JAVA_HOME' 
    }
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
            }
        }

        stage ('Build') {
            steps {
                sh 'mvn clean install -DskipTests=true'
            }
        }
        stage ('Build') {
            steps {
                sh 'mvn clean install -DskipTests=true'
            }
        }
    }
}
