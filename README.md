# A-Trak - Push files to the Cloud!
A-Trak is a tool to manage deploying content and resources to the cloud. It can also be used to backup content off of your primary cloud.
Choose to move data in 9 different directions, between Windows Azure, Amazon S3 and Windows Folders.

This is a utility for easily pushing files to Blob Storage on Windows Azure or S3 on Amazon. It is for developers to easily leverage Windows Azure's or Amazon's CDN services.

We have built this to help you with your development and deployment process. Agile Business Cloud Solutions Ltd. uses this tool as part of an automated deployment solution to Windows Azure.


## Getting Started

* Clone the repository at <code>git clone git@github.com:AgileBusinessCloud/A-Trak.git</code>
* Run the A-Trak.csproj file in Visual Studio
* Configure the command line arguments in DEBUG tab of Project Properties
  * Example Folder to Azure Blob: <code>"C:\Project\MyMVCWebSite\FromFolder" "UseDevelopmentStorage=true" "tocontainer"</code>
  * Example Folder to Amazon S3: <code>"C:\Project\MyMVCWebSite\FromFolder" "SecretKey" "SecretAccessKey" "tobucket"</code>
  * Example Folder to Folder: <code>"C:\Project\MyMVCWebSite\FromFolder" "C:\Project\MyMVCWebSite\ToFolder"</code>
  * Example Azure Blob to Folder: <code>"UseDevelopmentStorage=true" "fromcontainer" "C:\Project\MyMVCWebSite\ToFolder"</code>
  * Example Azure Blob to Azure Blob: <code>"UseDevelopmentStorage=true" "fromcontainer" "UseDevelopmentStorage=true" "tocontainer"</code>
  * Example Azure Blob to Amazon S3: <code>"UseDevelopmentStorage=true" "fromcontainer" "SecretKey" "SecretAccessKey" "tobucket"</code>
  * Example Amazon S3 to Folder: <code>"SecretKey" "SecretAccessKey" "frombucket" "C:\Project\MyMVCWebSite\ToFolder"</code>
  * Example Amazon S3 to Azure Blob: <code>"SecretKey" "SecretAccessKey" "frombucket"  "UseDevelopmentStorage=true" "tocontainer"</code>
  * Example Amazon S3 to Amazon S3: <code>"SecretKey" "SecretAccessKey" "frombucket" "SecretKey" "SecretAccessKey" "tobucket"</code>
  * first argument: location of files you wish to push to Azure on your local environment
  * second argument: name of the container you want to push to on Azure
  * third argument: connection string
* Run that puppy (Hit F5)!

## SDK's
Microsoft Windows Azure: https://www.windowsazure.com/en-us/develop/net/
Amazon S3: http://aws.amazon.com/sdkfornet/

### Screenshot of configuration arguments

![A-Trak Configuration](https://github.com/AgileBusinessCloud/A-Trak/raw/master/Config.PNG)

## About the Author

Jef King has worked in the software industry for twelve years. Over this time he has experienced a range of responsibilities in various industries. His passion for technology and motivating teams has kept his drive and focus strong. Early on in his career he showed an entrepreneurial spirit, starting multiple small companies. He departed from this to learn more about the software industry by working with larger companies, such as Microsoft. These diverse experiences have given a very unique perspective on teams and software engineering. Since moving back to Vancouver he has built several highly productive software development teams, and inspired others to try similar techniques.

## Contributing

Contributions are always welcome. If you have find any issues with A-Trak, please report them to the [Github Issues Tracker](https://github.com/AgileBusinessCloud/A-Trak/issues?sort=created&direction=desc&state=open).

## Apache 2.0 Licence

Copyright 2012 [Agile Business Cloud Solutions Ltd](http://www.agilebusinesscloud.com)

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

[http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
