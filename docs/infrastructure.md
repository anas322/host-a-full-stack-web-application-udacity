## Udagram Infrastructure

![Architecture](architecture.png)

### AWS RDS Postgres
The application uses RDS Postgres for storing and retrieving information.

Database URI: `postgres://postgres:test12345@database-1.colopl8ifvu6.us-east-1.rds.amazonaws.com:5432/store`

#### Elastic Beanstalk
The application is build, archived and uploaded to S3 bucket from where Elastic Beanstalk extracts and runs the application on an endpoint.

EB URL: `http://udagram-api-dev.eba-xz2amksu.us-east-1.elasticbeanstalk.com/`

#### S3 Bucket
The bundled assets are uploaded to an S3 bucket and that bucket is made publicly readable.

Bucket URL: `http://mybucket-udacity.s3-website-us-east-1.amazonaws.com/`
