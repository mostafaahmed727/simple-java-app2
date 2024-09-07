node{
    git branch: 'main', url: 'https://github.com/mostafaahmed727/simple-java-app2.git'
    stage('build'){
        try{
        sh'echo "build stage"'
        }
        catch(Exception e){
            sh'echo "error occured'
            throw e 
        }
    }
    stage('test'){
        if(env.BRANCH_NAME == "feat" ){
            sh'echo "test stage"'
        }
        else{
            sh'echo "skip test stage"'
        }
    }
}
