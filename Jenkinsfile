pipeline {
    agent any
    stages {
        stage('Clonar repositorio') {
            steps {
                git branch: 'main', url: '<URL_DE_TU_REPOSITORIO>'
            }
        }
        stage('Instalar dependencias') {
            steps {
                sh 'npm install'
            }
        }
        stage('Iniciar servidor') {
            steps {
                sh 'node app.js &'
            }
        }
    }
}
