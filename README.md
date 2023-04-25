# Power-Automate-Send-Files-to-Sharepoint
Send Files to Automatically to Sharepoint via Power Automate Desktop

This workflow basically shows a way to send new files that are being saved in a server 'On-premise' to a Sharepoint Folder.
In this case, the files were generated daily and sent after 'order by' DESC as Most Recent File.

In this picture, the flow works by a manually trigger but you just need to set a schedule of your preference i.e. Hourly, Daily, Weekly, Monthly, for example.

Workflow understanding:
Steps
1) Set a variable 1 with the folder path desired (in this case, 'On-premise' server folder).
2) Get archives in folder (generates a list of items that were ingested before in the folder path) This step generated the variable 'Files'.
3) Set a variable 2 wich contains the first item of the list 'Files' as 'Files[0]'.
4) Content data inside the File[0] is converted to binary.
5) A new file is created with the desired name and placed in a Sharepoint Folder.

Images
Image 1 - Complete Workflow;
Image 2 - Step2 Config;
Image 3 - Step3 Config;
Image 4 - Step4 Config;


![image](https://user-images.githubusercontent.com/98396618/234409767-36bd88f8-ae1c-49ef-af1f-fd4dc494dcbd.png)

![image](https://user-images.githubusercontent.com/98396618/234411104-77ed8b9e-9b76-465f-a8ed-fe1307b346c0.png)

![image](https://user-images.githubusercontent.com/98396618/234411283-27f575ab-f7f3-4fd9-8f0e-f4ca50c5bc50.png)

![image](https://user-images.githubusercontent.com/98396618/234411421-e9406603-a3d2-4cb0-ae8e-50ef13fd9602.png)
