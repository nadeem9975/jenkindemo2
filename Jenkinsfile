pipeline {
    agent any
    parameters{
    
        string( name: 'DevOps', defaultValue: 'abcd', description:'asdfghjk' )
        choice (name: 'Courses' , choices:['DevOps', 'Java', 'Pyhton Developer', 'Ruby'], description: 'Choose from the list ')
        booleanParam(name: 'isvalid', defaultValue: true , description: 'have you done with testing ')
    }
    
    
    stages {
        stage('unitTest ') {
            steps {
                echo 'Hello Unit test is ok '
                sh '''pwd
                      date
                      cal 2021
                      '''
                
            }
	}
        stage('Build ') {
            steps {
                echo 'Hello Build is ok'
                sh 'date'
                sh 'echo "${BUILD_ID}"'
               
        
            }
	}
        stage('Deploy ') {
            environment{ 
        name = 'abcde'
    }
            steps {
                echo 'Hello Deploy to test is ok '
                sh 'echo "${name}"'
            }
	}
        stage('DeploytoProd ') {
            steps {
                echo 'Hello DeploytoProd is ok '
                
            }
        }
    }
}
