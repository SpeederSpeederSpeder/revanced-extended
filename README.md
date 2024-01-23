## ReVanced eXtended
[![CI](https://github.com/AbakNacchan/revanced-extended/actions/workflows/ci.yml/badge.svg?event=schedule)](https://github.com/AbakNacchan/revanced-extended/actions/workflows/ci.yml)

### Extensive ReVanced eXtended Builder

※ Get the [latest CI release](https://github.com/MatadorProBr/revanced-extended-magisk-module/releases) ※

Use [**zygisk-detach**](https://github.com/j-hc/zygisk-detach) to detach YouTube and YouTube Music from Play Store if you are using Magisk modules. 

<details><summary><big>Features</big></summary>
<ul>
 <li>Support all present and future ReVanced eXtended apps</li>
 <li>Can build Magisk modules and non-root APKs</li>
 <li>Updated periodically with the latest versions of apps and patches</li>
 <li>Optimize APKs and modules for size</li>
 <li>Modules</li>
    <ul>
     <li>recompile invalidated odex for faster usage</li>
     <li>receive updates from Magisk app</li>
     <li>do not break safetynet or trigger root detections</li>
     <li>handle installation of the correct version of the stock app and all that</li>
     <li>support Magisk and KernelSU</li>
    </ul>
</ul>
Note that the <a href="../../actions/workflows/ci.yml">CI workflow</a> is scheduled to build the modules and APKs everyday using GitHub Actions if there is a change in ReVanced patches. You may want to disable it.
</details>

## To include/exclude patches or patch other apps
[**See the list of patches**](https://j-hc.github.io/rvmm-config-gen/)

 * Star the repo
 * [Fork the repo](https://github.com/AbakNacchan/revanced-extended/fork) or use it as a template
 * Customize [`config.toml`](./config.toml) using [rvmm-config-gen](https://j-hc.github.io/rvmm-config-gen/)
 * Run the build [workflow](../../actions/workflows/build.yml)
 * Grab your modules and APKs from [releases](../../releases)

Also see [`CONFIG.md`](./CONFIG.md).

## Building Locally
### On Termux
```console
bash <(curl -sSf https://raw.githubusercontent.com/AbakNacchan/revanced-extended/main/build-termux.sh)
```

### On Desktop
```console
$ git clone https://github.com/AbakNacchan/revanced-extended
$ cd revanced-extended
$ ./build.sh
```
