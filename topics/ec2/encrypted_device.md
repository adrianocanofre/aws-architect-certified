# Encrypted Root Device  

* Snapshot of encrypted volumes are encrypted automatically.  
* Volumes restored from encrypted snapshots are encrypted automatically.  
* You can share snapshots, but only if they are unencrypted.  
* These snapshots can be shared with other AWS accounts or made public.  
* Create a snapshot of the unencrypted root device volume.
* Create a copy of the snapshot and select the encrypt option.  
* create an AMI from the encrypted snapshot.
* Use that AMI to launch new encrypted instances.  


https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/building-shared-amis.html  
https://aws.amazon.com/articles/public-ami-publishing-hardening-and-clean-up-requirements/
