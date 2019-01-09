ansible-playbook -i hosts/HOST -e 'mode=install' deliverables.yaml --user alanjm --ask-pass --ask-become-pass

ansible-playbook -c local -i hosts/HOST -e 'mode=uninstall' deliverables.yaml --ask-become-pass
ansible-playbook -c local -i hosts/HOST -e 'mode=install' deliverables.yaml --ask-become-pass