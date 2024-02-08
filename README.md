# vps2devuan

> Install Devuan GNU/Linux on your VPS, no matter what the current OS is.

## Usage

1. Install make and git with your current package manager

2. Run this script

```
$ curl -OL https://raw.githubusercontent.com/SekaiMoe/vps2devuan/main/vps2devuan
$ chmod +x ./vps2devuan
$ sudo ./vps2devuan #[OPTIONS]
```

3. Sync data and reboot

```
$ sudo $SHELL -c 'sync && reboot -f'
```

4. Connect to server after about 3 minutes.

```
# the root password from the original system (or by using vps2suse as password if no root password was set).
$ ssh root@your-server-ip
```

5. Change your root password

```
passwd
```

### Options

```
-h Show help messages.
-s Set OS version, For example "-s stable" (Default: cares).
-c Set architecture type for the container image (Default: auto detect).
-m Set mirror address (Default: https://deb.devuan.org/merged).
```

## Credits

This project is based on [vps2arch](https://github.com/drizzt/vps2arch)

## License

GNU General Public License 3.0
