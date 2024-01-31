# archivematica_exploration
Exploration of Archivematica using Virtualisation

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




