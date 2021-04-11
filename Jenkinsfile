pipeline{
    agent any
    stages{
        stage('build'){
            steps{
                sh 'echo "hello word"'
                sh '''
                    echo "before the execute"
                    ls -la
                '''
            }
        }
        stage('run'){
            steps{
                sh '''
                    echo "runing comming"
                    python hello.py
                '''
            }
        }
    }
}