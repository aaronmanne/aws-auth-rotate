# aws-auth-rotate


TODO: A lot...

Simple script to rotate personal aws cli key
Requires MFA

Create the file $HOME/.aws/aws-accounts.json  with the following format
```
{
    "accounts": [
        {
            "iamuser": "myiamusername",
            "name": "ACCOUNTNAME",
            "totp": "TOPTOPTOPTOPTOPTOPTOPTOPTOPTOPTOP",
            "aws_access_key_id": "ABCDEFGHIJKLMNOPQRSTUVWXYZ",
            "aws_secret_access_key": "SUPERSECRETKEYAWSGAVEME",
            "aws_mfa_device": "arn:aws:iam::123456789102:mfa/myiamusername",
            "aws_mfa_duration": 129600
        }
    ]
}
```
