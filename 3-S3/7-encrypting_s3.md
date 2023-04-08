## types of encryption

## encryption in transit

* SSL/TLS
* HTTPS

###  encryption at rest

* server side encryption
* sse-s3 -> S3-managed keys -> AES 256 bit encryption
* SSE-KMS - key managements service- managed key
* sse-c: customer provided keys

* client side encryption
* you encrypt the file before you upload to s3

## enforcing sse

* console or bucket policy
* x-amz-sse -> parameter included in header -> AES256 (s3 managed keys) or aws:kms (key managed service)