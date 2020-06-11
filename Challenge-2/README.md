Challenge #2

Summary

We need to write code that will query the meta data of an instance within aws and provide a json formatted output. The choice of language and implementation is up to you.

Details:

Go language is used for the solution

Prerequisite:

At least one AWS instance should be up and running to get the meta-data
‘GO ’should be installed on the system where script is executing.

Steps:

Execute the below command to see the json formatted output.

File Name: ec2metadata.go

go run ec2metadata.go

Output as an instance:

{"ami-id":"ami-09d95fab7fff3776c","ami-launch-index":"0","ami-manifest-path":"(unknown)","block-device-mapping":{"ami":"/dev/xvda","root":"/dev/xvda"},"events":{"maintenance":{"history":"[]","scheduled":"[]"}},"hostname":"ip-172-31-54-211.ec2.internal","identity-credentials":{"":""},"instance-action":"none","instance-id":"i-0dcf0a95274953dff","instance-type":"t2.micro","local-hostname":"ip-172-31-54-211.ec2.internal","local-ipv4":"172.31.54.211","mac":"06:1a:b0:11:1b:a9","network":{"interfaces":{"macs":{"06:1a:b0:11:1b:a9":{"device-number":"0","interface-id":"eni-0236120a50d0ce3ca","ipv4-associations":{"52.86.69.93":"172.31.54.211"},"local-hostname":"ip-172-31-54-211.ec2.internal","local-ipv4s":"172.31.54.211","mac":"06:1a:b0:11:1b:a9","owner-id":"525339921445","public-hostname":"ec2-52-86-69-93.compute-1.amazonaws.com","public-ipv4s":"52.86.69.93","security-group-ids":"sg-039f813d228fcfc2a","security-groups":"launch-wizard-1","subnet-id":"subnet-0bbfced44ae9f7ef7","subnet-ipv4-cidr-block":"172.31.48.0/20","vpc-id":"vpc-0c0b51c4bb3b0970f","vpc-ipv4-cidr-block":"172.31.0.0/16","vpc-ipv4-cidr-blocks":"172.31.0.0/16"}}}},"placement":{"availability-zone":"us-east-1e"},"profile":"default-hvm","public-hostname":"ec2-52-86-69-93.compute-1.amazonaws.com","public-ipv4":"52.86.69.93","public-keys":{"0=terraform":"ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCZlDEKl0nxnyS7RGnKxnXNW8Vvnyi0CirrYMiKxE8pEI5T0IWfSYMajAa+bngwcalYAK8wjV5nsKvHotLMQwwqJG+9ZeSCZMv0Q+vKMXQCTUrQB6BwG/hSUUf6tNedLpV3Wv4o+GNVzbZUS0pdcwe4B8l31YWlrsowuc+IOmhwQqHdKCS4DjPJwzsZdIDTmm8YTpNOnCjiAaJHU6CWzk/DwUNbbk4+gJZCKfpUB+/c1UZwOimh5G0k5EVZFXVq4R4ZVpvC2E+PzRx9hEWDeFhjz/1iZ9QmvLkeEEPmsB2aslJNuZZvc9kD9AP+E8lZVcodSIIyMpoF0BLtuL4odz8D terraform"},"reservation-id":"r-0bb440522ebf2d3e3","security-groups":"launch-wizard-1","services":{"domain":"amazonaws.com","partition":"aws"}}
