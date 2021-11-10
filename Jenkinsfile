pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs'nodejs' 
    }
 

    stages{
        stage('Build'){
            steps{
                echo 'this is the Build job'
                sh 'npminstall' 
            }
        }
        stage('Test'){
            steps{
                echo 'this is the Test job'
                sh 'npmtest' 
            }
        }
        stage('Package'){
            steps{
                echo 'this is the Package job'
                sh 'uptime'
                sleep 7
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
