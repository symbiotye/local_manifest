LOCAL_MANIFEST
========================
CM-14.1 for MSM8916 Family

### Installing Repo ###
```bash
# Make a directory where Repo will be stored and add it to the path
    $ mkdir ~/.bin
    $ PATH=~/.bin:$PATH

# Download Repo itself
    $ curl https://storage.googleapis.com/git-repo-downloads/repo > ~/.bin/repo

# Make Repo executable
    $ chmod a+x ~/.bin/repo
```

### Initializing Repo ###
```bash
    $ repo init -u https://github.com/CyanogenMod/android.git -b cm-14.1
    $ curl --create-dirs -L -o .repo/local_manifests/cm-14.1.xml -O -L https://raw.githubusercontent.com/MSM8916/local_manifest/master/cm-14.1.xml
```
### For sync: ###
```bash
    $ repo sync -j4
```
### To build for your device.. ###
```bash
    $ . build/envsetup.sh
    $ breakfast device_name_here
    $ mka bacon
```



