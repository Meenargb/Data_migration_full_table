MS SQL Server to PostgreSQL Data Migration Tool
📌 Overview

This project provides a Windows-based data migration tool to transfer database tables from MS SQL Server to PostgreSQL. The tool validates network connectivity, checks port accessibility, and allows selective or full table migration with real-time progress updates. 

Steps to be followed for Migrate…

✨ Features

Connects to MS SQL Server and PostgreSQL

Validates network connectivity (Ping & Telnet)

Supports table-wise or full database migration

Shows migration progress and error logs

Simple GUI-based execution (no coding required)

⚠️ Trial Version Limitations

This is a trial version

Supports up to 20,000 records per table

For larger datasets, a premium version is required

🖥️ System Requirements

Windows 10 / 11

MS SQL Server (source)

PostgreSQL (destination)

Network access between source and destination systems

Required ports open:

SQL Server: 1433 (or custom)

PostgreSQL: 5432

🚀 How to Use the Tool (Step-by-Step)
1️⃣ Check Network Connectivity

Run ping from your system to the SQL Server machine:

ping <SQL_Server_IP> -t

2️⃣ Verify SQL Server Port Access

Enable Telnet Client on Windows and run:

telnet <SQL_Server_IP> <SQL_Port>


A blank screen means the port is accessible.

3️⃣ Configure PostgreSQL Access

Open pg_hba.conf from PostgreSQL data directory

Add your system IP address

Save the file and restart PostgreSQL service

4️⃣ Verify PostgreSQL Port
telnet <PostgreSQL_IP> 5432

5️⃣ Create Destination Database

Create a blank PostgreSQL database (example: Data_Transfer).

6️⃣ Run the Migration Tool

Open the .exe file

Enter MS SQL Server credentials

Click MSSQL DB to validate connection

Select tables (or choose All Tables)

Enter PostgreSQL credentials

Click PGSQL DB

Click Migrate Tables to start migration

📦 Downloading the Tool (GitHub Releases)

🔽 How to Download

Go to the Releases section of this repository

Open the latest release

Download the attached .exe file under Assets

👉 Direct link:

[https://github.com/<your-username>/<repo-name>/releases/latest](https://github.com/Meenargb/Data_migration_full_table/releases/tag/v1.0.0)


🏷️ Versioning

v1.0.0 – Initial trial release (20,000 records/table limit)

📄 License

This project is provided for trial and evaluation purposes.
