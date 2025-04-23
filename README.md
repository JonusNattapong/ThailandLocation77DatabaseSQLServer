# ThailandLocation77DatabaseSQLServer

Thailand Database [SQLServer] ฐานข้อมูล ประเทศไทย รายชื่อ จังหวัด, อำเภอ, ตำบล ,รหัสไปรษณีย์ ในประเทศไทย

- รายชื่อภาค 6 ภาค
- รายชื่อจังหวัด 77 จังหวัด / ภาษาอังกฤษ
- รายชื่ออำเภอ 998 อำเภอ / 729 อำเภอ ภาษาอังกฤษ
- รายชื่อตำบล 8,860 ตำบล

## Set database collation

```sql
ALTER DATABASE ... COLLATE Thai_CI_AS;
```

โดยที่:

- `...` คือ DATABASE name

ใช้คำสั่ง sqlcmd ต่อไปนี้เพื่อนำเข้าข้อมูล:

## การนำเข้าฐานข้อมูล

```sql
sqlcmd -S "..." -d "..." -U "sa" -P "..." -i "..." -f 65001
```

โดยที่:

- `-S` คือ Server name
- `-d` คือ Database name
- `-U` คือ Username
- `-P` คือ Password
- `-i` คือ Input file path
- `-f` คือ Code page of the input file (65001 = UTF-8)

## Original Data

- Original: <https://www.thaicreate.com/member-profile/uid-100725.html> [AT12]

- Original Eng:<https://github.com/kongvut/thai-province-data> [kongvut]
