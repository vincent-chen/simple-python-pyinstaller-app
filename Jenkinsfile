pipeline {
    agent { label: "node1" }
    stages {
        stage('Build') { 
            steps {
                sh 'python -m py_compile sources/add2vals.py' 
                stash(name: 'compiled-results', includes: 'sources/*.py*') 
            }
        }
    }
}
