node  {
    def mvnhome = toolname: 'maven3' , type: 'maven'
    def "${mvnhome}/bin/mvn package"

stage ('checkout') {
git credentialsId: 'naresh', url: 'https://github.com/naresh4191/maven-web-application/'
  }

 stage ('build')    { 
     sh "clean package"
  }
    
    
}
    
    
