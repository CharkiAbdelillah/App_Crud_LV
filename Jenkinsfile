pipeline{
    agent any
    stages{
        stage('build'){
            steps{
                sh 'echo "hello word"'
                sh '''
                    echo "before the execute"
                    ls -la
                    whoami
                    hostname
                    cd /var/www
                    ls
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