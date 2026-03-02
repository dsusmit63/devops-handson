# Linux Volume Management

## Task 1: Introduction to Volume Management
- What is Linux Volume? When you create an EC2 Instance minimum volume that is attached to your instance?
- Which service in AWS lets you create volumes?
- Difference between root volume vs data volume.
- Run lsblk, df -h. What information does these both commands show?
- Difference between volume attaching and volume mounting

## Task 2: Create and attach volume
- Create 3 EBS volumes (10G, 12G, 14G). Check their current status (creating/available).
- Attach them (once available) with your EC2 instance. Check their current status.
- Run lsblk and verify if all the blocks are successfully attached to your instance.
- Run df -h and note what did you notice?

## Task 3: LVM
- Run lvm as non-root user (ubuntu). Did you see any warning?
- If yes Run lvm as root user (sudo su)
- Create 3 physical volumes from attached EBS blocks/volumes.Run pvs to view all of the created physical volumes.
- Create a volume group using first two physical volumes and run vgs to view details of the created volume group.
- Create a logical volume of 10G from the volume group and run lvs to view the details of the created logical volume.
- Run lsblk now and view the details

## Task 4: Mount logical volume
- Create a mountpoint directory (mkdir /mnt/my-lv-mount)
- Format the logical volume before mounting
- Mount the logical volume to the mountpoint
- Create any file inside /mnt/my-lv-mount
- Check if it is accessible from /
- Run df -h and verify if the mounted loggical volume is listed there or not.
- Unmount the volume. Now try to read the same file from /. Is it accessible now? If not why?
- Now again mount the same volume. Check if the file is there inside /mnt/my-lv-mount?
