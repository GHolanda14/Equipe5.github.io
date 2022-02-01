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
        sleep(time: 15, unit: 'SECONDS')
        build(job: 'Teste padrão', propagate: true)
        mail(to: 'gabrielbotelho@alu.ufc.br', subject: 'Teste', body: 'Você é o responsável pelos testes, confira tudo!')
      }
    }

  }
}