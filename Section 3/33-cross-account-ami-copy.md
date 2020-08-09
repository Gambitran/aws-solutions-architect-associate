## Cross Account AMI Copy

* Can share AMI with another AWS account
* Sharing does not affect ownership
* If copy AMI that has been shared with your account, you are owner of target AMI
* To Copy AMI that was shared, owner of source must grant you read permissions for storage that backs AMI 
  * Either associated EBS snapshot (EBS-backed AMI) or associated S3 bucket (instance store-backed AMI)
* Limits
  * Can't copy encrypted AMI that was shared. If underlying snapshot and encryption were shared, can copy snapshot while re-encrypting it with key of your own. You own the copied snapshot, and can register as new AMI
  * Can't copy AMI with associated billingProduct code. This includes Windows AMIs and AMIs from AWS Marketplace. Create EC2 instance using shared AMI and then create an AMI from the instance