## Improving Operational Efficiencies of Apache Iceberg tables build on Amazon S3 Data Lakes

Amazon S3 uses object tagging to categorize storage where each tag is a key-value pair. From Apache Iceberg perspective, it supports custom S3 Object tags that can be added to S3 objects while writing and deleting into the table. Iceberg Users can also configure tag-based object lifecycle policy at bucket level to transition objects to different S3 tiers. With the s3.delete.tags config property in Iceberg, objects are tagged with the configured key-value pairs before deletion. When the catalog property s3.delete-enabled is set to false, the objects are not hard-deleted from S3. This is expected to be used in combination with S3 delete tagging, so objects are tagged and removed using S3 lifecycle policy. This property is set to true by default. The example notebook in this blog shows example implementation of S3 Object tagging and Lifecycle rules for Apache Iceberg Tables to optimize the storage cost.

Open the **Sample_Notebook.ipynb** file for a step by step instruction on how to implement the storage optimization solution on Apache Iceberg Tables unning on Amazon S3 Data Lake.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved. \
This library is licensed under the MIT-0 License. See the LICENSE file. \
SPDX-License-Identifier: MIT-0


