@Library('jenkins-shared-library') _

buildAndDeployApp([
    imageName: 'ivtheforth/jenkins-test',
    namespace: 'test',
    deployment: 'jenkins-test',
    container: 'jenkins-test',
    serviceUrl: 'https://test.leultewolde.com/notifications/actuator/health/liveness',
    vaultCred: 'vault-credentials',
    projectType: 'gradle',
    buildScript: './gradlew clean build',
    testScript: './gradlew test',
    skipSonar: true,
    projectId: '38fe5c74-237a-4af3-8d69-5df261b77a5d'
])