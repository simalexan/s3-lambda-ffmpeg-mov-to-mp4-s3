
# S3 Bucket -> Lambda (FFMPEG Convert MOV to MP4) -> S3 Bucket

## Description

This is a serverless component that takes uploaded MOV video files from one S3 Bucket, then using FFMPEG Lambda Layer converts them to MP4 and uploads to another S3 Bucket. It contains:

- an Input S3 Bucket that accepts MOV video files.

- a Lambda that takes the MOV video file from the Input S3 bucket, converts it to a MP4 one and uploads it to the Output bucket

- an Output S3 Bucket that receives MP4 files.

## Deployment Parameters

This component has one CloudFormation deployment parameter:

- `ConversionTimeout`, an optional parameter, represents the timeout of the Conversion Lambda function. By default it's 180 seconds.

## Latest Release - 1.0.0

- Initial release.

## Roadmap - Upcoming changes

Here are the upcoming changes that I'll add to this serverless component:

- ESLint
- Tests