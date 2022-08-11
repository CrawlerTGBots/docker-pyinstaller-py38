@Library('michi-global-library') _

codenturyPipeline() {
    build {
        stage("Container") {
            dockerBuildAndPush("tools/python-win64", "3.8", [
                    dockerfile: "Dockerfile-py3-win64",
                    username: "crawlertgbots"
            ])
        }
    }
}
