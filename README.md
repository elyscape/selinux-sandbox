# selinux-sandbox
A Docker environment for writing SELinux policy modules.

You can use this image as a sandbox for writing SELinux policy modules. To use it, simply launch a shell with it:

    $ docker run -it elyscape/selinux-sandbox

It is a good idea to mount a local directory to work in so that, when you leave the container, you still have access to any policy modules that you may have written or compiled:

    $ docker run -it -v ~/selinux-policies:/selinux-policies elyscape/selinux-sandbox
