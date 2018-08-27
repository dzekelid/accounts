{
  "info": {
    "name": "AWS Identity and Access Management API Delete Account Alias",
    "_postman_id": "652ce18f-7407-4304-b0a8-d0a5782e65c3",
    "description": "Deletes the specified AWS account alias.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "OpenID Connect Providers",
      "item": [
        {
          "id": "9fd0145f-0eed-46b5-ab75-73dcc0e6d0b1",
          "name": "addClientIDToOpenIDConnectProvider",
          "request": {
            "url": "http://example.com/api/?Action=AddClientIDToOpenIDConnectProvider?ClientID=ClientID&OpenIDConnectProviderArn=OpenIDConnectProviderArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds a new client ID (also known as audience) to the list of client IDs already\n      registered for the specified IAM OpenID Connect (OIDC) provider resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c034e06-5e12-4f9b-b931-84a0de967f57"
            }
          ]
        },
        {
          "id": "74c28191-f1d3-456f-8c81-1ad9550768f1",
          "name": "createOpenIDConnectProvider",
          "request": {
            "url": "http://example.com/api/?Action=CreateOpenIDConnectProvider?ClientIDList.member.N=ClientIDList.member.N&ThumbprintList.member.N=ThumbprintList.member.N&Url=Url",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an IAM entity to describe an identity provider (IdP) that supports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f04b710-c1c7-4997-8dc6-54106c9d766b"
            }
          ]
        }
      ]
    },
    {
      "name": "Role Instance",
      "item": [
        {
          "id": "e4a0bc56-1819-4e4b-91ef-cd4acb38a594",
          "name": "addRoleToInstanceProfile",
          "request": {
            "url": "http://example.com/api/?Action=AddRoleToInstanceProfile?InstanceProfileName=InstanceProfileName&RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the specified IAM role to the specified instance profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02cf5476-d141-4a4c-bcdd-c6341d35b2a0"
            }
          ]
        }
      ]
    },
    {
      "name": "User Groups",
      "item": [
        {
          "id": "554fdb1c-90e1-4482-a7fb-c373472a9f65",
          "name": "addUserToGroup",
          "request": {
            "url": "http://example.com/api/?Action=AddUserToGroup?GroupName=GroupName&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the specified user to the specified group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0f19ddff-0092-4aba-ac92-3b25e76a6f2f"
            }
          ]
        }
      ]
    },
    {
      "name": "Group Policies",
      "item": [
        {
          "id": "668e3a93-1ae3-4c13-b3fa-35927691d593",
          "name": "attachGroupPolicy",
          "request": {
            "url": "http://example.com/api/?Action=AttachGroupPolicy?GroupName=GroupName&PolicyArn=PolicyArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches the specified managed policy to the specified IAM group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "340f4312-4b71-47c1-ae3f-5d82475663b4"
            }
          ]
        }
      ]
    },
    {
      "name": "Role Policies",
      "item": [
        {
          "id": "a61c0889-3d30-4cc8-bce0-e9865039386d",
          "name": "attachRolePolicy",
          "request": {
            "url": "http://example.com/api/?Action=AttachRolePolicy?PolicyArn=PolicyArn&RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches the specified managed policy to the specified IAM role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3afb21cf-afc5-478a-865d-8ba1c3ff34af"
            }
          ]
        }
      ]
    },
    {
      "name": "User Policies",
      "item": [
        {
          "id": "44e700c1-2523-4acc-ac81-2231a1a7a4f3",
          "name": "attachUserPolicy",
          "request": {
            "url": "http://example.com/api/?Action=AttachUserPolicy?PolicyArn=PolicyArn&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches the specified managed policy to the specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e28368f0-e00a-4616-9f6a-b09f208262dc"
            }
          ]
        }
      ]
    },
    {
      "name": "Passwords",
      "item": [
        {
          "id": "23b17e07-0c1f-4659-8a5f-1cb5f6000068",
          "name": "changePassword",
          "request": {
            "url": "http://example.com/api/?Action=ChangePassword?NewPassword=NewPassword&OldPassword=OldPassword",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Changes the password of the IAM user who is calling this action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dfedfd92-f0e5-48e2-b1b8-0f2d4a32cad9"
            }
          ]
        }
      ]
    },
    {
      "name": "Access Keys",
      "item": [
        {
          "id": "413232c6-c771-44d5-b7c0-3ea67b437e6f",
          "name": "createAccessKey",
          "request": {
            "url": "http://example.com/api/?Action=CreateAccessKey?UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new AWS secret access key and corresponding AWS access key ID for the\n      specified user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d0c8163-086a-4254-9e53-8c8b8fcc3bdf"
            }
          ]
        },
        {
          "id": "3e947156-13e2-4c92-8c96-0719900f4fb8",
          "name": "deleteAccessKey",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAccessKey?AccessKeyId=AccessKeyId&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the access key pair associated with the specified IAM user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73d89bac-569c-4fbf-82a7-e743c0674c1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Alias",
      "item": [
        {
          "id": "ad38307b-6fc6-4ed7-8dcf-fe115d60ae3f",
          "name": "createAccountAlias",
          "request": {
            "url": "http://example.com/api/?Action=CreateAccountAlias?AccountAlias=AccountAlias",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an alias for your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ab8ad371-cf4c-4554-876f-3ee61f3af521"
            }
          ]
        },
        {
          "id": "73ae6e0e-2af2-4bf8-a4c3-ef214dbccc23",
          "name": "deleteAccountAlias",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAccountAlias?AccountAlias=AccountAlias",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified AWS account alias."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e40431a1-81d9-4698-9bf3-ef231d8dfe26"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "c48ca41e-2210-45d1-9eac-99d9070cb97d",
          "name": "createGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateGroup?GroupName=GroupName&Path=Path",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f64c80f1-3170-4f5b-bfe5-823f2c1818fa"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance Profiles",
      "item": [
        {
          "id": "e2691482-c738-497a-bdb0-7c3b16127086",
          "name": "createInstanceProfile",
          "request": {
            "url": "http://example.com/api/?Action=CreateInstanceProfile?InstanceProfileName=InstanceProfileName&Path=Path",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new instance profile."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dec5fa72-3f89-433c-a07e-f7357cbdc99e"
            }
          ]
        }
      ]
    },
    {
      "name": "Login Profiles",
      "item": [
        {
          "id": "7328546b-d02c-4588-8053-c40ec30f022b",
          "name": "createLoginProfile",
          "request": {
            "url": "http://example.com/api/?Action=CreateLoginProfile?Password=Password&PasswordResetRequired=PasswordResetRequired&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a password for the specified user, giving the user the ability to access AWS\n      services through the AWS Management Console."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d89f92de-403e-443e-8609-6a7920ff4c5f"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "e735d8bd-ef13-4c9a-86d3-cc52700f23a5",
          "name": "createPolicy",
          "request": {
            "url": "http://example.com/api/?Action=CreatePolicy?Description=Description&Path=Path&PolicyDocument=PolicyDocument&PolicyName=PolicyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new managed policy for your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "002609cc-c32f-46c1-8bcb-8b569bf77a99"
            }
          ]
        },
        {
          "id": "c955afdb-69a9-417c-ae8b-c46682eedcbd",
          "name": "createPolicyVersion",
          "request": {
            "url": "http://example.com/api/?Action=CreatePolicyVersion?PolicyArn=PolicyArn&PolicyDocument=PolicyDocument&SetAsDefault=SetAsDefault",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new version of the specified managed policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15a82476-b5cc-445b-a1b4-e7f9f9cbfe4d"
            }
          ]
        }
      ]
    },
    {
      "name": "Roles",
      "item": [
        {
          "id": "5df5a494-3da4-4d16-b170-8c4b6aed61cf",
          "name": "createRole",
          "request": {
            "url": "http://example.com/api/?Action=CreateRole?AssumeRolePolicyDocument=AssumeRolePolicyDocument&Path=Path&RoleName=RoleName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new role for your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f148e687-b85a-4ee9-bc6c-921db1cef71b"
            }
          ]
        }
      ]
    },
    {
      "name": "SAML Providers",
      "item": [
        {
          "id": "62995ff8-6e17-422a-9a86-3989683330e7",
          "name": "createSAMLProvider",
          "request": {
            "url": "http://example.com/api/?Action=CreateSAMLProvider?Name=Name&SAMLMetadataDocument=SAMLMetadataDocument",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an IAM resource that describes an identity provider (IdP) that supports SAML\n      2."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85092e2d-cc0c-4cb6-a179-dc34a33ce69e"
            }
          ]
        }
      ]
    },
    {
      "name": "Service Specific Credentials",
      "item": [
        {
          "id": "4b2b8c7f-4ae4-4fb0-a0c3-57e253801f3a",
          "name": "createServiceSpecificCredential",
          "request": {
            "url": "http://example.com/api/?Action=CreateServiceSpecificCredential?ServiceName=ServiceName&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Generates a set of credentials consisting of a user name and password that can be used\n      to access the service specified in the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f751950-f6d1-4658-b0eb-a2e29ceae80f"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "16e18820-beb8-4386-8653-375d99655653",
          "name": "createUser",
          "request": {
            "url": "http://example.com/api/?Action=CreateUser?Path=Path&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new IAM user for your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a37d1c8-adf6-4aa1-a365-98ba1dd790f2"
            }
          ]
        }
      ]
    },
    {
      "name": "Virtual MFA Device",
      "item": [
        {
          "id": "b029c2c3-f19b-4b3b-8386-0128a3f63fc4",
          "name": "createVirtualMFADevice",
          "request": {
            "url": "http://example.com/api/?Action=CreateVirtualMFADevice?Path=Path&VirtualMFADeviceName=VirtualMFADeviceName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new virtual MFA device for the AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1491359e-27a6-473a-a75a-b51f5e930461"
            }
          ]
        },
        {
          "id": "e5ae0a01-2d43-45cb-8373-04ab9ee7c3fd",
          "name": "deactivateMFADevice",
          "request": {
            "url": "http://example.com/api/?Action=DeactivateMFADevice?SerialNumber=SerialNumber&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deactivates the specified MFA device and removes it from association with the user name\n      for which it was originally enabled."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3fd5d16-a166-4305-ba91-9b65675791e5"
            }
          ]
        }
      ]
    }
  ]
}