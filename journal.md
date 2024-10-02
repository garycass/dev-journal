## Wednesday 21/10/2019
##### Problem: Jenkins startup
Suggested Solution:
* java -jar jenkins.war --httpPort=8080
* URL: http://localhost:8080/
* ...

*Tags: jenkins*

---
## Monday 20/04/2020
##### Problem: Update TestCafe
Suggested Solution:
* npm outdated (-g for global)
* npm update testcafe (-g for global)
* ...

*Tags: TestCafe*

---
## Wednesday 17/02/2021
##### Problem: SQL Server - Identify most rcently modified stored procedures
Suggested Solution:
```
select name,create_date,modify_date
from sys.procedures
order by modify_date desc
```

*Tags: sql*

---
## Thursday 25/02/2021
##### Problem: Check .NET runtime versions
Suggested Solution:

You can see which versions of the .NET runtime are currently installed with the following command.
```
dotnet --list-runtimes
```

*Tags: .NET*

---
## Friday 07/01/2022
##### Problem: SQL execution time
Suggested Solution:
```
DECLARE @t1 DATETIME;
DECLARE @t2 DATETIME;

SET @t1 = GETDATE();
SELECT /* query one */ 1 ;
SET @t2 = GETDATE();
SELECT DATEDIFF(millisecond,@t1,@t2) AS elapsed_ms;
```

*Tags: sql*

---
## Wednesday 11/01/2023
##### Problem: Find string SQL stored procedures
Suggested Solution:
```
SELECT name
FROM   sys.procedures
WHERE  Object_definition(object_id) LIKE '%mystring%';
```

*Tags: sql*

---
## Wednesday 02/10/2024
##### Problem: Copy a directory retaining its permissions
Suggested Solution:
```
xcopy c:\source_folder_name e:\destination_folder_name /O /X /E /H /K

/E - Copies folders and subfolders, including empty ones.
/H - Copies hidden and system files also.
/K - Copies attributes. Typically, Xcopy resets read-only attributes.
/O - Copies file ownership and ACL information.
/X - Copies file audit settings (implies /O).
```

*Tags: xcopy*
