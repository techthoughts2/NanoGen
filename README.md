# NanoGen
GUI driven PowerShell script that enables you to quickly create Nano images

## Synopsis

NanoGen\NanoGen.Run.ps1 - GUI driven PowerShell script that enables you to quickly create Nano images.

## Description

NanoGen is a GUI wrapper for assisting with the rapid creation of a Nano Server images using the New-NanoServerImage cmdlet.

The GUI options presented assist with properly formulating the New-NanoServerImage command with the correct syntax.

This project was undertaken prior to Microsoft releasing the **Nano Server Image generation tool** (https://blogs.technet.microsoft.com/nanoserver/2016/10/15/introducing-the-nano-server-image-builder/)

The **Nano Server Image generation tool** accomplishes the same thing as NanoGen (correctly building a Nano Server Image with New-NanoServerImage cmdlet)

Usage of this tool is no longer recommended in favor of the **Nano Server Image generation tool** but NanoGen can still provide a great deal of insight into how these tools work and how to manually create a Nano Server Image.

## Prerequisites

* NanoGen\NanoGen.Run.ps1
* Running Server 2016 or Windows 10 (the ADK specific to these OS's is engaged to properly adjust the Nano Server Image)
* The 2016 Server Media ISO (preview edition or ISO from MSDN)

## How to run

NanoGen\NanoGen.Run.ps1

**NanoGen\NanoGen.Run.ps1**
 1. Copy code from NanoGen.Run.ps1 into Administrator ISE window
 2. Click Play
 3. On main GUI screen specify the location of the Nano Media
  * The nano media location should be a folder that contains the \NanoServer folder that is retrieved from the Windows Server 2016 ISO. Do not link directly to the NanoServer folder.
  * If you do not have a copy of the Nano Media readily available you will need to secure a trial edition or a copy of the ISO media from a MSDN download or other 2016 Server media
 4. Complete the Nano Image Configuration section to your desired specifications
 5. Click the **Create Nano Image** button which will load the necessary Nano Image creation command into your clipboard
 6. Close NanoGen by clicking the X button the GUI
 7. Paste the Nano Image creation command into an Administrator ISE Window
 8. Wait for the command to complete and finish creating your image.
  * Images are created at the Destination Path that you specify and are always called Nano.vhdx (or Nano.vhd if creating a Gen1 image)
  
### Contributors

Authors: Jake Morrison

Contributors: 

### Notes

Usage of this tool is no longer recommended in favor of the **Nano Server Image generation tool** but NanoGen can still provide a great deal of insight into how these tools work and how to manually create a Nano Server Image.