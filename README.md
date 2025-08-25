# AWS IAM Mini Project

## Overview
This hands-on guide will equip you with the skills needed to set up AWS IAM users, groups, and roles. By following these exercises, you'll gain practical experience in implementing IAM solutions and managing access policies within AWS.

---

## Table of Contents

1. [Accessing IAM in AWS Console](#accessing-iam-in-aws-console)
2. [Creating an IAM Policy](#creating-an-iam-policy)
3. [Creating and Attaching Users](#creating-and-attaching-users)
4. [Managing User Groups](#managing-user-groups)
5. [Attaching Policies to Groups](#attaching-policies-to-groups)
6. [Summary](#summary)

---

## Accessing IAM in AWS Console

1. Log in to your AWS Console.
2. Navigate to **IAM**.

   ![IAM Dashboard](images/1iam.png)

---

## Creating an IAM Policy

1. Select **Policies** from the IAM sidebar.
2. Click **Create policy** (top right).

   ![Create Policy](images/2iam.png)

3. Under the **Service** section, choose **EC2**.
4. Check **All EC2 actions**.

   ![EC2 Actions](images/3iam.png)
   ![Create Policy Steps](images/4iam.png)
   ![Create Policy Confirmation](images/5iam.png)

5. Name your policy (e.g., `policy_for_eric`) and finalize creation.

   ![Name Policy](images/6iam.png)
   ![Policy Created](images/7iam.png)

---

## Creating and Attaching Users

1. Select **Users** and click **Create user**.

   ![Create User](images/8iam.png)
   ![Select/Create User](images/9iam.png)

2. During setup, choose **Attach policies directly** and filter for custom policies.
3. Select the policy you just created (e.g., `policy_for_eric`) and proceed.

   ![Select Custom Policy](images/iam9.png)
   ![Custom Policy Filter](images/iam8.png)

4. Save your changes for future reference.

---

## Managing User Groups

1. Return to the user list.

   ![Return to User List](images/iam7.png)
   ![User List](images/iam6.png)

2. Click on **User groups**.

   ![User Groups](images/iam5.png)
   ![User Groups View](images/iam4.png)

3. Select your user(s).

   ![Select User](images/iamjack.png)
   ![User Selected](images/iamja.png)

4. Add the user to a group and click **Next**.

   ![Add User to Group](images/iamnext.png)
   ![User Added](images/iama.png)
   ![User Added Confirmation](images/iamad.png)
   ![User Added Final](images/iamade.png)

---

## Attaching Policies to Groups

1. Navigate to **Policies** and click **Create policy**.
2. Select **EC2** service and all actions.

   ![EC2 All Actions](images/1pol.png)
   ![EC2 Policy Setup](images/2pol.png)

3. Click **Next** to proceed.

   ![Proceed Next](images/3pol.png)
   ![Proceed Confirmation](images/4pol.png)

4. Expand and add S3 permissions, selecting **All actions**.

   ![Add S3 Policy](images/5pol.png)
   ![S3 Policy Setup](images/6pol.png)

5. Click **Create policy**.

   ![Create Final Policy](images/7pol.png)

6. Go to **User Groups**, select the group (e.g., `Development-team`).

   ![Select Group](images/8pol.png)

7. Under **Permissions**, grant the necessary permissions.

   ![Grant Permissions](images/9pol.png)
   ![Permissions Confirmation](images/pol9.png)
   ![Permissions Overview](images/pol8.png)

8. In **Customer managed policies**, choose the newly created policy (e.g., `Development-team-policy`) and attach it.

   ![Attach Policy](images/pol7.png)

9. You have successfully attached the policy to the group!

   ![Success](images/pol6.png)

---

## Summary

By following the steps above, you have:
- Created custom IAM policies for EC2 and S3.
- Set up IAM users and user groups.
- Assigned and managed permissions with policies.
- Strengthened your real-world AWS IAM implementation skills.

> **Tip:** Always review AWS IAM best practices to ensure your environment is secure and well-managed.

---

*For any questions or further improvements, feel free to contribute to this guide.*
