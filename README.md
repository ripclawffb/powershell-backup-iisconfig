# Backup-IISConfig
Script to backup IIS and Dotnet configs

## Overview
This script will backup your IIS and DotNet (.NET) configurations, both at the global and site levels. 

## Requirements
* IIS 7.0 or newer
* PowerShell WebAdministration Module

## Workflow
This script will check to see if IIS configuration exists and back them up accordingly

* IIS Configuration
  * Global
    * administration.config
    * applicationHost.config
* DotNet Configuration (x86/x64 - CLR 2.0/4.0)
  * MACHINE
    * machine.config
  * WEBROOT
    * web.config
* IIS/DotNet Configuration
  * Site
    * web.config
    
The files will be copied to the C:\Temp path with a timestamp in the filename of when the backup was made.

## Usage
* Edit the script and set your desired Backup Path
* Run the PowerShell script `.\Backup-IISConfig.ps1`

  
