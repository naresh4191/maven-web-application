node  {
    
stage ('checkout') {
git credentialsId: 'naresh', url: 'https://github.com/naresh4191/maven-web-application/'
  }

 stage ('build')    { 
def mvnhome = toolname:'Maven3',type:'maven'
     sh "${mvnhome}/bin/mvn package"
  }
    
    
}
    
    
