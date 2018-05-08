# aws-cloudformation-mssql-rds

This repository contains a CloudFormation Template to provision a RDS of AWS with Microsoft SQLServer instance.


Usage
--------

```
aws cloudformation create-stack --stack-name myteststack --template-body file:///home/testuser/mssql.json --parameters ParameterKey=Parm1, DBInstanceClass=db.t2.small, DBInstanceName=testrds, DBPassword=Tempass123, DBUser=testuser, Storage=50
```

Inputs
---------

  | Name | Description | Default | Required |
  |------|-------------|:-----:|:-----:|
  | DBInstanceName | RDS Instance name | - | yes |
  | DBPassword  | Password for the administrator DB user. | - | yes |
  | DBUser | Username for the administrator DB user. | - | yes |
  | Storage | The allocated storage in gigabytes. | `50` | no |
  | DBInstanceClass | The instance type of the RDS instance. | `db.t2.small` | yes | 
  | rds_multi_az | Specifies if the RDS instance is multi-AZ. | `false` | no |
  | VPC | The VPC identifier where security groups are going to be applied. | - | yes |
  | Subnet1/2 | A list of VPC subnet identifiers. | - | yes |

Outputs
---------

  | Name | Description |
  |------|-------------|
  | mssqlurl | Address of the mssql DB instance. |

Contributing
------------
Everybody is welcome to contribute. Please, see [`CONTRIBUTING`][contrib] for further information.

[contrib]: CONTRIBUTING.md

Bug Reports
-----------

Bug reports can be directly sent to authors and/or using github's issues.

-------

