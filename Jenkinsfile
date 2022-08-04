node{
 tools {
   maven 'maven383'
 }
 stage("Checkout"){
    git ''
 }
 stage("Build"){
    sh 'mvn clean compile'
 }
 stage("Test"){
     sh 'mvn test'
     junit '**/target/surefire-reports/TEST-*.xml'
 }
 stage("Package"){
     sh 'mvn package'
 }
 
}
