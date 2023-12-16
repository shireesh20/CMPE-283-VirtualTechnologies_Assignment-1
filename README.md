# CMPE-283-Virtual Technologies_Assignment-1

Assignment 1: Discovering VMX Features

Student names: Upasana Kumar , Shireesh Vennamaneni

University Name: San Jose State University

Prerequisites:-
You require a machine that supports Linux and has VMX virtualization features available. Depending on your hardware and software setup, it might be possible to run this within a virtual machine, but this is not guaranteed.

Assignment Details:-
We reviewed the Intel SDM supplied by our professor and attended the lecture related to this assignment.
Our goal is to identify specific features on our GCP VM.

Demo Screenshots

1.Pinbased (provided by professor Mike as codebase)

<img width="644" alt="image" src="https://github.com/upasanakr/CMPE-283-VirtualTechnologies_Assignment-1/assets/144417727/a5b8fdc2-0bcb-428b-a2ba-eb209090e9e0">

2.Primary ProcBased Controls

<img width="719" alt="image" src="https://github.com/upasanakr/CMPE-283-VirtualTechnologies_Assignment-1/assets/144417727/d2f79b38-e127-41b6-aec6-730f7b9d528c">


3.Secondary ProcBased Controls

<img width="719" alt="image" src="https://github.com/upasanakr/CMPE-283-VirtualTechnologies_Assignment-1/assets/144417727/4dfe6364-2c7a-42bb-96bc-de12954585e5">



4.Exit Controls

<img width="719" alt="image" src="https://github.com/upasanakr/CMPE-283-VirtualTechnologies_Assignment-1/assets/144417727/cd7238e5-587f-4757-a9b5-569d4adc997d">


5.Entry Controls and Tertiary

<img width="719" alt="image" src="https://github.com/upasanakr/CMPE-283-VirtualTechnologies_Assignment-1/assets/144417727/fb9bdf3f-2d00-4768-9886-f3674f8b45d9">





Questions:-
1. For each member in your team, provide 1 paragraph detailing what parts of the lab that member
implemented / researched.

Shireesh was responsible for configuring the Google Cloud Platform virtual machine, ensuring the correct settings for nested virtualization were enabled, a foundational step for the project. After setting up the environment, he created a dedicated project directory and proceeded to download the essential cmpe283-1.c source file and Makefile from Canvas. He tackled the implementation of primary and secondary MSR controls within the cmpe283.c file. This task required careful adherence to the professor's instructional video and a deep understanding of the Intel SDM volume 3 documentation. His work was critical in laying the groundwork for the kernel module development, ensuring the initial codebase was robust and well-structured.

Upasana focused on the latter stages of the assignment, building upon the groundwork established by Shireesh. Her primary responsibility was to enhance the kernel module by adding functionality for querying exit, entry, and tertiary-based MSR controls. This task required a comprehensive understanding of the Intel SDM volume 3 and the ability to interpret and apply complex technical guidelines into practical code, as detailed in the professor's video lecture. She  managed the compilation process, resulting in the creation of .o and .ko files, and played a key role in testing the module through the use of insmod and rmmod tools. Used the dmesg command to review system log messages, was crucial in verifying the successful implementation and functionality of the kernel module.



2. Describe in detail the steps you used to complete the assignment.




