# Run the Playbook
ansible-playbook playbook.yaml

##### ansible-playbook playbook.yaml command every 15 minutes using crontab in Linux, you can follow these steps:

1. Open the crontab editor by typing the following command in your terminal:

##### crontab -e

2. If this is your first time using crontab, you may be prompted to select a default text editor.

3. Once the editor opens, add the following line to the file:

#####  */15 * * * * ansible-playbook /opt/playbook.yaml

This line tells crontab to run the ansible-playbook command every 15 minutes. Make sure to replace /path/to/playbook.yaml with the actual path to your playbook file.

4. Save and close the file.

The */15 * * * * syntax means that the command will be executed every 15 minutes. The five asterisks correspond to the minute, hour, day of the month, month, and day of the week fields, respectively. The asterisk in each field means that the command will be executed for all values of that field.
