# authconnector-aws-roleanywhere

Automates authentication with AWS services using `aws-signing-helper` to obtain a Role Anywhere token, storing the valid token in the `.credentials` file.

## Prerequisites

- An active AWS account
- Role Anywhere configured with:
  - Trust anchor
  - IAM role with necessary permissions
  - X.509 certificate
- `aws-signing-helper` installed

## Installation

### Install AWS Signing Helper

Follow the official AWS documentation for installation instructions:

[AWS Signing Helper Guide](https://docs.aws.amazon.com/rolesanywhere/latest/userguide/credential-helper.html)

## Usage

1. Ensure your certificate and private key are accessible on the local machine.
2. Run the authentication command to obtain temporary credentials:

   ```bash
   ./authconnector-aws-roleanywhere --profile your-profile-name
