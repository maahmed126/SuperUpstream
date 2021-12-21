pipeline {			
    agent any
  stages {  
stage ('Starting downstream job ') {
  steps {
    build job: 'MasterDev'  
    echo "Pipeline currentResult: ${currentBuild.currentResult}"  
      
    build job: ' MasterUpstream' 
    echo "Pipeline currentResult: ${currentBuild.currentResult}"  
  }
}
}
}  
