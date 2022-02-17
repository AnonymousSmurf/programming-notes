# AMI (Amazon Machine Image)
An Amazon Machine Image (AMI) is **used to create virtual servers (Amazon Elastic Compute Cloud or EC2 instances) in the Amazon Web Services (AWS) environment**. Different types of instances can be launched from a single AMI to support the hardware of the host computer used for the instance.

## Use an AMI
The following diagram summarizes the **AMI lifecycle**. After you create and register an AMI, you can use it to launch new instances. (You can also launch instances from an AMI if the AMI owner grants you launch permissions.)

You can copy an AMI within the same AWS Region or to different AWS Regions. When you no longer require an AMI, you can deregister it.

After you launch an instance from an AMI, you can connect to it. When you are connected to an instance, you can use it just like you use any other server.

*Lifecycle Example:*
![[ami-lifecycle.png]]
#AWS 