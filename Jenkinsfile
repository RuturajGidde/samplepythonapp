pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git url: 'https://github.com/RuturajGidde/samplepythonapp.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'pytest test_app.py'
            }
        }
    }
}
