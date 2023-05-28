# Windows11-for-unsupported-cpus

Create Windows 11 installation media

On the Windows 11 software download page, select Create tool now and follow the instructions to install Windows 11.

Warning: 

Microsoft recommends against installing Windows 11 on a device that does not meet the Windows 11 minimum system requirements. 

If you choose to install Windows 11 on a device that does not meet these requirements, and you acknowledge and understand the risks, 
you can create the following registry key values and bypass the check for TPM 2.0 (at least TPM 1.2 is required) and the CPU family and model.

Registry Key: HKEY_LOCAL_MACHINE\SYSTEM\Setup\MoSetup

Name: AllowUpgradesWithUnsupportedTPMOrCPU

Type: REG_DWORD

Value: 1

Note: Serious problems might occur if you modify the registry incorrectly by using Registry Editor or by using another method. These problems might require that you reinstall the operating system. Microsoft cannot guarantee that these problems can be solved. Modify the registry at your own risk.

There are two installation paths available:

Upgrade by launching Setup on the media while running Windows 10. You will have the option to: 

a. Perform a Full Upgrade, which keeps personal files (including drivers), apps, and Windows Settings. This is the default experience and is the one that Installation Assistant uses.

b. Keep Data Only will keep personal files (including drivers) only, not apps and not Windows Settings.
 
c. Clean Install will install Windows 11 and keep nothing from the Windows 10 installation. For more info, see Give your PC a Fresh Start.

Boot from media to launch Setup. This path is a clean install and will not retain previous files or settings. For more info, see Give your PC a Fresh Start.

Important: You should verify that your device meets minimum system requirements before you choose to boot from media, because it will allow you to install Windows 11 if you have at least TPM 1.2 (instead of the minimum system requirement of TPM 2.0), and it will not verify that your processor is on the approved CPU list based on family and model of processor.