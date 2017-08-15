## Configuring the Touchpad in Windows 10 ##

  1. Download the Dell (Synaptics) Touchpad Driver for the Dell N7010
     - It uses a superior method of TouchCheck which allows moving the mouse while typing.
     - It has a usable configuration utility.
     
  2. Extract the archive and use the `Have Disk...` selector to choose the driver files.
  3. Use `gpedit.msc` to navigate to `Local Computer Policy` -> `Computer Configuration` -> `Administrative Templates` -> `System` -> `Device Installation` -> `Device Installation Restrictions`.
     - Enable the policy entitled `Prevent installation of devices that match any of these device IDs`
     - Add the following Device ID to the list: `ACPI\VEN_SYN&DEV_0A19`
  4. Navigate to `Scrolling` in the `Touchpad Settings`
     - Enable Reverse Scrolling
  5. Navigate to `Pointing` -> `Sensitivity` -> `TouchCheck`
     - Set the slider to `Maximum`
  6. Navigate to `Pointing` -> `Sensitivity` -> `Touch Sensitivity`
     - Set the slider to `Light Touch`
