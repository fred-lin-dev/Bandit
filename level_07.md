# 2025-10-23

I start with ls but there's nothing except:
bash_logout, bashrc, profile

then:
cd ..

so I'm on the root of the server and I tried find command:

bandit6@bandit:/home$ find -size 33c
./bandit15/.bandit14.password
find: ‘./drifter6/data’: Permission denied
./bandit18/readme
./bandit3/inhere/...Hiding-From-You
./bandit21/.prevpass
./bandit2/--spaces in this filename--
find: ‘./leviathan4/.trash’: Permission denied
./bandit25/.bandit24.password
./bandit1/-
./drifter0/chroot/drifter0.password
./bandit16/.bandit15.password
find: ‘./drifter8/chroot’: Permission denied
./bandit4/inhere/-file03
./bandit4/inhere/-file02
./bandit4/inhere/-file07
./bandit4/inhere/-file00
./bandit4/inhere/-file04
./bandit4/inhere/-file09
./bandit4/inhere/-file05
./bandit4/inhere/-file08
./bandit4/inhere/-file06
./bandit4/inhere/-file01
find: ‘./bandit30-git’: Permission denied
find: ‘./bandit29-git’: Permission denied
find: ‘./bandit28-git’: Permission denied
find: ‘./ubuntu’: Permission denied
./bandit17/.bandit16.password
find: ‘./leviathan0/.backup’: Permission denied
find: ‘./bandit27-git’: Permission denied
find: ‘./bandit5/inhere’: Permission denied
find: ‘./bandit31-git’: Permission denied

bandit6@bandit:/home$ find -user bandit7
find: ‘./drifter6/data’: Permission denied
find: ‘./leviathan4/.trash’: Permission denied
find: ‘./drifter8/chroot’: Permission denied
find: ‘./bandit30-git’: Permission denied
find: ‘./bandit29-git’: Permission denied
find: ‘./bandit28-git’: Permission denied
find: ‘./ubuntu’: Permission denied
find: ‘./leviathan0/.backup’: Permission denied
find: ‘./bandit27-git’: Permission denied
find: ‘./bandit5/inhere’: Permission denied
find: ‘./bandit31-git’: Permission denied
bandit6@bandit:/home$

bandit6@bandit:/home$ find -group bandit6
find: ‘./drifter6/data’: Permission denied
find: ‘./leviathan4/.trash’: Permission denied
find: ‘./drifter8/chroot’: Permission denied
find: ‘./bandit30-git’: Permission denied
find: ‘./bandit29-git’: Permission denied
find: ‘./bandit28-git’: Permission denied
find: ‘./ubuntu’: Permission denied
find: ‘./leviathan0/.backup’: Permission denied
find: ‘./bandit27-git’: Permission denied
find: ‘./bandit5/inhere’: Permission denied
find: ‘./bandit31-git’: Permission denied
bandit6@bandit:/home$

bandit6@bandit:/home$ find -user bandit7 -group bandit6 -size 33c
find: ‘./drifter6/data’: Permission denied
find: ‘./leviathan4/.trash’: Permission denied
find: ‘./drifter8/chroot’: Permission denied
find: ‘./bandit30-git’: Permission denied
find: ‘./bandit29-git’: Permission denied
find: ‘./bandit28-git’: Permission denied
find: ‘./ubuntu’: Permission denied
find: ‘./leviathan0/.backup’: Permission denied
find: ‘./bandit27-git’: Permission denied
find: ‘./bandit5/inhere’: Permission denied
find: ‘./bandit31-git’: Permission denied
bandit6@bandit:/home$

