# Azure-VM-Backup-and-Restore
This hands-on lab, I am going to demonstrate Azure VM backup.

Pre-requisites: a Resource Group and a VM
<img src="images/sydney-rg.png" alt="">

Step 1: Create a backup
Go to VM and select Backup and 
•	create a Recover Services vault 
•	and create a backup policy
<img src="images/lab1-vm-backup.png" alt="">
<img src="images/create-policy.png" alt="">
<img src="images/vault-sydney-vm01.png" alt="">

If we want to know the progress of our backup: go Vault-sydney-vmo1 then select Backup jobs
<img src="images/backup-jobs.png" alt="">

Step 2: Restore VM
To restore the VM, I need to stop the VM running first and I need to create a storage account. The region has to be the same at the Recover Services vault’s.
<img src="images/stagingrecoverydemo.png" alt="">
Go to VM and on the Operations select Backup. Click Restore, then select Restore point then you will see a snapshot the File-system Consistent.
<img src="images/restore-point.png" alt="">
Now choose Restore Configuration, crate a new VM and follow the instruction as the image below:
<img src="images/restore-vm.png" alt="">
Then go back to the Recover Services vault to see our restore progress.
<img src="images/backup-progress.png" alt="">
