H4K3ROM
===========

Getting Started
---------------

Install [Git and Repo](http://source.android.com/source/using-repo.html).

To initialize your local repo copy of H4K3ROM, use:

```bash
repo init --depth=1 -u git://github.com/H4K3ROM/android.git -b 18.1
```
Then to sync up:
```bash
repo sync --force-sync --no-tags --no-clone-bundle
```
Building
$ repo sync --force-sync --no-clone-bundle --no-tags -j$(nproc --all) && . build/envsetup.sh && brunch bonito

***Quoted from LineageOS Wiki***
```
Turn on caching to speed up build
Make use of ccache if you want to speed up subsequent builds by running:

export USE_CCACHE=1
export CCACHE_EXEC=/usr/bin/ccache
and adding that line to your ~/.bashrc file. Then, specify the maximum amount of disk space you want ccache to use by typing this:

ccache -M 50G
where 50G corresponds to 50GB of cache. This needs to be run once. Anywhere from 25GB-100GB will result in very noticeably increased build speeds (for instance, a typical 1hr build time can be reduced to 20min). If you’re only building for one device, 25GB-50GB is fine. If you plan to build for several devices that do not share the same kernel source, aim for 75GB-100GB. This space will be permanently occupied on your drive, so take this into consideration.

You can also enable the optional ccache compression. While this may involve a slight performance slowdown, it increases the number of files that fit in the cache. To enable it, run:

ccache -o compression=true
```
***Quoted from LineageOS Wiki***

***Install as per instructions for Bonito from LineageOS Wiki***

[https://wiki.lineageos.org/devices/bonito/install] 


I break things and void warranties for fun. All aside, this is just a loose custom spin of LineageOS with some added bells & whistles. I am a one-man h3k4r with limited time to update repos, build custom apps, etc. So the key here is to slowly build my own "custom user build" of Lineage for my personal needs. If they suit yours, then we both win ;)

Continual W.I.P

Sincerely,
Floyd Flivercod III
