## voron_configs

### Setup

```
# clone repo to home directory 
cd ~
git clone git@github.com:jrhorner1/voron_configs.git 
cd ~/voron_configs 
confdir=~/printer_data/config/
for conf in $(find ./ -maxdepth 1 -regextype posix-extended -regex ".*(d|cfg)"); do
  ln -s $conf $confdir
done
```

