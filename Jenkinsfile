pipeline {
    agent any
    environment {
        PATH = "$PATH:$HOME/workspace/ci-tools_master/linux_amd64:$HOME/.poetry/bin"
        WHATEVER = "git --version"
        CC = """${sh(
                returnStdout: true,
                script: 'ls'
            )}""" 
    }
    stages {
        stage('Build') {
            steps {
                echo "test1"
                echo "$WHATEVER"
                sh "MYVAR=sasf"
                echo "Jetzt kommt"
                println "pwd".execute().text
                echo "Der Inhalt ist"
                echo "$CC"


            }
        }
    }
}
