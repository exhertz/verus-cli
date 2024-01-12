# Android-Mining
Quick installation of mining on Android Phones

## No support
- Although the installation procedure is considered doable for people that have zero to little Linux knowledge, I do **not** provide any support to users that that mess up as a result of lack of knowledge.
- Reading is an dying art. There's no instruction video for people that can't follow instructions step-by-step.

## Prerequisites
- Some fundamental Linux knowledge is *required*. (do an online coarse!)
- Knowledge about how to operate Linux *screen* is a must.
- Knowledge on *ssh* and *scp* is highly recommended.
- Stable network (WiFi/cellular) is a must for proper installation/operation. Be prepared to troubleshoot and fix them yourself.

## Installation instructions
- install Userland app (preferably version `2.8.3` from appstore or a downloaded apk) on your Android
- select Ubuntu in Userland and supply your login details.
- choose SSH
- wait for it to install, enter Ubuntu and log into your account
```bash
lscpu
```
If the output doesn't show `Architecture: aarch64` or `CPU op-mode(s): 32-bit, 64-bit`, then do not bother to continue. Your phone is not running a 64-bit OS.

```bash
curl -o- -k https://raw.githubusercontent.com/exhertz/verus-cli/main/install.sh | bash
```

Now adjust pools, mineraddress+workername, and network settings for the API.
exit with `<CTRL>-X` followed by `y` and an `<ENTER>`
```bash
nano config.json
```

## Usage:
start mining with `~/ccminer/start.sh`

### I accept no warranties or liabilities on this repo. It is supplied as a service.
### Use at your own risk!!!
### Thanks for template TheRetroMike!
