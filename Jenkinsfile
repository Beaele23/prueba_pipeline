pipeline {
    agent any
    stages {
        stage('Clonar repositorio') {
         steps {
                git branch: 'main', url: 'https://github.com/Beaele23/prueba_pipeline.git'
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
