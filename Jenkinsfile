pipeline  {
  agent  any
  environment  {  APP_ENV = 'test'  }
  stages  {
    stage('Build')  {  steps  {  echo  'Building the project'  }  }
    stage('Test')   {  steps  {  echo  'Running  tests'  }  }
  }
  post  {
    success  {  echo  'pipeline succeeded'  }
    failure  {  echo  'Something failed'  }
  }
}
