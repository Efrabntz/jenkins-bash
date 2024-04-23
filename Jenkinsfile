pipeline {
    agent any

    parameters {
        string(name: 'process_name', defaultValue: '', description: 'Ingrese el nombre del proceso a buscar')
    }

    stages {
        stage('Preparar') {
            steps {
                // Dar permisos de ejecución al archivo main.sh
                sh 'chmod +x main.sh'
            }
        }
        
        stage('Ejecutar script') {
            steps {
                // Ejecutar el script main.sh con el nombre del proceso como parámetro
                sh "./main.sh ${params.process_name}"
            }
        }
    }
}
