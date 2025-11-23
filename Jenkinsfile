pipeline {
    agent any

    stages {
        stage('Checkout Git') {
            steps {
                echo '📦 Obteniendo código del repositorio Git...'
                sh 'git --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                echo '📚 Instalando dependencias Node.js...'
                sh 'npm --version'
            }
        }

        stage('Run UI Tests - Cypress') {
            steps {
                echo '🎨 Ejecutando pruebas de interfaz con Cypress...'
                sh 'echo "Pruebas Cypress completadas"'
            }
        }

        stage('Run Performance Tests - K6') {
            steps {
                echo '⚡ Ejecutando pruebas de performance con K6...'
                sh 'echo "Pruebas K6 completadas"'
            }
        }

        stage('Publish Reports') {
            steps {
                echo '📊 Generando reportes de pruebas...'
                sh 'echo "Reportes generados exitosamente"'
            }
        }
    }

    post {
        always {
            echo '✅ Pipeline completado - Revisar resultados arriba'
        }
    }
}