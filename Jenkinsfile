pipeline  {
  agent  any
  parameters  {  choice(name:  'ENVIRONMENT',
                        choices:  ['dev',  'staging',  'production'])  }
  stages  {
    stage('Approve')  {
      when  {  expression  {  params.ENVIRONMENT == 'prodection'  }  }
      steps  {  input message:  'Deploy to producion  }
    }
    stage('Deploy')  {
      steps  {  bat "echo Deploy to ${params.ENVIRONMENT}"  }
    }
  }
}
}
