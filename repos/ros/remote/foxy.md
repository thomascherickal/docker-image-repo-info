## `ros:foxy`

```console
$ docker pull ros@sha256:735755cd2793b4b4a357abeccdb5f3ee4a6dfce80213dc0c5c1481dc3aa58111
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:foxy` - linux; amd64

```console
$ docker pull ros@sha256:3bec0a335f38070c59e676455829c13951973be3d02326c794e0d6dd2bd0f83e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.9 MB (250922479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4438fb9a5d55786fd05b32d73437c087f915d8564aa7edcf12667f4f1323ec6f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:45:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:39:48 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:51:44 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Wed, 01 Feb 2023 20:51:46 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 01 Feb 2023 20:51:46 GMT
ENV LANG=C.UTF-8
# Wed, 01 Feb 2023 20:51:46 GMT
ENV LC_ALL=C.UTF-8
# Wed, 01 Feb 2023 20:51:46 GMT
ENV ROS_DISTRO=foxy
# Wed, 01 Feb 2023 20:52:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:52:50 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Wed, 01 Feb 2023 20:52:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 01 Feb 2023 20:52:50 GMT
CMD ["bash"]
# Wed, 01 Feb 2023 20:53:13 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 20:53:18 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 01 Feb 2023 20:53:23 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Wed, 01 Feb 2023 20:53:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db143da9f5a088b47cfbe87905f9e615f3b537f906257fc11ac7a38ffb0f236c`  
		Last Modified: Wed, 01 Feb 2023 18:58:42 GMT  
		Size: 1.2 MB (1154526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f52bb4834a5fa25fa5b39cba579b1676bc6fc585a61819ffad44865e1f80e40`  
		Last Modified: Wed, 01 Feb 2023 20:55:33 GMT  
		Size: 5.6 MB (5553686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f105b35b0dfc6028b74d92fda44d6d2c3af732aca846352b68466fa262457ea`  
		Last Modified: Wed, 01 Feb 2023 20:58:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1da6af1c9709b569597a5ba230c17042bc010f9750727f5c8758e5b1772139b`  
		Last Modified: Wed, 01 Feb 2023 20:58:08 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4390ba395fc8695bc2fa5c6b394cd5d5646325ef60302c849898873530f6d9b1`  
		Last Modified: Wed, 01 Feb 2023 20:58:29 GMT  
		Size: 120.4 MB (120357173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c508771ef6bc75da73349529405df86553b5351d4963f8b9a0f9b0bd39b568a`  
		Last Modified: Wed, 01 Feb 2023 20:58:08 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04699b3e750a87a1ac026108652f71ed30dbd1658b8992675307ee50b00d13bc`  
		Last Modified: Wed, 01 Feb 2023 20:58:47 GMT  
		Size: 73.3 MB (73334255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60655459143d2e28fcf98e47908a7e7521455039a65dffdcde118686599dc91`  
		Last Modified: Wed, 01 Feb 2023 20:58:37 GMT  
		Size: 277.8 KB (277775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ea369debb9602b8c58eb54bc2ae097a85dca159d27e70505ae0b6dbfb73e22`  
		Last Modified: Wed, 01 Feb 2023 20:58:37 GMT  
		Size: 2.4 KB (2426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c16f94d4b42426319c336c992c2ae0a9420d2cda68e8de9c663e7544512d8d`  
		Last Modified: Wed, 01 Feb 2023 20:58:40 GMT  
		Size: 21.7 MB (21662340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:foxy` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:934c9283e3d48098dadf95c77a79a88ea4c5e9a0f271bede8e7fc154b93f9e97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.8 MB (226802496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:797fdf269cafa9a646733093d1d3d343908984b5908fe293f93ad246f522f787`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 05:24:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:24:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:24:53 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:24:55 GMT
ADD file:110968e7ce1c893bcdf7597ece624ff881de3e1ee2c4e2b70dbc18c9a5271fc0 in / 
# Wed, 01 Mar 2023 05:24:55 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 03:29:39 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:29:53 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:43:36 GMT
RUN echo "deb http://packages.ros.org/ros2/ubuntu focal main" > /etc/apt/sources.list.d/ros2-latest.list
# Thu, 02 Mar 2023 03:43:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Mar 2023 03:43:37 GMT
ENV ROS_DISTRO=foxy
# Thu, 02 Mar 2023 03:44:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-core=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:31 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 02 Mar 2023 03:44:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Mar 2023 03:44:31 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 03:44:52 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     git     python3-colcon-common-extensions     python3-colcon-mixin     python3-rosdep     python3-vcstool     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 03:44:56 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Thu, 02 Mar 2023 03:45:01 GMT
RUN colcon mixin add default       https://raw.githubusercontent.com/colcon/colcon-mixin-repository/master/index.yaml &&     colcon mixin update &&     colcon metadata add default       https://raw.githubusercontent.com/colcon/colcon-metadata-repository/master/index.yaml &&     colcon metadata update
# Thu, 02 Mar 2023 03:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-foxy-ros-base=0.9.2-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:970e18d4d6e7e6f413a168be4dd550847bf3c325f54e7c69a5ad6435dfd1fe48`  
		Last Modified: Wed, 01 Mar 2023 10:21:59 GMT  
		Size: 27.2 MB (27194521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68cba7bfabf687405ca086cd0f7c2dd41598d503e63af5d7a5ee49931ff4befd`  
		Last Modified: Thu, 02 Mar 2023 04:06:42 GMT  
		Size: 1.2 MB (1154531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bd306c6e57df2c972eff933b6975a0d34abf4ab4e726b76eb90bbcca4dfeb4`  
		Last Modified: Thu, 02 Mar 2023 04:06:41 GMT  
		Size: 5.5 MB (5531909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424a1659f1c90f60434c50265969a97cd41a22913c2037483ff3bd9792717987`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a73223e5ee62173a4b294378545321fee65e69698550366cccd744cdda7fa2`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cd7e465b25c7c0b51fa71a0769a0d8ee12c963a8760da60297aaaf481d33d8`  
		Last Modified: Thu, 02 Mar 2023 04:09:07 GMT  
		Size: 104.6 MB (104569036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bd83378013cccd76320c75fb5937199f996eb144292044c9dfcb1419089d8d`  
		Last Modified: Thu, 02 Mar 2023 04:08:55 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0208396681856b3ee322e06ae0454a98f416931c3b6e27c348fe4923edeefefd`  
		Last Modified: Thu, 02 Mar 2023 04:09:23 GMT  
		Size: 67.7 MB (67683638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd600f7c98c5fbacb990bfb6221305e0b939a4a8850b0681d70ce3b97870e8e`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 279.2 KB (279217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea21264705160c5780c3c14d6050afbc00c6b2de0b190944cbe9c6bad84ec3a`  
		Last Modified: Thu, 02 Mar 2023 04:09:16 GMT  
		Size: 2.4 KB (2413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f1e1e57ea67c116aa79df7407e788e1060cedbd46bd14461fa7c06a434bd2b`  
		Last Modified: Thu, 02 Mar 2023 04:09:18 GMT  
		Size: 20.4 MB (20384821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
