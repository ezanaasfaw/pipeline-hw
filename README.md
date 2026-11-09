# Software Delivery Pipeline (GitHub -> CodeBuild -> Manual Review -> S3)

- `pipeline.yaml`: CloudFormation template that creates the pipeline, CodeBuild project, SNS topic, IAM roles and S3 buckets.
- `buildspec.yml`: build and test steps run by CodeBuild.
- `index.html`: sample application deployed after approval.

Pipeline stages: Source (GitHub) -> Build (CodeBuild) -> ManualReview (approval + SNS email) -> Deploy (S3).
