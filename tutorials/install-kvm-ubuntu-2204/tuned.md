
. Optimize the Host with TuneD

sudo systemctl enable --now tuned

tuned-adm active

tuned-adm list

sudo tuned-adm profile virtual-host

sudo tuned-adm verify


Verification failed, current system settings differ from the preset profile.
You can mostly fix this by restarting the Tuned daemon, e.g.:
  systemctl restart tuned
or
  service tuned restart
Sometimes (if some plugins like bootloader are used) a reboot may be required.
See tuned log file ('/var/log/tuned/tuned.log') for details.


sudo reboot

But tuned is problematic

tuned-adm off


## Install Tuned

https://github.com/redhat-performance/tuned

