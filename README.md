# Backup in AWS for EC2
Amazon machine Image and Snapshots

```bash
There are two types of backup we can create in AWS such as AMI and Snapshots.
AMI: is a complete copy of our Ec2 instance, We can restore a whole data including os with help of AMI.
Snapshot: is a copy of our EBS volume (hard disk) only.
```

# Creating an AMI
```bash
1. Go to Ec2 Dashboard and select the instance which you want to take backup.
2. Navigate to Actions.
3. Select Images and Template.
4. Click on Create Image.
5. Provide the desired name to the Image.
6. Give appropriate Discription.
7. No Reboot: Enable the button, if we dont select the checkbox instance will get restart after creating image and impact the production.
8. In the storage part check the delete on termination and if you will require the volume even after terminating the server uncheck the box.
9. In the tag options select tag image and snapshot together.
10. Click on create Image.
Note: AMI will create snapshot of your every attached volume so there will be no need of taking Snapshot seperately.
```
# Creating Snapshots
```bash
1. Go to Ec2 Dashboard and Navigate to Elastic Block storage (EBS).
2. Click on snapshots.
3. Click on the Create snapshot
4. Select resource type accoring to our requirement. Select volume if you want to take backup of specific disk or select instance to take back up of all disks attached to a server.
5. If you select volume : Select the volume ID
6. If you select Instance : Select instance ID
7. Give discription in required.
8. Click on Create snapshot and snapshot will get created.
```
