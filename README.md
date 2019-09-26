Index No# 16550272
Project Name: Cloud Platform Integration Framework

Download and extract CloudDataTransferringFramework.zip file.

* Cpif.Main.sln is the main solution file which contains all projects.

* Following projects contain Windows Service implementation to upload files to a configured cloud platform and receive files via configured cloud plaform respectively.  
Cpif.Cloud.Sender.WindowsService  
Cpif.Cloud.Receiver.WindowsService

* Following projects contains actual executables of cloud based file upload service and file download service which execute by above mentioned Windows Services.  
Cpif.Cloud.Receiver.App  
Cpif.Cloud.Sender.App

* Actual cloud plaforms integration (Azure and Amazon AWS) implemented in below projects. Following projects represents as plug-ins which are dynamically invoked by above mentioned executables without having hardbound references.  
Cpif.Cloud.Receiver.Azure.Plugin  
Cpif.Cloud.Receiver.Amazon.Plugin

* Following projects contain common logics and those projects could be referenced by any other projects in the solution. (e. g. Log4Net logger, common file operations).  
Cpif.Cloud.Common  
Cpif.Cloud.Common.Utility

* Following projects contain MEF framework (plug-in architecture) related components.  
Cpif.Framework.Mef  
Cpif.Framework.Mef.Interfaces  
