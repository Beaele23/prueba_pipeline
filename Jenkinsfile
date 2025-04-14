pipeline {
    agent any
    stages {
        stage('Clonar repositorio') {
            bat {
                git branch: 'main', url: '<URL_DE_TU_REPOSITORIO>'
            }
        }
        stage('Instalar dependencias') {
            bat {
                sh 'npm install'
            }
        }
        stage('Iniciar servidor') {
            bat {
                sh 'node app.js &'
            }
        }
    }
}
