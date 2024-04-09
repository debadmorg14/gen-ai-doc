---
slug: first-blog-post
title: First Blog Post
authors:
  name: Deba 
  title: Deploy Datahub in AWS
  url: https://github.com/mohade09
  image_url: https://github.com/mohade09.png
tags: [data, datahub]
---
## [Deploy Datahub in AWS](https://aws.amazon.com/blogs/big-data/part-1-deploy-datahub-using-aws-managed-services-and-ingest-metadata-from-aws-glue-and-amazon-redshift/)
Many organizations are establishing enterprise data warehouses, data lakes, or a modern data architecture on AWS to build data-driven products. As the organization grows, the number of publishers and subscribers to data and the volume of data keeps increasing. Additionally, different varieties of datasets are introduced (structured, semistructured, and unstructured). This can lead to metadata management issues, and the following questions:

“Can I trust this data?”
“Where does this data (lineage) come from?”
“How accurate is this data?”
“What does this column mean in my business terminology?”
“Who is the owner of this data?”
“When was the data last refreshed?”
“How can I classify the data (PII, non-PII, and so on) and build data governance?”
Metadata conveys both technical and business context to help you understand your data better and use it appropriately. It provides two primary types of information about data assets:

Technical metadata – Information about the structure of the data, such as schema and how the data is populated
Business metadata – Information in business terms, such as table and column description, owner, and data profile
Metadata management becomes a key element to allow users (data analysts, data scientists, data engineers, and data owners) to discover and locate the right data assets to address business requirements and perform data governance. Some common features of metadata management are:

Search and discovery – Data schemas, fields, tags, usage information
Access control – Access control, groups, users, policies
Data lineage – Pipeline runs, queries, transformation logic
Compliance – Taxonomy of data privacy, compliance annotation types
Classification – Classify different datasets and data elements
Data quality – Data quality rule definitions, run results, data profiles
These features can help organizations build standard metadata management processes, which can help remove redundancy and inconsistency in data assets, and allow users to collaborate and build richer data products quickly.

In this two-part series, we discuss how to deploy DataHub on AWS using managed services with the AWS Cloud Development Kit (AWS CDK), populate technical metadata from the AWS Glue Data Catalog and Amazon Redshift into DataHub, and augment data with a business glossary and visualize data lineage of AWS Glue jobs.

In this post, we focus on the first step: deploying DataHub on AWS using managed services with the AWS CDK. This will allow organizations to launch DataHub using AWS managed services and begin the journey of metadata management.


