```
{
  "Id": "Policy1690260299236",
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Stmt1690260012453",
      "Action": "s3:*",
      "Effect": "Deny",
      "Resource": "arn:aws:s3:::jam-challenge-patientdata-us-east-1-569419362345",
      "Principal": {
        "AWS": [
          "arn:aws:iam::569419362345:user/USER-A"
        ]
      }
    },
    {
      "Sid": "Stmt1690260048278",
      "Action": "s3:*",
      "Effect": "Allow",
      "Resource": "arn:aws:s3:::jam-challenge-patientdata-us-east-1-569419362345",
      "Principal": {
        "AWS": [
          "arn:aws:iam::569419362345:user/USER-B"
        ]
      }
    }
  ]
}
```