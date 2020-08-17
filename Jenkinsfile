node  {
  def mvnhome = tool name:'maven3', type:'maven'
    def "${mvnhome}/bin/mvn"   

stage ('checkout') {
git credentialsId: 'naresh', url: 'https://github.com/naresh4191/maven-web-application/'
  }
 stage ('build')    { 
     sh "clean package"
  }
   
    
}
    
    
