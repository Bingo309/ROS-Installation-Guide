# ROS Installation Guide using VirtualBox and Ubuntu 20.04


1. Open VirtualBox and click on "New".
   
![image](https://github.com/user-attachments/assets/a3838365-014f-4f4c-8d93-6ab635cc7241)

3. set OS "Linux" and the version as "Ubuntu (64-bit)".
   
![image](https://github.com/user-attachments/assets/2289122b-09f4-4aa7-9af9-2f884057fcb8)

5. Set the memory size (RAM). 
   
![image](https://github.com/user-attachments/assets/179c6442-3206-4ee6-9458-0f9590abef80)

7. Set the size of the virtual hard disk.
   
![image](https://github.com/user-attachments/assets/2fa29269-aeaf-4db6-a843-bdc74dfa6eea)

9. After Creating it , we first define the ISO file.
    
![image](https://github.com/user-attachments/assets/bc1476be-55ab-4332-8810-e71769e30ef8)

![image](https://github.com/user-attachments/assets/5a0e3612-9ad2-46d0-a725-51b9b68fe703)

![image](https://github.com/user-attachments/assets/8d10dcd3-0e3f-4af3-9665-87f8021162ca)

![image](https://github.com/user-attachments/assets/5b6c8022-bdab-42f8-a966-070f10d8c925)



11. we open a terminal window and Add the ROS repository to your system:
    ```bash
    sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
    ```

    ![1](https://github.com/user-attachments/assets/7369f815-7b5d-42ae-a224-ac83dfae915e)


3. Add the ROS key:
    ```bash
    curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
    sudo apt install curl
    ```
    
   ![image](https://github.com/user-attachments/assets/355ccd74-ba0c-445b-a7f5-04f94b0dd1d2)

   ![image](https://github.com/user-attachments/assets/3681ad7f-68fb-40c2-b5d3-9e4d3e3726a9)



5. Update the package list:
    ```bash
    sudo apt update
    ```
    ![image](https://github.com/user-attachments/assets/8cc0edc8-10f2-42dc-9a98-df27b3da3ddb)



6. then afterwards we Install the full version of ROS (Noetic) and Set up the ROS environment:
  
    ```bash
    sudo apt install ros-noetic-desktop-full
    ```
    
    ```bash
    echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
    source ~/.bashrc
    ```
    then finally the ros version will be displayed , as a confirmation for successful installation.
   
    ![5](https://github.com/user-attachments/assets/cfd26278-941a-4637-8ebd-08c51c9db113)













   






