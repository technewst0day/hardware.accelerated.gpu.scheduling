# hardware accelerated gpu scheduling

[![hardware accelerated gpu scheduling](gett-stateed.png)](https://computersolve.com/hardware-accelerated-gpu-scheduling/)

Usually, your computer’s processor offloads some visual and graphics-intensive data to the GPU to render so that games, multimedia, and other apps run smoothly. The CPU gathers the frame data, assigns commands, and prioritizes them one by one so that the GPU can render the frame.

With the Hardware-Accelerated GPU Scheduling feature, the GPU’s scheduling processor and memory (VRAM) takes over the same work and runs it in batches to render the frames. In that way, your GPU relieves the processor from some work and reduces latency to potentially make your PC run better.

## What is Hardware Accelerated GPU Scheduling?

Now, as it happens, the Windows Display Driver Model, also known as WDDM, is a scheduler for the GPU that manages the processes or the tasks that require using your GPU. Your GPU is essentially responsible for rendering, but it is the CPU that sends those tasks to the GPU which are then managed by WDDM. 

One way of making this process more efficient would be to send the tasks that require a GPU in batches instead of sending them one by one. However, this comes at its own cost which is input latency. This is apparent from the fact that a task will not be able to use the GPU unless it is sent in a batch by the CPU. 

As it turns out, the Hardware Accelerated GPU Scheduling feature, introduced by Microsoft, takes the high priority tasks, that would normally be managed by your CPU, and sends them to a dedicated GPU-based scheduler. Doing this takes some of the load off of the CPU which allows your CPU to execute more tasks. This will potentially help in making your PC run faster or perform better. 

## Should you Enable Hardware Accelerated GPU Scheduling? 

With all of that said, the main question is should you enable the said feature? In case you have a low-end or even a mid-tier PC, the feature is worth giving a shot. It can be especially helpful when your CPU is at 100% usage when you are playing games or something similar. 

In case the feature is not available for you, there are other ways using which you can speed up your PC. Naturally, the end decision of whether you should turn on the feature or not is yours. We would recommend testing it with a few games to see if it gets you a positive result. In case it does, keep it enabled. Otherwise, you can always disable it pretty easily.

## Requirements for Hardware-Accelerated GPU Scheduling

As we have mentioned, the Hardware Accelerated GPU Scheduling feature was introduced in May of 2020 by Microsoft. As such, you require a fairly decent PC in order to use the feature. Let us have a look at the requirements down below:

For Windows, you need to be running at least version 2004 or later in order to be able to use the feature. 
When it comes to your GPU, if you are using an NVIDIA graphics card, you will be needing at least something from the 1000 series or later. As for AMD, you will want to have something from the 5600 series or later. In addition to that, make sure that your display drivers are up to date. 

## Enable Hardware Accelerated GPU Scheduling using Windows Registry

If you are more of a tech-savvy type, you can also choose to enable the said feature using the Windows Registry. As it happens, Windows Registry is essentially responsible for how your operating system functions. Therefore, we would recommend creating a backup of the Windows Registry before proceeding. With that done, follow the instructions down below:


* To start off, open up the Run dialog box by pressing the Windows key + R on your keyboard.
* In the Run dialog box, type in regedit and then hit Enter.
* After that, in the address bar of the Windows Registry, copy and paste the following path: 
* Alternatively, you can also navigate to the specified location manually.
* On the right hand side, double click on the HwSchMode key provided.
* Set the value to 2 and make sure Base is set to Hexadecimal.
* Click OK and then go ahead and restart your computer. 
* In case you want to disable the feature in future, simply change the value from 2 to 1.
