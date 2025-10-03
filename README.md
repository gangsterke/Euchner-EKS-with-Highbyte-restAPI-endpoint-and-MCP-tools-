# Euchner-EKS-with-Highbyte-restAPI-endpoint-and-MCP-tools-
Used Highbyte to create a restAPI endpoint and MCP tooling to work with the Euchner EKS system

**SQLite DB creation:**

    sqlite3 eksSQLiteDB.db
    create table tblUserDataBase (keyID varchar(20), Locked Bool, Last_name varchar(20),First_name varchar(20), KeyCRC varchar(20), accessLevel         int);

    Keys can be added via the insert commands or via the MCP tooling and Claude Desktop for instance:
    
    insert into tblUserDataBase VALUES ('KEY1', false, 'Gits', 'Koen', 'ERT233', 7);
    insert into tblUserDataBase VALUES ('KEY2', false, 'Kilo', 'Peter', 'ERT23A', 4);

<img width="644" height="324" alt="image" src="https://github.com/user-attachments/assets/8ff502a5-7283-4a51-9cb3-23a04a63155c" />


**MCP tooling**
<img width="778" height="567" alt="image" src="https://github.com/user-attachments/assets/f8bbcbaf-efb7-4933-8681-9b7cc39588be" />
