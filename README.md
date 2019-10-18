# edgetpu-bin

**https://github.com/google-coral/edgetpu#build-and-install-from-source**

```bash
$ cd ~
$ git clone https://github.com/google-coral/edgetpu.git
$ cd edgetpu

$ mkdir -p bin
$ export PATH=$PATH:$HOME/bin
$ curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
$ chmod a+x ~/bin/repo

$ git config --global user.name "Your Name"
$ git config --global user.email "you@example.com"

$ repo init -u https://coral.googlesource.com/manifest -b release-day
$ repo sync -j$(nproc)

$ scripts/runtime/install.sh
$ scripts/build_swig.sh
$ make wheel
```

The wheel file is generated in the following path.  
**`~/edgetpu/dist/edgetpu-2.12.1-py3-none-any.whl`**
