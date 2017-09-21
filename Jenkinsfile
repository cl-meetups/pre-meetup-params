pipeline {
  agent any
  parameters {
    choice(name: 'pizza',
      choices: 'Calabresa\n4 Queijos\nTomate\nPresunto',
      description: 'Selecione sua Pizza')
    booleanParam(name: 'COM_BORDA',
      defaultValue: true,
      description: 'Borda Recheada')
    string(name: 'adicionais',
      defaultValue: 'Pimenta',
      description: 'Adicionais para a Pizza')
  }

  stages {
    stage('Exemplo') {
      steps {
        echo 'Params:'
        echo "Pizza: ${params.pizza}"
        echo "Com borda receheada: ${params.COM_BORDA}"
        echo "Adicionais: ${params.adicionais}"
      }
    }
  }
}
