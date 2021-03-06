# docker-images

Docker images for fun and for profit, mostly meant to be used in GitLab CI or Drone CI jobs.

* **`ubuntu16.04-gcc5.3.1-openmpi1.10-mkl2017.4.239`**: install GCC 5.3.1, OpenMPI 1.10 and MKL 2017.4.239 on top of Ubuntu 16.04
  Currently used for testing [LSDALTON](https://gitlab.com/dalton/lsdalton)
* **`ubuntu18.04-gcc7.3.0-openmpi2.1.0-mkl2017.4.239`**: install Python3, GCC 7.3.0, OpenMPI 2.1.0 and MKL 2017.4.239 on top of Ubuntu 18.04
* **`ubuntu16.04-pgi17.4`**: install PGI 17.4 CE on top of Ubuntu 16.04
  Currently used for testing [LSDALTON](https://gitlab.com/dalton/lsdalton)
* **`ubuntu16.04-intel2018.1`**: install Intel 2018.1 on top of Ubuntu 16.04.
* **`cmake-cookbook_ubuntu16.04-intel2018.1`**: install Intel 2018.1 on top of Ubuntu 16.04.
  Currently used for testing [CMake Cookbook](https://github.com/dev-cafe/cmake-cookbook)
* **`cmake-cookbook_ubuntu16.04-pgi17.4`**: install PGI 17.4 on top of Ubuntu 16.04.
  Currently used for testing [CMake Cookbook](https://github.com/dev-cafe/cmake-cookbook)

## DockerHub

The container images are automatically built on `DockerHub` at https://hub.docker.com/u/devcafe/
`DockerHub` does not allow dashes in user and organization names. It's **devcafe**, not **dev-cafe**!

For example you can download the `ubuntu16.04-pgi17.4` container locally with:

    docker pull devcafe/ubuntu16.04-pgi17.4

Then get a shell inside the container with

    docker run -it devcafe/ubuntu16.04-pgi17.4 /bin/bash
