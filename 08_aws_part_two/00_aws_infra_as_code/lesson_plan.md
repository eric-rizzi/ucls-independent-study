## Essential Questions

## Lesson Plan

### Setup

1. Setup Infra Pipeline for student in their own region
    1. Make a copy of `Documents/workspace/Projects/AWSInfraSample` repo
        - `cp -r AWSInfraSample AWSInfraStudentName`
    2. Checkout `829a747`
    3. Create a fresh repo at that commit
        - `rm -rf .git`
        - `git init`
        - `git add .`
        - `git commit -m "Initial Commit"`
    4. Clear out old libraries and build
        - `rm -rf node_modules`
        - `npm install`
        - `npm run build`
    5. Bootstrap to new region
        - `cdk bootstrap aws://598791268315/ca-central-1`
    6. Create a **new** GitLab project that student will take over
        - e.g., "AWSInfraStudentName"
        - Link project with local repo just created
        - Push project
    7. Set up CI/CD
        1. Set path to CI/CD file
        2. Set variables
            - AWS_ACCESS_KEY_ID
            - AWS_DEFAULT_REGION
                - Set to region **SPECIFIC** to student to avoid collisions
            - AWS_SECRET_ACCESS_KEY

### Actual Lesson

- Rough: https://docs.google.com/document/d/1ZLFzG_-HqCs_UDjQs9KIOmp8zFPp5bSBtSDVgH_3e34

- Ideas:
    - API Gateway that links back to GitHubPages
        - Provides own (random) inspirational quote
        - Doesn't let person be picked twice in a row
        - ???