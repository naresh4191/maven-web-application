node  {
    
stage ('checkout') {
          git crdentialsID: "naresh4191", url: 'https://github.com/naresh4191/maven-web-application'
                   }

 stage ('build')    { 

    tool name: 'maven3', type: 'maven'
     echo "building the project"
  }
    
    
}
    
    
