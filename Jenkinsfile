pipeline{
    agent any
    stages{
        stage ' Stage one git code '{
            steps{
               git brach : "main" ,
                url : "https://github.com/laxmipsavadati-code/PythonfromPepeline.git"
            }
        }
        stage 'stage two check python'{
            steps{
                bat """ python --version """
            }
        }
        stage 'stage three installation'{
            steps{
                bat """ pip install -r requirements.txt """
            }
        }
        stage 'stage four run'{
            steps{
                bat """ python app.py """
            }
        }
    }
}