# How to add a user to a list of teamdrives:
1. Use the Export.Teamdrive.List.2.CSV.bat file to export team drive list into a CSV file. It will export teamdrive with user name in column 1, teamdrive id in to column 2 and teamdrive name in column 3. You can ignore other columns and leave them there. If you want to keep only first three columns, you need to remove extran tokens from the Add.A.User.Access.Permission.2.All.Teamdrives.bat script
![image](https://github.com/redwanulalam/GAMADV-XTD3/assets/7146686/59c8cd28-5b3e-454b-ba60-99a2ce44d287)

2. Copy the teamdrive rows you need to add for a user in to a new CSV file
3. Use the Add.A.User.Access.Permission.2.All.Teamdrives.bat script to add the user access permission to those teamdrives 


teamdrive-sample.csv CSV file with first three columns:
```
User	id	name
randomUser1@example.com	1234567890	Drive 1
randomUser2@example.com	2345678901	Drive 2
randomUser3@example.com	3456789012	Drive 3
randomUser1@example.com	4567890123	Drive 4
randomUser2@example.com	5678901234	Drive 5
randomUser3@example.com	6789012345	Drive 6
randomUser1@example.com	7890123456	Drive 7
randomUser2@example.com	8901234567	Drive 8
randomUser3@example.com	9012345678	Drive 9
randomUser1@example.com	123456789	Drive 10
randomUser2@example.com	1234123412	Drive 11
randomUser3@example.com	2345234523	Drive 12
randomUser1@example.com	3456345634	Drive 13
randomUser2@example.com	4567456745	Drive 14
randomUser3@example.com	5678567856	Drive 15
randomUser1@example.com	6789678967	Drive 16
randomUser2@example.com	7890789078	Drive 17
randomUser3@example.com	8901890189	Drive 18
randomUser1@example.com	9012901290	Drive 19
randomUser2@example.com	123012301	Drive 20
randomUser3@example.com	1234123412	Drive 21
randomUser1@example.com	2345234523	Drive 22
randomUser2@example.com	3456345634	Drive 23
randomUser3@example.com	4567456745	Drive 24
randomUser1@example.com	5678567856	Drive 25
randomUser2@example.com	6789678967	Drive 26
randomUser3@example.com	7890789078	Drive 27
```
![image](https://github.com/redwanulalam/GAMADV-XTD3/assets/7146686/5a3c6198-bc5b-4e30-b297-fa2ff44e1607)


Sample successful output:
```
c:\GAMADV-XTD3>teamdrive-access.bat
Command: gam add drivefileacl id user User role >>>organizer<<<

ERROR: Invalid argument
Help: Syntax in file c:\GAMADV-XTD3\GamCommands.txt
Help: Documentation is at https://github.com/taers232c/GAMADV-XTD3/wiki
User: randomUser1@example.com, Add 1 Drive File/Folder ACL
  User: randomUser1@example.com, Drive File/Folder ID: 1234567890, Permission ID: randomUser1@example.com, Added
  Random Drive
    id: 9876543210
    type: user
    emailAddress: randomUser1@example.com
    domain: example.com
    role: organizer
    permissionDetails:
      role: organizer
        type: member
        inherited: False
    photoLink: https://lh3.googleusercontent.com/a/default-user=s64
    deleted: False
User: randomUser2@example.com, Add 1 Drive File/Folder ACL
  User: randomUser2@example.com, Drive File/Folder ID: 2345678901, Permission ID: randomUser2@example.com, Added
  Random Drive
    id: 0123456789
    type: user
    emailAddress: randomUser2@example.com
    domain: example.com
    role: organizer
    permissionDetails:
      role: organizer
        type: member
        inherited: False
    photoLink: https://lh3.googleusercontent.com/a/default-user=s64
    deleted: False
User: randomUser3@example.com, Add 1 Drive File/Folder ACL
  User: randomUser3@example.com, Drive File/Folder ID: 3456789012, Permission ID: randomUser3@example.com, Added
  Random Drive
    id: 1230123012
    type: user
    emailAddress: randomUser3@example.com
    domain: example.com
    role: organizer
    permissionDetails:
      role: organizer
        type: member
        inherited: False
    photoLink: https://lh3.googleusercontent.com/a/default-user=s64
    deleted: False
User: randomUser4@example.com, Add 1 Drive File/Folder ACL
  User: randomUser4@example.com, Drive File/Folder ID: 4567890123, Permission ID: randomUser4@example.com, Added
  Random Drive
    id: 2345234523
    type: user
    emailAddress: randomUser4@example.com
    domain: example.com
    role: organizer
    permissionDetails:
      role: organizer
        type: member
        inherited: False
    photoLink: https://lh3.googleusercontent.com/a/default-user=s64
    deleted: False
User: randomUser5@example.com, Add 1 Drive File/Folder ACL
  User: randomUser5@example.com, Drive File/Folder ID: 5678901234, Permission ID: randomUser5@example.com, Added
  Random Drive
    id: 3456345634
    type: user
    emailAddress: randomUser5@example.com
    domain: example.com
    role: organizer
    permissionDetails:
      role: organizer
        type: member
        inherited: False
    photoLink: https://lh3.googleusercontent.com/a/default-user=s64
    deleted: False
```

