pipeline {			
    agent any
  stages {  
stage ('Starting downstream job ') {
  steps {
    build job: 'MasterUpstream'
  }
}
}
}  
