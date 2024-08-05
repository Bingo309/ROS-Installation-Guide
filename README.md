# ROS Installation Guide using VirtualBox and Ubuntu 20.04


1. Open VirtualBox and click on "New".
   
![image](https://github.com/user-attachments/assets/7cbaa029-3418-4048-90b6-79e0b44d3511)

3. set OS "Linux" and the version as "Ubuntu (64-bit)".
   
![image](https://github.com/user-attachments/assets/52939439-b27b-47f3-af81-b7695233d27d)

5. Set the memory size (RAM). 
   
![image](https://github.com/user-attachments/assets/ba8d1c7b-469c-4b28-8ba0-040b7ee9f47a)

7. Set the size of the virtual hard disk.
   
![image](https://github.com/user-attachments/assets/108636af-fbae-4c11-a4c7-4e7736a70857)

9. After Creating it , we first define the ISO file.
    
![image](https://github.com/user-attachments/assets/02212dfa-0773-491a-bf29-5926d0ff128d)

![image](https://github.com/user-attachments/assets/c5bf255d-7d37-44f4-b395-be350a534580)

![image](https://github.com/user-attachments/assets/4429058f-83dc-4fe2-adb3-9aa071e0a3a8)

![image](https://github.com/user-attachments/assets/16f830ea-a734-4353-bb46-721d02145531)



11. we open a terminal window and Add the ROS repository to your system:
    ```bash
    sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
    ```

    ![1](https://github.com/user-attachments/assets/f5f1bcff-59ee-4769-a977-2815ff83f76a)




3. Add the ROS key:
    ```bash
    curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
    sudo apt install curl
    ```
    
    ![image](https://github.com/user-attachments/assets/468124df-710e-4ef7-9dd0-de271ff81291)



4. Update the package list:
    ```bash
    sudo apt update
    ```
    
    ![image](https://github.com/user-attachments/assets/f73de8f8-4500-469a-954f-c367db4ce0c4)


5. then afterwards we Install the full version of ROS (Noetic) and Set up the ROS environment:
  
    ```bash
    sudo apt install ros-noetic-desktop-full
    ```
    
    ```bash
    echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
    source ~/.bashrc
    ```
    then finally the ros version will be displayed , as a confirmation for successful installation.
   
   ![5](https://github.com/user-attachments/assets/a3720f84-95e7-4d60-96e7-5f6dc821f764)












   






