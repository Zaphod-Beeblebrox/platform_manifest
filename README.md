This is a modified version of AOKP built specifically for an Rockchip 3188 based automotive head unit
(Newsmy 3001/5002).  There are significant changes to the frameworks that would likely make this unsuitable for any other device.  If you are looking for straight AOKP,  I suggest you go straight to their git hub: https://github.com/AOKP


[Android Open Kang Project](http://aokp.co)
====================================


Download the Source
===================

Please read the [AOSP building instructions](http://source.android.com/source/index.html) before proceeding.

Initializing Repository
-----------------------

Init core trees 

    $ repo init -u https://github.com/Zaphod-Beeblebrox/platform_manifest.git -b kitkat


sync repo :

    $ repo sync

***

Building
--------

After the sync is finished, please read the [instructions from the Android site](http://s.android.com/source/building.html) on how to build.

    . build/envsetup.sh
    brunch


You can also build (and see how long it took) for specific devices like this:

    . build/envsetup.sh
    time brunch aokp_rk3188

Remember to `make clobber` every now and then!
