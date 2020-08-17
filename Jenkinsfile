node  {
  def mvnhome = tool name:'maven3', type:'maven'
       

stage ('checkout') {
git credentialsId: 'naresh', url: 'https://github.com/naresh4191/maven-web-application/'
  }
 stage ('build')    { 
   sh "${mvnhome}/bin/mvn deploy"
   
  
  }
  stage ('deploy to tomcat') {
    sh " scp -o StrictHostKeyChecking=no /target/*.war root@172.31.34.1:/opt/apache-tomcat-8.5.57/webapps"
    }
    
}
    
    
