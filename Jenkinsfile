pipeline {
  agent any
  stages {
    stage('Inicializar') {
      steps {
        echo 'Pipeline teste'
        mail(subject: '[Jenkins] Iniciando pipeline', body: 'Estamos iniciando a pipeline', to: 'gabriel.raulino@alu.ufc.br')
      }
    }

    stage('Teste') {
      steps {
        echo 'Iniciando teste...'
        sleep(time: 15, unit: 'MINUTES')
        build(job: 'unicorn-test', propagate: true)
      }
    }

  }
}