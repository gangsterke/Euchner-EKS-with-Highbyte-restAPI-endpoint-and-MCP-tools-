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
		"highbyte": {
			"command": "npx",
			"args": [
			"-y",
			"mcp-remote",
			"http://192.168.2.41:45345/mcp/",
			"--allow-http",
			"--transport",
			"http-only",
			"--header",
            "Authorization:${AUTH_HEADER}"
			],
			"env": {
			"AUTH_HEADER": "Bearer <your key>"
			}
		}


        
**MCP tooling**


<img width="1149" height="944" alt="image" src="https://github.com/user-attachments/assets/d25a81bf-be7b-42e5-b322-687bc4eac291" />

<img width="778" height="567" alt="image" src="https://github.com/user-attachments/assets/f8bbcbaf-efb7-4933-8681-9b7cc39588be" />
