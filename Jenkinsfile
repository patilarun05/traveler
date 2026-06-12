pipeline {

    agent any
    tools {
        maven 'Apache Maven 3.9.16'
    }
    stages {
        stage ('Code compile') {
            steps {
                echo "Code compilation starts"
                sh 'mvn clean compile'
                echo "Code compilation completed"
            }
        }
        stage ('Code package') {
            steps {
                    echo "Code packaging starts"
                    sh 'mvn clean package'
                    echo "Code packaging completed"
            }
        }
    }

}