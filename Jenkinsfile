pipeline {

    agent any

    options {
        timestamps ()
    }

    stages {

        stage ("Checkout JJB") {
            steps {
                git url: 'https://github.com/ochirkov/cicd_classes_jjb.git'
            }
        }

        stage ("Test JJB") {
            steps {
                 sh "jenkins-jobs --conf jenkins_jobs.ini test -r jobs/ > /dev/null"
            }
        }
    }
}