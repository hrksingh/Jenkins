pipeline{
    agent{
        label "Docker"
    }
    stages{
        stage("Build"){
            steps{
                echo "========executing Build========"
            }
            post{
                always{
                    echo "========always block executed========"
                }
                success{
                    echo "========Build executed successfully========"
                }
                failure{
                    echo "========Build execution failed========"
                }
            }
        }
        stage("Test"){
            steps{
                echo "doing test"
            }
        }

    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}