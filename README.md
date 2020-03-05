# macOS mkjail
### This project is no longer maintained.
Script to automatically prepare a functional chroot jail with the following utilities:

| Utility | Priority | Type | Depends |
|:----|:---:|:---:|:----|
| [bash](https://www.gnu.org/s/bash) | Required | Self-compiled | none |
| [coreutils](https://www.gnu.org/software/coreutils/coreutils.html) | Required | Self-compiled | none |
| [inetutils](https://www.gnu.org/software/inetutils/) | Required\* | Self-compiled | none |
| [grep](https://www.gnu.org/software/grep/) | Extra | Self-compiled | none |
| [less](https://www.gnu.org/software/less/) | Extra | Self-compiled | none |
| [make](https://www.gnu.org/s/make) | Extra | Self-compiled | none |
| [nano](https://www.nano-editor.org) | Extra | Self-compiled | none |
| [gzip](https://www.gnu.org/software/gzip/) | Extra | Self-compiled | none |
| [zsh](http://zsh.sourceforge.net) | Extra | Self-compiled | none |
| [tar](https://www.gnu.org/software/tar/) | Extra | Self-compiled | none |
| [binutils](https://www.gnu.org/software/binutils/) | Extra | Self-compiled | none |
| [xz-utils](https://tukaani.org/xz/) | Extra | Self-compiled | none |
| [bzip2](https://web.archive.org/web/20180801004107/http://www.bzip.org) | Extra | Pre-compiled | none |
| [bashpm](https://github.com/pixelomer/bashpm) | Not recommended, not maintained | Bash Script | curl, xz-utils, tar, grep |
| [curl (no SSL support)](https://curl.haxx.se) | Recommended | Pre-compiled | CoreFoundation\*\* |

\*: The script will continue even if this utility isn't compiled properly  
\*\*: A preinstalled framework in macOS, copied by the script inside the jail.  

**Tested on:** macOS High Sierra (10.13.6), macOS Mojave (10.14)  
  
[Original gist](https://gist.github.com/pixelomer/f29eedb34368bec62df545c05db706b4)
