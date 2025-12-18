pipeline {
    agent any
    
    // AJOUTE CETTE SECTION pour utiliser Maven configuré dans Jenkins
    tools {
        maven 'MAVEN_HOME'  // C'est le NOM que tu as donné dans la config Jenkins
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Bonjour, ceci est mon premier pipeline Jenkins!'
            }
        }
        stage('Test Maven') {
            steps {
                // Utilise 'bat' pour Windows, mais avec Maven configuré
                bat 'mvn --version'
            }
        }
    }
}
