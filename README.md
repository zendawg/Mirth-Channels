Mirth-Channels
==============

Contains channels for use with Mirth ESB. Use the `OpenEyes-Install-Scripts` repository to manage files in this project.

Note that the channels here are in pre-processed format; that is, the files are named `.xml.in`. These contain variables and values that need to be matched up with an existing installation. Install scripts are used to pre-process these scripts in to `.xml` format, which are then deployed to a Mirth instance. Since the files require pre-processing, that also means that in order to check the files back in again, they then need to be reverted from `.xml` files (once exported from the Mirth instance) back in to `.xml.in` files. This can be achieved using the install scripts.

To transform `.xml.in` files to `.xml` files (to 'pre-process' them):

	sh esb/mirth/mirth-install.sh -p

... and to transform them back ('revert') from `.xml` files to `.xml.in`:

	sh esb/mirth/mirth-install.sh -r
