pipeline{
    agent any
    stages{
        stage ('Stage one git code '){
            steps{
               git branch : "main" ,
                url : "https://github.com/laxmipsavadati-code/PythonfromPepeline.git"
            }
        }
        stage ('Stage two check python'){
            steps{
                bat '"C:\\Users\\Administrator\\AppData\\Local\\Programs\\Python\\Python312\\python.exe" --version'
            }
        }
        stage ('Stage three installation'){
            steps{
                bat """ pip install -r requirements.txt """
            }
        }
        stage ('Stage four run project'){
            steps{
                bat """  python app.py  """
            }
        }
    }
}