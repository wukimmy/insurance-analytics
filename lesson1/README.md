# Lesson 1

On this lesson we will be creating the S3 buckets for the process. 

## 1. Creat the Data Source bucket

As an data source, we will have two different files, therefore we will separate in two differents S3 buckets:
- insurance-data-bucket
- property-data-bucket

And you will also nedd the bucket for the result, with a folder for the tranformed file:
```
result-bucket
    |
    └───transformed-file-folder

```
You can follow the instructuions on the [AWS documentation](https://docs.aws.amazon.com/AmazonS3/latest/gsg/CreatingABucket.html) to create your bucket.

 [Optional] If you would like to, you set up [lifycycles](https://docs.aws.amazon.com/AmazonS3/latest/user-guide/create-lifecycle.html) to change the un used files category, or enable [versioning](https://docs.aws.amazon.com/AmazonS3/latest/dev/ObjectVersioning.html) so your crawler will only use the latets file.

## 2. Add files
After you create the S3 buckets, you may add the [sample csv files](https://github.com/wukimmy/insurance-analytics/tree/master/sample-csv) on the datasource bucket. 
```
insurance-data-bucket
    |FL_insurance_sample.csv

property-data-bucket
    |FL_insurance_sample_property.csv

```
 - - - -
You may follow to [lesson 2](https://github.com/wukimmy/insurance-analytics/tree/master/lesson2)