# Adhocs 

### Create Group Admin
ansible app -b -m group -a "name=admin state=present"

### Create User Kitavi & Add ssh Key & Add home folder & Add to group Admin

ansible app -b -m user -a "name=kitavi group=admin createhome=yes generate_ssh_key=yes"