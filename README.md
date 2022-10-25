# Manjaro-secure-boot
Setup secure boot setup for Manjaro  and enable dual boot with WIndows 11

## After running the script 
Now, Go to your UEFI-BIOS to manually enrool the keys 
 Copy \"Keys\" folder with \"*.auth\" keys to a FAT formatted file system (you can use EFI system partition). 
 Then enroll : 
     Platform Key (PK)       : Keys/PK/PK.auth 
     Key Exchange Key (KEK)  : Keys/KEK/KEK.auth 
     Signature Database (db) : Keys/db/db.auth 
     #Then Append Signature Database (db) with Microsoft key. 
     Signature Database (db) : Keys/Win/add_MS_db.auth  {Append}
