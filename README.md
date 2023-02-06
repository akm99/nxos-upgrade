ansible version = 2.7.9
python version = 2.6.6

This playbook is designed to do code upgrade on nxos switch, using the following tasks(catered to nxos.9.3.9 and some dependent SMUs/EPLD).

Here are the general tasks that have been used to create the playbooks.

Stage 0:

Check version on the box. 

Stage 1:

Check available space on the box for new files to be stored. 

Stage 2:

Push all the files needed for upgrade to the box. 

Stage 3:

Collect pre-check data before device isolation pre-upgrade

Stage 4:

Upgrade OS/install 2xSMUs and Verify

Stage 5:

Upgrade EPLD and Verify 

Stage 6:

Collect post-check data after putting the device back to service post-upgrade 

Stage 7:

Compare pre-check and post-check data 

