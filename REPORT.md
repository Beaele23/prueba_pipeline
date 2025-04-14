# Reporte de Implementación
## Pasos realizados
1. Configuración inicial del repositorio.
2. Creación y configuración del Jenkinsfile.
3. Configuración del pipeline en Jenkins.
4. Resolución de errores en URL y credenciales.
## Problemas encontrados
- Problemas al clonar el repositorio debido a errores en la URL.
- Ajuste de credenciales y configuración de Git en Jenkins.
- Cambié los comandos en el Jenkinsfile de sh a bat para adaptar el pipeline a un entorno Windows.

pipeline {
    agent any
    stages {
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
    }
}

## Resultados
- Pipeline exitoso, todas las etapas completadas.