bandit6@bandit:/$ ls
behemoth           etc         lib64              media   run                 tmp
bin                formulaone  lib.usr-is-merged  mnt     sbin                usr
bin.usr-is-merged  home        libx32             narnia  sbin.usr-is-merged  utumno
boot               krypton     lost+found         opt     snap                var
dev                lib         manpage            proc    srv                 vortex
drifter            lib32       maze               root    sys
bandit6@bandit:/$ find -user bandit7 -group bandit6 -size 33c
find: ‘./tmp’: Permission denied
find: ‘./etc/credstore.encrypted’: Permission denied
find: ‘./etc/sudoers.d’: Permission denied
find: ‘./etc/stunnel’: Permission denied
find: ‘./etc/multipath’: Permission denied
find: ‘./etc/ssl/private’: Permission denied
find: ‘./etc/polkit-1/rules.d’: Permission denied
find: ‘./etc/credstore’: Permission denied
find: ‘./etc/xinetd.d’: Permission denied
find: ‘./dev/mqueue’: Permission denied
find: ‘./dev/shm’: Permission denied
find: ‘./snap’: Permission denied
find: ‘./lost+found’: Permission denied
find: ‘./run/pam_pidns’: Permission denied
find: ‘./run/udisks2’: Permission denied
find: ‘./run/chrony’: Permission denied
find: ‘./run/user/15006’: Permission denied
find: ‘./run/user/15005’: Permission denied
find: ‘./run/user/15004’: Permission denied
find: ‘./run/user/15003’: Permission denied
find: ‘./run/user/15002’: Permission denied
find: ‘./run/user/15001’: Permission denied
find: ‘./run/user/15000’: Permission denied
find: ‘./run/user/12001’: Permission denied
find: ‘./run/user/11003’: Permission denied
find: ‘./run/user/11022’: Permission denied
find: ‘./run/user/14002’: Permission denied
find: ‘./run/user/11019’: Permission denied
find: ‘./run/user/11014’: Permission denied
find: ‘./run/user/11021’: Permission denied
find: ‘./run/user/8001’: Permission denied
find: ‘./run/user/12002’: Permission denied
find: ‘./run/user/11025’: Permission denied
find: ‘./run/user/11032’: Permission denied
find: ‘./run/user/11013’: Permission denied
find: ‘./run/user/11008’: Permission denied
find: ‘./run/user/8006’: Permission denied
find: ‘./run/user/11007’: Permission denied
find: ‘./run/user/11009’: Permission denied
find: ‘./run/user/11024’: Permission denied
find: ‘./run/user/11006/systemd/inaccessible/dir’: Permission denied
find: ‘./run/user/11023’: Permission denied
find: ‘./run/user/11002’: Permission denied
find: ‘./run/user/11001’: Permission denied
find: ‘./run/user/11005’: Permission denied
find: ‘./run/user/11016’: Permission denied
find: ‘./run/user/11011’: Permission denied
find: ‘./run/user/11004’: Permission denied
find: ‘./run/user/11012’: Permission denied
find: ‘./run/user/11000’: Permission denied
find: ‘./run/sudo’: Permission denied
find: ‘./run/screen/S-bandit20’: Permission denied
find: ‘./run/multipath’: Permission denied
find: ‘./run/cryptsetup’: Permission denied
find: ‘./run/lvm’: Permission denied
find: ‘./run/systemd/propagate/fwupd.service’: Permission denied
find: ‘./run/systemd/propagate/ModemManager.service’: Permission denied
find: ‘./run/systemd/propagate/polkit.service’: Permission denied
find: ‘./run/systemd/propagate/chrony.service’: Permission denied
find: ‘./run/systemd/propagate/systemd-logind.service’: Permission denied
find: ‘./run/systemd/propagate/irqbalance.service’: Permission denied
find: ‘./run/systemd/propagate/systemd-networkd.service’: Permission denied
find: ‘./run/systemd/propagate/systemd-resolved.service’: Permission denied
find: ‘./run/systemd/propagate/systemd-udevd.service’: Permission denied
find: ‘./run/systemd/inaccessible/dir’: Permission denied
find: ‘./run/lock/lvm’: Permission denied
find: ‘./home/drifter6/data’: Permission denied
find: ‘./home/leviathan4/.trash’: Permission denied
find: ‘./home/drifter8/chroot’: Permission denied
find: ‘./home/bandit30-git’: Permission denied
find: ‘./home/bandit29-git’: Permission denied
find: ‘./home/bandit28-git’: Permission denied
find: ‘./home/ubuntu’: Permission denied
find: ‘./home/leviathan0/.backup’: Permission denied
find: ‘./home/bandit27-git’: Permission denied
find: ‘./home/bandit5/inhere’: Permission denied
find: ‘./home/bandit31-git’: Permission denied
find: ‘./proc/tty/driver’: Permission denied
find: ‘./proc/1/task/1/fd’: Permission denied
find: ‘./proc/1/task/1/fdinfo’: Permission denied
find: ‘./proc/1/task/1/ns’: Permission denied
find: ‘./proc/1/fd’: Permission denied
find: ‘./proc/1/map_files’: Permission denied
find: ‘./proc/1/fdinfo’: Permission denied
find: ‘./proc/1/ns’: Permission denied
find: ‘./proc/2/task/2/fd’: Permission denied
find: ‘./proc/2/task/2/fdinfo’: Permission denied
find: ‘./proc/2/task/2/ns’: Permission denied
find: ‘./proc/2/fd’: Permission denied
find: ‘./proc/2/map_files’: Permission denied
find: ‘./proc/2/fdinfo’: Permission denied
find: ‘./proc/2/ns’: Permission denied
find: ‘./proc/187/task/187/fd/6’: No such file or directory
find: ‘./proc/187/task/187/fdinfo/6’: No such file or directory
find: ‘./proc/187/fd/5’: No such file or directory
find: ‘./proc/187/fdinfo/5’: No such file or directory
find: ‘./manpage/manpage3-pw’: Permission denied
find: ‘./var/crash’: Permission denied
find: ‘./var/tmp’: Permission denied
find: ‘./var/log’: Permission denied
find: ‘./var/lib/apt/lists/partial’: Permission denied
find: ‘./var/lib/ubuntu-advantage/apt-esm/var/lib/apt/lists/partial’: Permission denied
find: ‘./var/lib/amazon’: Permission denied
./var/lib/dpkg/info/bandit7.password
find: ‘./var/lib/udisks2’: Permission denied
find: ‘./var/lib/snapd/void’: Permission denied
find: ‘./var/lib/snapd/cookie’: Permission denied
find: ‘./var/lib/polkit-1’: Permission denied
find: ‘./var/lib/private’: Permission denied
find: ‘./var/lib/chrony’: Permission denied
find: ‘./var/lib/update-notifier/package-data-downloads/partial’: Permission denied
find: ‘./var/spool/bandit24’: Permission denied
find: ‘./var/spool/cron/crontabs’: Permission denied
find: ‘./var/spool/rsyslog’: Permission denied
find: ‘./var/cache/apt/archives/partial’: Permission denied
find: ‘./var/cache/private’: Permission denied
find: ‘./var/cache/pollinate’: Permission denied
find: ‘./var/cache/apparmor/70b6ca72.0’: Permission denied
find: ‘./var/cache/ldconfig’: Permission denied
find: ‘./root’: Permission denied
find: ‘./boot/efi’: Permission denied
find: ‘./boot/lost+found’: Permission denied
find: ‘./drifter/drifter14_src/axTLS’: Permission denied
find: ‘./sys/kernel/tracing/osnoise’: Permission denied
find: ‘./sys/kernel/tracing/hwlat_detector’: Permission denied
find: ‘./sys/kernel/tracing/instances’: Permission denied
find: ‘./sys/kernel/tracing/trace_stat’: Permission denied
find: ‘./sys/kernel/tracing/per_cpu’: Permission denied
find: ‘./sys/kernel/tracing/options’: Permission denied
find: ‘./sys/kernel/tracing/rv’: Permission denied
find: ‘./sys/kernel/debug’: Permission denied
find: ‘./sys/fs/pstore’: Permission denied
find: ‘./sys/fs/bpf’: Permission denied
bandit6@bandit:/$

et ici j'avais commencer à perdre espoir car je ne savais plus quoi faire ici.
j'ai donc demandé à claude un indice et il m'a dit que c'était dans le texte que je venais de lui envoyer.
il m'a dit de faire une redirection vers /dev/null
Donc la commande qui permet de le résoudre et 

find -user bandit7 -group bandit6 -size 33c 2> /dev/null

cd ./var/lib/dpkg/info/

cat bandit7.password

# 2026-06-27

I did exactly the same mistake, forgot to redirect to /dev/null

cat ./var/lib/dpkg/info/bandit7.password

