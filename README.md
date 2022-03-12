# Grub-Rescue-Solution

* Select the right partitoning after checking one by one: `ls`

* set the boot location: `set prefix=(hd1,gpt6)/boot/grub`

* set the root location: `set root=(hd1,gpt6)`

* Initiate the normal mode: `insmod normal`

* Go to normal mode: `normal`


> In the terminal Window of your Linux Machine

* `grub-install /dev/sda `

* To save the new changes: `update-grub `


# How-To-Remove-Grub-or-Delete-Grub-Permanently

`diskpart`

`list disk`

`sel disk 0`

`list vol`

`sel vol 2`

`assign letter=G:`


> To remove the letter again (Execute After executing the below statements): `remove letter=G: `         

`exit`

`cd /d G:`

`ls`

`ls EFI`

`cd EFI`

`ls`

`rmdir /S kali`

`ls`
