def myfn(){
  println "i am printing data from myfn"
}
def myfn_with_parameters(a,b) {
  sum = a + b 
  println " sum of ${a} & ${b} is &{sum}"
}
pipeline {
  agent any
  stages{
    stage ('working with conditions') {
      steps {
        script {
           myfn()
           myfn_with_parameters(100,200)
           }
          }
        }
      }
    }
