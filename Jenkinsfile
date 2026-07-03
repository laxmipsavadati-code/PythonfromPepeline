pipeline {
    agent any

    environment {
        PYTHON = 'C:/Users/Laxmi/AppData/Local/Programs/Python/Python313/python.exe'
    }

    stages {

        stage('Check Python') {
            steps {
                bat '"%PYTHON%" --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat '"%PYTHON%" -m pip install --upgrade pip'
                bat '"%PYTHON%" -m pip install -r requirements.txt'
            }
        }

        stage('Run Flask') {
            steps {
                bat '"%PYTHON%" app.py'
            }
        }
    }
}