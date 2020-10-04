pipeline {
    agent any
    parameters 
    {
        string(name:'Greeting', defaultValue: 'Hello', description: 'how to greet')
    }
    stages
        {
            stage("Hello")
            {
            steps {
                timeout(time:1,unit:'MINUTES')
                {
                echo "${params.Greeting} World!"           }
                
            }
}
stage("Build")
{
 steps{
     sh 'echo "Build Step starts"'
     sh 'echo "Hello From Jenkins"'
 }   
}

}
}
