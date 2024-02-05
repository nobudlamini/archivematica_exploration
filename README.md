<h1>Exploration of Archivematica using Virtualisation</h1>
</br></br>

<h2>Description</h2>
In this exercise, I am exploring the different features and settings of archivematica that I want to familiarise myself with ahead of implementing archivematica on an AWS S3 environment. I will share the plans of how we plan to implement the final solution on S3 at a later point
</br></br>

<h2>Languages and Utilities Used</h2>

- <b>Vagrant</b> 
- <b>VIrtual Box</b>

<h2>Environments Used </h2>

- <b>Linux</b> 

<h2>Setup walk-through:</h2>


(all the detail information and system requirements is provided by Archivematica at</br>
https://www.archivematica.org/en/docs/archivematica-1.15/getting-started/quick-start/quick-start/#installing-on-vm)</br>

Installation using virtualbox and vagrant: </br>
https://www.virtualbox.org/ </br>
https://www.vagrantup.com/


<b>Implementation of Archivematica using Vagrant</b>:</br> 
On the command line, run:</br> 
<code>mkdir archivematica-vagrant && cd archivematica-vagrant</code></br>
This action creates a new directory for Vagrant from current location
</br>
</br>
<code>vagrant init artefactual/archivematica</code></br>
This action converts the current directory to be a Vagrant directory
</br>
</br>
<code>vagrant up</code></br>
This action runs vagrant
</br>
</br>
Vagrant will download our custom box and boot it in VirtualBox. When the files have been downloaded, we can login.
</br>
<code>vagrant ssh</code></br></br>
I'm in!

![image](https://github.com/nobudlamini/archivematica_exploration/assets/150668386/e7cc9788-386d-4bb2-8252-438af8048c11)
</br>
</br>
I can now access this Archivematica instance through the web browser </br>
http://10.10.10.20/
</br>
</br>
![image](https://github.com/nobudlamini/archivematica_exploration/assets/150668386/42fa9567-a095-4f57-a237-5956430e9fd2)
</br>
</br>
And I can connect to the storage device in the virtual machine
http://10.10.10.20:8000/
</br>
</br>
![image](https://github.com/nobudlamini/archivematica_exploration/assets/150668386/29669c08-522f-41e2-80ff-7195fe8aa440)
</br>
</br>
<b> User Management Portal </b>
![image](https://github.com/nobudlamini/archivematica_exploration/assets/150668386/19cc97cd-d7e5-4a6e-8dcc-a3c80cdf88fe)
</br>
</br>
<b>Uploading Data to Storage Facility</b>
</br></br>
From the Archivematica dashboard, I can browse to any location and select data set to be uploaded to archivematica connected storage
</br>
</br>
![image](https://github.com/nobudlamini/archivematica_exploration/assets/150668386/cb00eead-8015-47db-8e05-79d04fefe701)
</br>
Data uploads can be set to be automated or the micro service can be manually triggered. In this case, once the dataset has been identified I need to click on "Start Transfer" for archivematica to initiate data transfer.
</br></br>
![image](https://github.com/nobudlamini/archivematica_exploration/assets/150668386/b9810254-a360-4693-bd81-828f6ad4301e)
</br>
Before starting transfer, I have the option to examine contents of data set on the microservices on the dashboard
</br></br>
![image](https://github.com/nobudlamini/archivematica_exploration/assets/150668386/651ff87a-ac54-4400-ab54-738afc2a08d2)
</br>
When starting the transfer, archivematica invites me to create the Submission Information Package (SIP) and process the dataset
</br></br>
![image](https://github.com/nobudlamini/archivematica_exploration/assets/150668386/8140a6e4-f688-4842-abbd-889588d89782)
</br></br>
Once we have confirmed the transfer kickstarting, archivematica will move to confirm ingest settings for this specific dataset. Again,this can be defined upfront and set to automate, otherwise for each dataset we can manually double check the micro services settings regarding the normalising settings as well as meta data settings and specification
</br></br>
![image](https://github.com/nobudlamini/archivematica_exploration/assets/150668386/5748df4f-d28c-4fc8-afcd-84fa7d714997)
</br></br>
![image](https://github.com/nobudlamini/archivematica_exploration/assets/150668386/07c5c6f4-1e97-474d-b80d-4ee14f0d33ca)
</br></br>
![image](https://github.com/nobudlamini/archivematica_exploration/assets/150668386/a538c8f4-b2d2-46bd-b4e8-4fcf34cfdafb)






