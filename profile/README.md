<h2 align="center">Multi-Py MultiArchitecture Python Containers</h2>

![](./images/hydra-social.png)

This organization builds Python containers that support multiple architectures. While most python packages support speedy installs with prebuilt wheels, most do not yet build wheels for ARM based architectures. This leaves developers on those systems faced with a choice- use a potentially buggy emulation layer for their containers or wait 20+ minutes while their containers compile those packages.

The containers in this repository all support-

* linux/amd64
* linux/arm64
* linux/arm/v7

New versions are build automatically using Github Actions, with new builds generally starting within 30 minutes of the package being released to PyPI.
