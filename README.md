
PhpStorm Protocol handler for Windows
---
This code allows to use ```phpstorm://``` protocol to open a file in a [PhpStorm](http://www.jetbrains.com/phpstorm/).

One of the following links must be specified as an editor in your app:

```bash
phpstorm://open?url=file://%f&line=%l

phpstorm://open?file=%f&line=%l
```

If something doesn't work, then feel free to [submit an issue](https://github.com/pniaps/PhpStormProtocol/issues/new) on GitHub.


Installing
---
1. clone this repository in the folder ```C:\Program Files\PhpStorm Protocol (Win)```
```bash
git clone https://github.com/Makedit/PhpStormProtocolWin.git "C:\Program Files\PhpStorm Protocol (Win)"
```
2. double click on ```C:\Program Files\PhpStorm Protocol (Win)\install.reg``` file and agree to whatever Registry Editor asks you
3. by default **PhpStorm** has to be installed in ```C:\Program Files\JetBrains\PhpStorm``` on Windows x64. If you use 32 bits version or another folder, update settings at ```C:\Program Files\PhpStorm Protocol (Win)\run_phpstorm.js```
4. if you use [Xdebug](https://xdebug.org/), set the following line on php.ini ```xdebug.file_link_format = "phpstorm://open?file=%f&line=%l"```