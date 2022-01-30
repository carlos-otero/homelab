# Download last ISO from Truenas website

# Upload ISO to proxmox LVE

# Create new VM

# Disk Passthrough

ssh to proxmox machine

Find serial number and unique identifier for the disks

lsblk -o +MODEL,SERIAL

List disks by id

ls /dev/disk/by-id

Add physical disks to TrueNAS VM

qm set ID -scsi* /dev/disk/by-id/UNIQUE_ID
