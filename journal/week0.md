# Week 0 — Billing and Architecture

The pricing of aws services is vary depending on the region. Make sure to use the region close to you and see if all services you will utilise are available for the region. And also make sure you set the billing alarm so you don't have unexpected costs.

## Required Homework

### Security Considerations

Created IAM user for security reasons so that I don't use the root account

### Install AWS CLI
https://github.com/mg410/aws-bootcamp-cruddur-2023/blob/main/.gitpod.yml

### IAM account

$ aws sts get-caller-identity
{
    "UserId": "AIDASLCVTX7V3Q76D7ELH",
    "Account": "161240825835",
    "Arn": "arn:aws:iam::161240825835:user/iamadmin"
}

### Recreate Conceptual Diagram in Lucid Charts or on a Napkin

https://lucid.app/lucidchart/b6212c26-eefe-40d7-8569-ec0c51449413/edit?viewport_loc=-231%2C-846%2C1707%2C768%2C0_0&invitationId=inv_81c403b5-c0be-4915-8242-34f928d71032

### Recreate Logical Architectual Diagram in Lucid Charts
https://lucid.app/lucidchart/invitations/accept/inv_a642497a-eaec-42b7-ae4e-911f3abadf28

### Budgets

Created 2 budget alarms for My Zero-Spend Budget and My Monthly Cost Budget
The alarm triggers when your account billing exceeds the threshold you specify. It triggers only when the current billing exceeds the threshold. It doesn't use projections based on your usage so far in the month.
If you create a billing alarm at a time when your charges have already exceeded the threshold, the alarm goes to the ALARM state immediately.    
