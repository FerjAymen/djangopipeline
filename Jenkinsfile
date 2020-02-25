node {

        stage('checkout') {
            checkout scm
            sh "git rev-parse --short HEAD > .git/commit.id"
            commit_id = readFile('.git/commit.id').trim()
        }
/*
        stage('test') {
            sh '../pip install -r requirements.txt'
            sh '../python manage.py test'
        }
        def dockerImage
        stage('build docker') {
            dockerImage = docker.build("ferjaymen/djnagotestrepo:${commit_id}",'.')
		}
        
        stage('publish docker') {
            docker.withRegistry('https://hub.docker.com/repository/docker/ferjaymen/djnagotestrepo/', 'dockerhub') {
			dockerImage.push "${commit_id}"
			dockerImage.push "latest"
			}
        }
*/

}