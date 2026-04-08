# AWS-S3-IAM-project
The public access problem.
AWS S3: The public access issue; Today I solved a real word problem.
-- I started by creating an Amazon S3 bucket. 
-- uploaded files to said bucket and then earned how to enable static website hosting within the bucket
-- those files gave an access denied error when trying to open them
-- I confirmed public access was not blocked
-- then i created a bucket policy allowing access
-- I then created an IAM policy through JSON allowing developers to upload to the bucket
-- the policy did not allow for delete or change permissions
-- I created an IAM user to simulate a test for the new policy
-- the dev uploaded a new product image and again we got an access denied log
-- the dev used a private object ACL
-- I then when into the ACL and granted "everyone" read access which resolved the access denied issue

**I learned how to: ✅ Identify permission misconfigurations ✅ Write least-privilege S3 bucket policies ✅ Confirm security + availability balance
