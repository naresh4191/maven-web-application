node  {
  def mvnhome = tool name:'maven3', type:'maven'
       

stage ('checkout') {
git credentialsId: 'naresh', url: 'https://github.com/naresh4191/maven-web-application/'
  }
 stage ('build')    { 
   sh "${mvnhome}/bin/mvn package"
   
  
  }
  stage ('deploy to tomcat') {
    sshagent(['tomcat-new']) {
    sh"""
    
    scp -o StrictHostKeyChecking=no target/*.war root@172.31.34.1:/apache-tomcat-8.5.57/webapps/
    
    shh root@172.31.34.1 /apache-tomcat-8.5.57/bin/shutdown.sh
    
    shh root@172.31.34.1 /apache-tomcat-8.5.57/bin/startup.sh
    
       """
    }
  }
    
}
    
    
