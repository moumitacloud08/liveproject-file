pipeline {
    agent any
    tools { 
        maven 'jenkins-maven' 
    }
    stages {
        stage('Checkout spring-petclinic-rest-visit') {
            steps {
                bat 'echo spring-petclinic-rest-visit image build'
                bat 'git config --global http.sslVerify false'
                git branch: "dev", url: 'https://github.com/moumitacloud08/spring-petclinic-rest-visit.git'
                // Do a ls -lart to view all the files are cloned. It will be clonned. This is just for you to be sure about it.
                //bat "dir" 
                // List all branches in your repo. 
                bat "git branch -a"
                bat "mvn package"
                bat "dir target" 
                bat "copy target\\spring-petclinic-rest-visit-1.7.jar src\\main\\docker"
                bat "dir src\\main\\docker"
                //bat "docker build -t spring-petclinic-rest-visit src/main/docker"
                bat "docker-compose -f src/main/docker/spring-petclinic-rest-visit.yml up --build -d"
                
             }
        }
        stage('Checkout spring-petclinic-rest-vet') {
            steps {
                bat 'echo spring-petclinic-rest-vet image build'
                bat 'git config --global http.sslVerify false'
                git branch: "dev", url: 'https://github.com/moumitacloud08/spring-petclinic-rest-vet.git'
                // Do a ls -lart to view all the files are cloned. It will be clonned. This is just for you to be sure about it.
                //bat "dir" 
                // List all branches in your repo. 
                bat "git branch -a"
                bat "mvn package"
                bat "dir target" 
                bat "copy target\\spring-petclinic-rest-vet-1.7.jar src\\main\\docker"
                bat "dir src\\main\\docker"
                //bat "docker build -t spring-petclinic-rest-visit src/main/docker"
                bat "docker-compose -f src/main/docker/spring-petclinic-rest-vet.yml up --build -d"
                
             }
        }
        stage('Checkout spring-petclinic-rest-system') {
            steps {
                bat 'echo spring-petclinic-rest-system image build'
                bat 'git config --global http.sslVerify false'
                git branch: "dev", url: 'https://github.com/moumitacloud08/spring-petclinic-rest-system.git'
                // Do a ls -lart to view all the files are cloned. It will be clonned. This is just for you to be sure about it.
                //bat "dir" 
                // List all branches in your repo. 
                bat "git branch -a"
                bat "mvn package"
                bat "dir target" 
                bat "copy target\\spring-petclinic-rest-system-1.7.jar src\\main\\docker"
                bat "dir src\\main\\docker"
                //bat "docker build -t spring-petclinic-rest-visit src/main/docker"
                bat "docker-compose -f src/main/docker/spring-petclinic-rest-system.yml up --build -d"
                
             }
        }
        stage('Checkout spring-petclinic-rest-pet') {
            steps {
                bat 'echo spring-petclinic-rest-pet image build'
                bat 'git config --global http.sslVerify false'
                git branch: "dev", url: 'https://github.com/moumitacloud08/spring-petclinic-rest-pet.git'
                // Do a ls -lart to view all the files are cloned. It will be clonned. This is just for you to be sure about it.
                //bat "dir" 
                // List all branches in your repo. 
                bat "git branch -a"
                bat "mvn package"
                bat "dir target" 
                bat "copy target\\spring-petclinic-rest-pet-1.7.jar src\\main\\docker"
                bat "dir src\\main\\docker"
                //bat "docker build -t spring-petclinic-rest-visit src/main/docker"
                bat "docker-compose -f src/main/docker/spring-petclinic-rest-pet.yml up --build -d"
                
             }
        }
        stage('Checkout spring-petclinic-rest-owner') {
            steps {
                bat 'echo spring-petclinic-rest-owner image build'
                bat 'git config --global http.sslVerify false'
                git branch: "dev", url: 'https://github.com/moumitacloud08/spring-petclinic-rest-owner.git'
                // Do a ls -lart to view all the files are cloned. It will be clonned. This is just for you to be sure about it.
                //bat "dir" 
                // List all branches in your repo. 
                bat "git branch -a"
                bat "mvn package"
                bat "dir target" 
                bat "copy target\\spring-petclinic-rest-owner-1.7.jar src\\main\\docker"
                bat "dir src\\main\\docker"
                //bat "docker build -t spring-petclinic-rest-visit src/main/docker"
                bat "docker-compose -f src/main/docker/spring-petclinic-rest-owner.yml up --build -d"
                
             }
        }
    }
}
