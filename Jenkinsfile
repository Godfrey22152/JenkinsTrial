def gv

pipeline {
    agent any

    stages {
        stage("init") {
            steps {
                script {
                    gv = load "script.groovy" // This loads the script, but may not be suitable for loading an object
                }
            }
        }
        stage("Build") {
            steps {
                script {
                    gv.buildApp() // Assuming gv is an object with a method buildApp()
                }
            }
        }
        stage("Test") {
            steps {
                script {
                    gv.testApp() // Assuming gv is an object with a method testApp()
                }
            }
        }
        stage("Deploy") {
            steps {
                script {
                    gv.deployApp() // Assuming gv is an object with a method deployApp()
                }
            }
        }
    }
}
