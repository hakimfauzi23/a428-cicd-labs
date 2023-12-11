node {
    def nodeImage = 'node:16-buster-slim'

    // Run Node.js application inside Docker container
    stage('Build') {
        docker.image(nodeImage).inside('-p 3000:3000') {
            sh 'npm install'
        }
    }
}
