pipeline {
    agent {
        label 'DevSlave'
    }
    stages {
        stage('scm checkout'){
            echo "Pulling repo from git"
        }
        stage('maven build'){
            echo "Creating a jar file"
            sh(script: "mvn clean install -DskipTests")
        }
    }
}
