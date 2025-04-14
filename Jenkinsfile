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
                bat 'npm install'
            }
        }
        stage('Iniciar servidor') {
            steps {
                bat 'node app.js &'
            }
        }
        stage('Ejecutar pruebas') {
           steps {
               bat 'npm test'
    }
}
    }
}
