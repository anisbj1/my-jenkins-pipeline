pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Bonjour, ceci est mon premier pipeline Jenkins!'
            }
        }
        stage('Git checkout') {
            steps {
                git branch: 'main', 
                url: 'https://github.com/anisbj1/my-jenkins-pipeline.git'
            }
        }
        stage('Build avec Maven') {
            steps {
                script {
                    // Si tu n’as pas Maven installé, ça va échouer, mais c’est pour l’exemple
                    bat 'mvn --version'
                }
            }
        }
    }
}
