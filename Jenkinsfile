pipeline {
    agent any
    stages {
        stage("Git CheckOut"){
            when {
                branch "develop"
            }
            steps {
                echo " Checking out code from git"
            }
        }

        stage("Maven Build"){
            when {
                branch "develop"
            }
            steps {
                echo " Maven build finished ..."
            }
        }

        stage("Dev Deploy"){
            when {
                branch "develop"
            }
            steps {
                echo " Successfully deployed to Dev Server"
            }
        }

        stage("Production Deployment"){
            when {
                branch "main"
            }
            steps {
                echo " Successfully deployed to Production Server"
            }
        }
    }
}