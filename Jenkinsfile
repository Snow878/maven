node('master') {
stage('ContinuousDowload_Master') {
   git 'https://github.com/intelliqittrainings/maven.git'
}
stage('ContinuousBuild_Master') {
   sh 'mvn package'
}
stage('ContinuousDeployment_Master') {  sh 'scp          /home/ubuntu/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war ubuntu@172.31.6.168:/var/lib/tomcat8/webapps/testapp.war'
}
 }                      
