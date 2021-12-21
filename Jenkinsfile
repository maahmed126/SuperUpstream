pipeline {			
    agent any
  stages {  
stage ('Starting downstream job') {
  steps {
    echo 'TRIGGERED ALL DEVELOP AND MASTER PIPELINE'
    build job: 'MasterDev'  , propagate: false
    echo "Pipeline currentResult: ${currentBuild.currentResult}"  
      
    build job: 'MasterUpstream' , propagate: false
    echo "Pipeline currentResult: ${currentBuild.currentResult}"  
  }
}
}
}  
