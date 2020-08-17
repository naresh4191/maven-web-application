node  {
  def mvnhome = tool name:'maven3', type:'maven'
       

stage ('checkout') {
git credentialsId: 'naresh', url: 'https://github.com/naresh4191/maven-web-application/'
  }
 stage ('build')    { 
   sh "${mvnhome}/bin/mvn package" 
  
  }
   
    
}
    
    
