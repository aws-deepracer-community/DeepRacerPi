# Introducing the PiRacer: A Budget-Friendly Compute Module Replacement for AWS DeepRacer

The **PiRacer** is a custom-designed PCB that serves as a cost-effective replacement for the original AWS DeepRacer compute module. With a production and assembly cost of just **$33**, the PiRacer brings the power of the **Raspberry Pi Compute Module 4 (CM4)** and the upcoming **Compute Module 5 (CM5)** to your DIY racing projects.

<img src="Images/PiRacer.jpg" alt="PiRacer PCB" width="50%">

## What You Need
To get started with the PiRacer, you’ll need:
1. **Raspberry Pi CM4 Lite**: The brain of the operation.
2. **SD Card**: For booting and storing your project data.
3. **PiCamera V2**: For capturing the track and enabling autonomous driving.

---

The PiRacer empowers makers and students to build, modify, and innovate with their AWS DeepRacer cars. it is a small enough package to fit into 1/28th scale car significantly reducing the footprint needed for AWS DeepRacer.




## TODO for PiRacer Development

1. **Implement Battery Monitor**  
   - Add circuitry and software support to monitor battery voltage and health.
   - Display battery status in real-time for improved usability.

2. **Fix USB OTG Support**  
   - Modify USB configuration to enable OTG (On-The-Go) functionality.
   - Ensure compatibility with peripherals and reliable data transfer.
3. **Add Tail light LED**
   - Implement multicolor Tail light indicator
4. **Add Fan header**
   - Enable FAN for additional cooling support
5. **Add UART via serial connector headers**
   - to enable additional debugging


## Setting Up the board

1. **Image SD card with  Ubuntu 22.04**
   - use win+shift+x to enable SSH and Wifi during imaging process
   - Edit /boot/firmware/config.txt
     - Add dtparam=i2c_arm=on
     - Add Start_x=1
     - Add dtoverlay=vc4-fkms-v3d
2. Follow these instructions
   - https://github.com/aws-deepracer-community/deepracer-custom-car

Special Thanks for Lars for all the work he did on the Deepracer-custom-car repo to make this a possibility!



