# SitefinityTimer
This repository contains Sitefinity 8.2 project, which is using the free Bootstrap Timer Template: https://themewagon.com/themes/timer-free-responsive-multi-page-personal-bootstrap-template/

## How to start using it?

1. Clone the repository
2. Go to SitefinityWebApp/App_Data. In this folder you will find the s Timer.zip, containing the Timer.bak, which is a backup of the Timer project's database.
3. Restore the backup in SQL management studio.
4. Go back to SitefinityWebApp/App_Data/sitefinity/Configuration/DataConfig.config and make sure that the connectionString source attribute points to your server:

```<add connectionString="data source=serverName;Integrated Security=SSPI;initial catalog=Timer" providerName="System.Data.SqlClient" dbType="MsSql" name="Sitefinity" />```

5. Currently the bin folder of the project doesn't contain any dlls. You need to get the dlls for Sitefinity 8.2.5900.0 from an existing project or from the _EmptyProject created by the Sitefinity project manager.
6. Host SitefinityWebApp in IIS.
