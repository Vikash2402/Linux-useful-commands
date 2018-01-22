# Linux-useful-commands

1. Trassfer file/files from one machine to another
pscp -r currentMAchinePAth username@localIp:destination path

pscp -r D:\ABC\XYZ\CDF vikash2402@172.0.0.10:/home/vikash2402/project/xyz


2. get  into a root environment 
sudo su


3. check running dockers
docker ps

4. get inside a container shell

docker exec -t -i container_name /bin/bash

docker exec -t -i my_container /bin/bash


5. using docker - host to container vice versa file sharing

docker cp sourcepath continerName:path

docker cp /home/vikash2402/xyz  my_container:/app/xyz/


docker cp foo.txt my_container:/foo.txt

docker cp my_container:/foo.txt foo.txt


6. Find a File
find / -name abcd.txt

7. get geditor
sudo apt-get install gedit

8. remove all files from including directry
rm -rf mydir

9. install make
sudo apt-get update
sudo apt-get install build-essential

10. install vim

sudo apt-get install vim


3. Insatll unixODBC
https://help.sap.com/viewer/4ed80c6b3a854bf0a3596b18e5ad5cd9/2.0.01/en-US/e783b19c6f0f10149a438f15eda0ba9f.html

4. Install SAP hana client
https://blogs.sap.com/2012/09/14/install-hana-client-on-ubuntu/

6. Test sap hana connection
https://blogs.sap.com/2012/09/14/hana-with-odbc-on-ubuntu-1204/


Command to build docker image – 
Syntax     :  sudo docker build -t <image name> .
Example :  sudo docker build -t abcFile .

Command to run docker image –
                Syntax    :  sudo docker run -p <portnumber>:80 <image name>
                Example : sudo docker run -p 5001:80 abcFile

Please Note:
1.	Package files to be kept in the folder named as publish
2.	Docker file to be present in the same folder where publish folder is kept
3.	Execute the docker commands from the parent folder where publish and docker file is kept



2. Insall chrome-

wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | sudo apt-key add - 
sudo sh -c 'echo "deb https://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google.list'
sudo apt-get update
sudo apt-get install google-chrome-stable

https://askubuntu.com/questions/79280/how-to-install-chrome-browser-properly-via-command-line


