# SEMANTIC VERSIONING

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/kvix65tpddjk4grv5m2n.png)
 
`Major` จะเป็นตัวเลขในการเปลี่ยน version ครั้งใหญ่ เช่น เปลี่ยนโฉม UI เลย ตัวเลข Major จะเปลี่ยนเพิ่มขึ้น ก็ต่อเมื่อ API เปลี่ยนแบบ breaking change หมายถึงเปลี่ยนแปลงแบบ application หรือ software รอบข้าง มีสิทธิ์พัง กระทบ จำเป็นต้องอัพเดต code

`Minor`: เป็นการเปลี่ยนในลักษณะการเพิ่มของใหม่ feature ใหม่ ในลักษณะ backward compatible หมายความ การเพิ่มใหม่ ต้องยังคงทำให้เก่ายังทำงานได้ปกติ (คือ code feature เก่าเปลี่ยนแปลงได้ แต่ผลคือ feature เก่ายังต้องทำงานได้เหมือนเดิม)

`Patch`: เป็นตัวเลขย่อยหลักสุดท้าย นั่นคือ มีการเปลี่ยนแปลง code ในลักษณะของการซ่อมแซมของเดิมเท่านั้น (ไม่ทำให้ feature เดิมขาดหายไป) แต่เป็นการ fix ซ่อม เพื่อแก้ bug แก้ defect เท่านั้น

## Command Line

init

```sh
$ git flow init -d
```

create git flow success
```sh
Using default branch names.
No branches exist yet. Base branches must be created now.
Branch name for production releases: [master]
Branch name for "next release" development: [develop]

How to name your supporting branch prefixes?
Feature branches? [feature/]
Bugfix branches? [bugfix/]
Release branches? [release/]
Hotfix branches? [hotfix/]
Support branches? [support/]
Version tag prefix? []
Hooks and filters directory? [D:/DEMO/GIT/gitflow-version/.git/hooks]
```

## Start a new feature

```sh
$ git flow feature start feature-first-commit

Switched to a new branch 'feature/feature-first-commit'

Summary of actions:
- A new branch 'feature/feature-first-commit' was created, based on 'develop'
- You are now on branch 'feature/feature-first-commit'

Now, start committing on your feature. When done, use:

     git flow feature finish feature-first-commit
```

