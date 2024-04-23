pipeline {
    agent any

    parameters {
        string(name: 'process_name', defaultValue: '', description: 'Ingrese el nombre del proceso a buscar')
    }

    stages {
        stage('Ejecutar script') {
            steps {
                // Clonar el repositorio donde se encuentra el script
                git 'https://ruta.a.tu/repositorio.git'

                // Ejecutar el script main.sh con el nombre del proceso como parámetro
                sh "./main.sh ${params.process_name}"
            }
        }
    }
}
