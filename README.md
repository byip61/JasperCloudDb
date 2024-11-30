# JasperCloudDb
JasperCloud database project using PostgreSQL.

## PostgreSQL Setup with Docker
1. Install [Docker Desktop](https://www.docker.com/get-started/).
2. In Docker Desktop, open the built-in terminal and login using ```docker login --username {username}```.
3. Run ```docker pull postgres```.

## Creating the Database Container
1. Clone the repository to your local machine.
2. In the Docker Desktop terminal, cd to the *docker* folder in this repository.
3. Run ```docker-compose up```.
   
## Setting Up Azure Data Studio
1. Install [Azure Data Studio](https://learn.microsoft.com/en-us/azure-data-studio/download-azure-data-studio?tabs=win-install%2Cwin-user-install%2Credhat-install%2Cwindows-uninstall%2Credhat-uninstall).
2. Open Azure Data Studio and install the **PostgreSQL** extension via the extension manager.
3. Open a new connection and fill in/select the following:
   - Connection type (select): ```PostgreSQL```
   - Server name: ```localhost```
   - Authentication type (select): ```Password```
   - User name: ```jc_admin```
   - Password: ```jaspercloud```
4. Connect to the server.

## Creating Tables Using Entity Framework
1. Clone the [JasperCloud](https://github.com/byip61/JasperCloud) repository.
2. In the built-in terminal on Visual Studio or Visual Studio Code, run ```dotnet ef database update -v --project JasperCloud```