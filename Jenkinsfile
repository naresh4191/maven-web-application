node  {

    def mvnhome = tool name: 'maven3', type: 'maven'
    
stage ('checkout') {
          git 'https://github.com/naresh4191/maven-web-application'
                   }

 stage ('build')    { 

           sh 'mvn package"
  }
    
    
}
    
    
