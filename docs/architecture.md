\# AWS 3-Tier Architecture



Architecture Flow



User

&#x20;|

&#x20;v

Application Load Balancer

&#x20;|

&#x20;v

EC2 Web Server (Private Subnet)

&#x20;|

&#x20;v

RDS MySQL Database (Private Subnet)





&#x20;Network Design



VPC

|

|-- Public Subnet

|     |

|     |-- Load Balancer

|

|-- Private Subnet

&#x20;     |

&#x20;     |-- EC2 Instance

&#x20;     |

&#x20;     |-- RDS Database





&#x20;Security



\- SSH access through Security Group

\- HTTP access through Load Balancer

\- Database available only from EC2 server

