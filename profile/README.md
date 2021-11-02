<h2 align="center">Multi-Py: MultiArchitecture Python Containers</h2>

![](https://raw.githubusercontent.com/multi-py/.github/main/profile/images/hydra-social.png)

This organization builds Python containers that support multiple architectures. While most python packages support speedy installs with prebuilt wheels, many do not yet build wheels for ARM based architectures- and even fewer are built with musl libc, the C Library used in Alpine. This leaves developers on those systems faced with a choice- use a potentially buggy emulation layer for their containers or wait 20+ minutes while their containers compile those packages. The containers in this organization provide another option.


<center>
<h2>Multi Architecture Builds</h2>
</center>

The containers in this project attempt to support these architectures-

All containers in this organization support `amd64` and `arm64`, and most of them also support `arm v7`.

<center>
<h2>Small Images via Multi Stage Builds</h2>
</center>

All libraries are compiled in one image before being moved into the final published image. This keeps all of the build tools out of the published container layers.


<center>
<h2>No Rate Limits</h2>
</center>

This project uses the Github Container Registry to store images, which have no rate limiting on pulls (unlike Docker Hub).


<center>
<h2>Rapid Building of New Versions</h2>
</center>

Within 30 minutes of a new release to the upstream project on PyPI builds will kick off for new containers. This means new versions can be used in hours, not days.


<center>
<h2>Regular Updates</h2>
</center>

Containers are rebuilt weekly in order to take on the security patches from upstream containers.

