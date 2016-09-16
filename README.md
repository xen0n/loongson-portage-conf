# Portage configuration for Loongson

## Supported configuration

* Loongson 3A2000
    - GNOME 3 + systemd

Recommended overlays:

* `gentoo-zh`
* `gnome`
* `qt`
* `x11`

You can install them with `layman`.


## Usage

```sh
emerge git
git clone https://github.com/xen0n/loongson-portage-conf.git somewhere

# 使用所有配置，执行下面的指令
# for using entirety of configuration
cd /etc
mv portage portage.bak
ln -s /path/to/somewhere/3a2000 portage
cp make.site.conf.example make.site.conf
vim make.site.conf  # edit to your liking

# 您也可以只取用需要的部分
# or you can symlink only the parts you're interested in
```


<!-- vim:set ai et ts=4 sw=4 sts=4 fenc=utf-8: -->
