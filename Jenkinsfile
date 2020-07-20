
node {
   // This is to demo github action	
   //def sonarUrl = 'sonar.host.url=http://172.31.30.136:9000'
   
   stage('SCM Checkout'){
    // Clone repo
	
	git 'https://github.com/enthusiast100/my-app'
   }
	
	stage('Compile-Package')
	
	{
	         def mvnHome = tool (name: 'maven', type: 'maven')
		sh "${mvnHome}/bin/mvn package"
	}
	
}
