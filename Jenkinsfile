pipeline{
    agent{
        docker{
            image 'maven:3.8.6-openjdk-18'
            args '-v /Users/xsw/.m2:/root/.m2'
        }
    }
    stages{
        stage('Build'){
            steps{
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}