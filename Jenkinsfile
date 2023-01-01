pipeline {
    agent any
    environment {
        AWS_ACCOUNT_ID="500278297469"
        AWS_DEFAULT_REGION="ap-south-1" 
	CLUSTER_NAME="default"
	SERVICE_NAME="devops-container-service"
	TASK_DEFINITION_NAME=" first-run-task-definition:1 "
	DESIRED_COUNT="1"
        IMAGE_REPO_NAME="devops-demo"
        IMAGE_TAG="${env.BUILD_ID}"
        REPOSITORY_URI = "${AWS_ACCOUNT_ID}.dkr.ecr.${AWS_DEFAULT_REGION}.amazonaws.com/${IMAGE_REPO_NAME}"
	registryCredential = "demo-admin-user"
    }
}
