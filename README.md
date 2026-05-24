# Secure Cross-Account Data Pipeline & Auditing Architecture

## Project Overview
This project demonstrates a secure AWS IAM architecture designed to protect sensitive cloud data using temporary role-based access instead of permanent permissions.

## Problem Statement
Organizations face security risks when users are given excessive or direct access to cloud resources. This project focuses on implementing least privilege and secure temporary access controls.

## AWS Services Used
- AWS IAM
- Amazon S3
- AWS CloudTrail
- IAM Access Analyzer

## Security Concepts Implemented
- Role-Based Access Control (RBAC)
- Least Privilege
- AssumeRole
- Explicit Deny Policies
- Trust Relationships
- Cloud Auditing

## Architecture Flow
dev2 → AssumeRole → DataAccessRole → Secure S3 Access → CloudTrail Monitoring

## Project Features
- Secure S3 bucket with blocked public access
- Encrypted storage for sensitive data
- Temporary role-based access
- Restricted delete operations
- CloudTrail auditing and monitoring
- IAM trust relationship configuration

## Scenarios Tested
- User denied direct access
- Temporary role-based access granted
- Restricted destructive actions
- Monitoring AssumeRole activity in CloudTrail

## Learning Outcomes
This project improved my understanding of IAM policies, temporary credentials, trust relationships, least privilege, cloud auditing, and security hardening techniques in AWS.
