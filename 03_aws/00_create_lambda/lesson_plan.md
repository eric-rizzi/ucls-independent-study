## Essential Questions

## Actual Lesson

### Setup

- Create account for student
    - Log into AWS account `598791268315` as administrator
    - Go to IAM service
    - Create new user that is their UCLS Google email
    - Give access to Students Group:
        - Lambda - Full, S3 - Full, Cloudwatch - ReadOnly, SQS - Full
        - MFA setup
    - Send email asking them to log in

### Lesson Plan

Challenge Ladder

- Create your own `HelloWorld` Lambda via the console
    - Test via `lambda tests`
- Create your own `JsonReader` Lambda via the console
    - Should be able to read Json events
    - Test via `lambda tests`
- Create your own `S3Trigger` Lambda that's triggered by the addition of a file to s3
    - Does not actually read the file (aka not client)
    - Test via the creation of file in s3
- Read about the importance of a `Data Abstraction Layer` / `Data Access Object (DAO)`
    - Submit design doc for the two classes that should be created for reading s3 file
- Alter the `S3Trigger` Lambda that reads first and last words from s3 file
    - Test via the creation of file in s3
- Alter the `S3 Trigger` Lambda so that it writes first and last words from one s3 file to another s3 file
    - Submit design doc for the addition class that should be created for writing s3
    - Test via the creation of file in s3
- Do CI/CD deployment of code
    - Lots of help from teacher here
- Add custom library/code

### Resources

- AWS Lambda Introduction
    - https://youtu.be/iUIWG0h2D84?si=vBhUd8ZpzIHG0oAw
- AWS Lambda -> Lambda Invocation
    - https://youtu.be/Lf98s3NczBE?si=nWTaclVZirCyrhdC
- AWS S3 Events
    - https://youtu.be/H_rRlnSw_5s?si=JFMti45oWqijiKuY