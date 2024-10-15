## Essential Questions

## Lesson Plan

### Setup


TODO: Switch from `sample_app_src_rep` to `aws_src_repo-`

1. Setup Src Pipeline
    1. Make a copy of `Documents/workspace/Projects/AWSInfraTXU` repo
        - `cp -r AWSInfraTXU AWSSrcStudentName`
    2. Checkout `80ea255`
    3. Create a fresh repo at that commit
        - `rm -rf .git`
        - `git init`
        - `git add .`
        - `git commit -m "Initial Commit"`
    4. Create a **new** GitLab project that student will take over
        - e.g., "AWSSrcStudentName"
    5. Alter `gitlab-ci.yml` file so pushes to ECR repo created by Infra
        - ACCOUNT, TRIGGER_URL variables
            - Get `TIGGER_URL` from CURL example in `Settings` -> `CI/CD` -> `Pipeline Trigger Tokens`
            - Create new token named `SourceCodePublishEvent`
    6. Set up CI/CD
        1. Set path to CI/CD file
        2. Set variables
            - AWS_ACCESS_KEY_ID
            - AWS_DEFAULT_REGION
                - Set to region **SPECIFIC** to student to avoid collisions
            - AWS_SECRET_ACCESS_KEY
            - INFRA_TRIGGER_TOKEN

### Actual Lesson

- Rough: https://docs.google.com/document/d/15mgQNYt54nPrwl8miEN0n_T1ZJqVGHRXdm3BB0animg
