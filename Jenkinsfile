pipeline {			
    agent any
  stages {  
stage ('Starting downstream job ') {
  steps {
    build job: 'MasterDev' , propagate: false
    echo "Pipeline currentResult: ${currentBuild.currentResult}"  
      
    build job: 'DevUP' , propagate: false
    echo "Pipeline currentResult: ${currentBuild.currentResult}"  
  }
}
}
}  
