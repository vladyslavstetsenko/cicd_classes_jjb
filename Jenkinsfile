pipeline {

    agent any

    options {
        timestamps ()
    }

    stages {

        stage ("Checkout") {
            steps {
                git url: 'https://github.com/ochirkov/cicd_classes_jjb.git'
            }
        }

        stage ("Test") {
            steps {
                 sh "ls -l"
            }
        }
    }
}