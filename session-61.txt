RBAC
----------
expense

trainee --> only read access
senior enginner --> deployments
team leader --> namespace admin
manager --> cluster admin

Authentication and Authorization

Role
RoleBinding
ClusterRole
ClusterRoleBinding

AWS IAM --> RBAC for AWS IAM
EKS -> PaaS, AWS EKS can use IAM as authentication provider. SSO

1. team leader will send an email to create namespace, provide access to diff employees and their permissions

now admin will perform
harish and suresh
harish --> trainee
suresh --> senior devops

1. creation of user

users should access only expense project cluster....

role and permissions

resources --> nouns
verbs --> action

creation of ec2 --> verbs
1. what resources I should have access

data center --> noun
enter into center --> verb, read
creation of server in data center --> verb, create access
update exisiting server in data center --> verb, update access
delete exisiting server in data center --> verb, delete access

https://docs.aws.amazon.com/eks/latest/userguide/auth-configmap.html

admin will email project team that namespace and access is given


1. harish has access to eks describe cluster or not
2. get aws-auth configmap
3. user harish authenticated
4. check role and rolebindings

HPA
------------
horizontal scaling
create one more server when traffic is increased
create one more server when traffic is increased
create one more server when traffic is increased
remove one server when traffic is decreased

vertical scaling --> common resources increases, less privacy, building may not withstand
increase ram and hd and number of CPU cores
increase ram and hd and number of CPU cores
increase ram and hd and number of CPU cores
increase ram and hd and number of CPU cores

autoscaling and autoscaling policy and metric CPU utilisation

24hr --> 8hrs(metric)

a pod is over utlised or less utilised how to decide? based on resource defnition

1. metric server
2. resource defnition inside pod
3. HPA should be attached to deployment

kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml