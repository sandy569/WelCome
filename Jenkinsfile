pipeline{
	agent any
	environment {
		NEW_VERSION = '1.0.0'
	}
	
	stages {
		stage("build"){
		steps {
			echo 'building started'
			echo 'building version ${NEW_VERSION}'
		}
		}
		stage("test"){
		when{
			expression {
			BRANCH_NAME == 'dev' || BRANCH_NAME =='master'
			}
		}
		steps{
			echo 'testing is started : '
		}
		}
		stage("deploy"){
		steps{
			echo 'deployment staerted :'
		}
		}
	}
}