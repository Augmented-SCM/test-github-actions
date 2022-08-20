# Automatic Sync of Config Files in S3

## Stage 1 : Sync from repostiory to S3 single account.

1. When changes in a specific folder are pushed, actions sync s3 to that account.


## Stage 2: Sync from repository to S3 multiple accounts.

1. When changes are made in a specific folder, actions triggers.
2. Sync to Main Account.
    a. Checkout to master.
    b. Sync to the master s3 account.

3. Sync to the Secondary Account.
    a. Checkout to secondary.
    b. Run s3_update.py
    c. Sync to the secondary account.