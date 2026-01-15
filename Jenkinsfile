@Library('sonarqube-shared-lib') _

def config = readYaml text: libraryResource('sonarqube-config.yml')

sonarqubePipeline(
    REPO_URL: 'https://github.com/purusharma635/sonarqube-ansible-project.git',
    SLACK_CHANNEL_NAME: config.SLACK_CHANNEL_NAME,
    ENVIRONMENT: config.ENVIRONMENT,
    CODE_BASE_PATH: config.CODE_BASE_PATH,
    ACTION_MESSAGE: config.ACTION_MESSAGE,
    KEEP_APPROVAL_STAGE: config.KEEP_APPROVAL_STAGE
)

