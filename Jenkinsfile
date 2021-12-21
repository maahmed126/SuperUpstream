pipeline {			
    agent any
  stages {  
stage ('Starting downstream job ') {
  steps {
    build job: 'MasterDev'  , propagate: false
    echo "Pipeline currentResult: ${currentBuild.currentResult}"  
      
    build job: 'MasterUpstream' , propagate: false
    echo "Pipeline currentResult: ${currentBuild.currentResult}"  
  }
}
}
}  
