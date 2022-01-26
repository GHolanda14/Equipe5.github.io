pipeline {
  agent any
  stages {
    stage('Inicializar') {
      steps {
        echo 'Pipeline teste'
        mail(subject: '[Jenkins] Iniciando pipeline', body: 'Estamos iniciando a pipeline')
      }
    }

  }
}