__Versioning__

* Stores all versions of an object (including all writes and even if you deleten an object). Can boost the cost.
* Great backup tool.
* Integrates with lifecycle rules.
* After enabled, you cannot disable it, but you can suspend.
* All versions can be managed by clicking the object in the S3 management UI console.
* Versioning's MFA Delete capability, which uses multi factor auth, can be used to provide an additional layer of security.

__Cross Region Replication__

* e.g. replicate data in a bucket located in London => Sydney.
* Both buckets must have versioning enabled.
* All contents or some content can be replicated.
* Only new data will be replicated, not existing ones.
* Delete markers are replicated.
* Deleting individual versions or delete markers will not be replicated.
* You cannot replicate to multiple buckets or use daisy chaining at this time.

__Lifecycle Management__

* Current version can move to S3 - IA after configured time.
* Current version can move to Glacier after configured time.
* Previous version can move to S3 - IA after configured time.
* Previous version can move to Glacier after configured time.
* Current and previous versions:
    * Can expire after configured time. (Expire: putting a delete marker)
    * Can be permanently deleted after configured time.
* Incomplete multipart uploads can be cleaned after configured time.
* Transition to S3 - IA (must be > 128Kb and min 30 days after creation date)
* Archive to the Glacier (min 30 days after IA, if relevant.)