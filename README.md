# Euchner-EKS-with-Highbyte-restAPI-endpoint-and-MCP-tools-
Used Highbyte to create a restAPI endpoint and MCP tooling to work with the Euchner EKS system

**SQLite DB creation:**

    sqlite3 eksSQLiteDB.db
    create table tblUserDataBase (keyID varchar(20), Locked Bool, Last_name varchar(20),First_name varchar(20), KeyCRC varchar(20), accessLevel         int);

    Keys can be added via the insert commands or via the MCP tooling and Claude Desktop for instance:
    
    insert into tblUserDataBase VALUES ('KEY1', false, 'Gits', 'Koen', 'ERT233', 7);
    insert into tblUserDataBase VALUES ('KEY2', false, 'Kilo', 'Peter', 'ERT23A', 4);

<img width="644" height="324" alt="image" src="https://github.com/user-attachments/assets/8ff502a5-7283-4a51-9cb3-23a04a63155c" />


**Claude Desktop config** for Highbyte MCP server

to be added in claude_desktop_config.json
        **remark: avoid using spaces in the name of the MCP server**

<img width="653" height="388" alt="image" src="https://github.com/user-attachments/assets/d4fed2cf-cdb6-46d0-b71b-e65f26379185" />

        
**MCP tooling**

<img width="762" height="533" alt="image" src="https://github.com/user-attachments/assets/9d405f9a-18e3-409f-831a-2b46ebecc6f5" />


<img width="1153" height="957" alt="image" src="https://github.com/user-attachments/assets/2494a2a8-a181-4c8f-bee8-c5738c383fe2" />

getAllKeyInformation
<img width="1750" height="776" alt="image" src="https://github.com/user-attachments/assets/765f04cc-6a18-4a19-97d6-eb04abafc830" />

getOneKeyInformation

getAccessLevel

<img width="896" height="825" alt="image" src="https://github.com/user-attachments/assets/93b334f9-ee53-451c-b507-427f9e69a1ed" />

updateAccessLevel


**PLC code**

<img width="630" height="645" alt="image" src="https://github.com/user-attachments/assets/11a19bd2-8c8d-44e0-8ffb-9b51c47a454d" />

<img width="700" height="270" alt="image" src="https://github.com/user-attachments/assets/116c2103-f1b7-4687-af13-63a74aece513" />



