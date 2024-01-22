pipeline {
    agent any

tools{

    maven "maven"

}
    environment{
         
           VERSION_NAME="1.34"
}
    stages 
   {
        
        stage('Build') {
            steps {
                echo 'Build Application'
                echo '${VERSION_NAME}'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Test Application'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploy Application'
            }
        }
    }
    
    post
{

      always
{
       emailext body: 'Summary ', subject: 'Pipeline Status ', to: 'qaautomationvipul@gmail.com'
      }
   }
}
