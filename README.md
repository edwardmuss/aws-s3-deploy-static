# aws-s3-deploy-static

This project explains how to deploy a static website on AWS

### Our Deployed static website can be accessed via the following links

[Link 1: Cloud Front](https://d2c13m1jfy0sgt.cloudfront.net)<br>
[Link 2: Default](http://udacity-edwards.s3-website-us-east-1.amazonaws.com)

Use this code the configure bucket policy. Remember to repalace `your-website` with your **bucket name**

```
{
"Version":"2012-10-17",
"Statement":[
 {
   "Sid":"AddPerm",
   "Effect":"Allow",
   "Principal": "*",
   "Action":["s3:GetObject"],
   "Resource":["arn:aws:s3:::your-website/*"]
 }
]
}
```

# Website example

![website Image](web-sample.png)
