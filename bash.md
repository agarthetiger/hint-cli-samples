# ssh

* `ssh-keygen -o -a 100 -t ed25519 -f ~/.ssh/id_ed25519 -C "<user@host>"` Generate a strong ssh key
* `eval $(ssh-agent -s)` Start the ssh agent
* `ssh-keygen -R <hostname_or_ip>` Remove a host fingerprint from the known hosts 

# curl

* `curl -s "https://pypi.org/pypi/<package_name>>/json" | jq  -r '.releases | keys | .[]' | sort -V` Get all available versions of a package from pypi.org

# jobs

* `nohup command &>> ./output.txt 2>&1 &` Run a job in the background, append output to file, logging stdout and stderr
* `Ctrl z, bg` Suspend foreground process and resume as a background job

# disk

* `diskutil list` List disks for mounting and unmounting on MacOS
* `diskutil unmountDisk disc2` Unmount microSD card from USB adapter
