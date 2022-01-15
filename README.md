# AWS_BlazingTextClassifier
Building SageMaker BlazingText built-in algorithm to predict if the sms is spam ot not. BlazingText is a variant of FastText which is based on word2vec.
The Dataset which is used for the model is in public S3 bucket: https://s3.console.aws.amazon.com/s3/buckets/daria-hlibova-test?region=us-east-2&tab=objects.
If there will be some issues to open this bucket, train and validation dataset are  in repository (train.csv and val.csv)

The repository includes all steps:
1. Downloading dataset from the S3 bucket
2. Transforming and preparing dataset, bacause BlazingText algorithm requires the special format of data.
3. Splitting data to train and validation datasets.
4. Uploading train and validation datasets to S3 bucket.
5. Model building
6. Creating endpoint and deploying model.
7. Doing prediction and testing model. 
