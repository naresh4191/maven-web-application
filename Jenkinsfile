node  {

    def mvnhome = tool name: 'Maven3.6.0' , type: 'maven'
    
stage ('checkout') {
          git 'https://github.com/naresh4191/maven-web-application'
                   }

 stage ('buidl')    { 

           sh 'mvn package'
  }
    
    
}
    
    
