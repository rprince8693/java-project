
node {
   stage('Unit Test') {
    ant -f test.xml -v 
    junit 'reports/result.xml'
     }
   stage('Builds') {
      ant -f build.xml -v
      archive 'target/*.jar'
   }
  stage('Deploy') {
      ant -f build.xml -v
      archive 'rectangle/*.jar'
  
  
}


