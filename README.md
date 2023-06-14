
# VPC FLOW LOGS - USING S3 BUCKET AND ATHENA





## Creating VPC FlowLOgs

1. Go to VPC Dashboard
2. Click on Flowllogs
3. Click Create Flowlog
4. Give : Name - xyz
5. Select Destination : Send to an Amazon S3 bucket
6. Create an S3 buckt 
6. Give arn of your S3 bucket 
7. Click Create 

## S3 bucket

1. Go to your S3 bucket that stores VPC logs 
2. Copy the path of S3 logs
3. Create an output folder for storing s3 output 

## ATHENA Setup

1. Go to Athena Dashboard
2. In settings set up output folder 
3. Click on add query button situated on right hand side 
4. Paste the following code 

![Screenshot from 2023-06-08 11-55-07](https://github.com/mayankmajreti1/Cloud-Custodian/assets/126334005/f591a344-6335-49ce-b64f-d0306e8c828f)

5. Replace path of S3 bucket , and paste url of S3 bucket which stores log path .
6. Add another Query & Run the following script , baut first replace the path and set date according to you .

![Screenshot from 2023-06-08 12-00-18](https://github.com/mayankmajreti1/Cloud-Custodian/assets/126334005/7a0f9290-f575-4382-9412-059d2dc0ca29)

7. Open another Query and RUN the following script

![Screenshot from 2023-06-08 12-03-32](https://github.com/mayankmajreti1/Cloud-Custodian/assets/126334005/fdf8575e-b7c3-43a0-8155-fcfa557432cd)

#### In the Result section you can check your logs now .
