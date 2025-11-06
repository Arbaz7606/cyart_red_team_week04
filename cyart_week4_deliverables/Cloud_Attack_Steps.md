# Cloud_Attack_Steps

**Lab prerequisites**
- AWS lab account or local mock environment (CloudGoat recommended)
- Pacu installed for automated cloud recon and exploitation

**Steps**
1. Use awscli to enumerate buckets: aws s3api list-buckets
2. Use Pacu modules: enum_s3, find_iam_principals
3. Validate S3 permissions and simulate downloading mock data: aws s3 cp s3://<bucket>/mockdata ./mockdata
4. If an over-privileged role exists, simulate role assumption in lab to validate impact.
5. Log all actions and forward logs to SIEM in lab for detection analysis.

**Safety**
- Use only on your authorized lab accounts and test data.
