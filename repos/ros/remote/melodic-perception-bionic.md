## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:c31a22c7464ca36e4f30ecd2e56aae4275613f06ac3d9d5f13d11237259635df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:be4597ce7bc9e89f114baaeb3d9bbfca25d0823264b89bba8493583ebb44b343
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742471468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0abc68b332bea9499a8f5a85bb588fbacb32a320b25ef9d866c1227a98231df9`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:15 GMT
ADD file:7274ece1917848683250bbeda9eacf6eb7510481cbaa177880e3a60b4133e35b in / 
# Tue, 13 Jul 2021 22:29:15 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 22:53:53 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:53:40 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 01:53:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 01:53:43 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 01:57:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:57:45 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 01:57:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 01:57:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:58:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:58:43 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 01:59:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:05:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7ae86ffe2df0787131a4c49ace1b018fd38d62929b007d86bdd1f825e56a852`  
		Last Modified: Tue, 13 Jul 2021 22:31:03 GMT  
		Size: 26.7 MB (26706145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1107129de068a3615596b08dc61d39c6a7722d1f446096ae57c3f28769bfca39`  
		Last Modified: Tue, 13 Jul 2021 23:14:34 GMT  
		Size: 840.8 KB (840788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff77a7fbbce93b678f9a7ec24c63012d604fef4a9cad8414c5b8a467f2930e4d`  
		Last Modified: Wed, 14 Jul 2021 02:29:23 GMT  
		Size: 4.9 MB (4872342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea558154c977de1713b413508635ea067b8a9cb2caac2c2d33399aa134072c7a`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324a009470670a1026f1819627c53fb14edf956e0cc56b9ead79340c9de91ed8`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d8abfba080c1ed4e3b4bdc2bf0d8eee89b03d0c97b04d513b964b4b26aa96d`  
		Last Modified: Wed, 14 Jul 2021 02:30:07 GMT  
		Size: 259.4 MB (259436482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b906763856d86a129884f2d128bbc8ba73658b2c439deafb32dc704ad6f8f3d3`  
		Last Modified: Wed, 14 Jul 2021 02:29:22 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51e724da914872a99c21d1c752fe003c146cf3fda351f11997235ba7772cdba`  
		Last Modified: Wed, 14 Jul 2021 02:30:31 GMT  
		Size: 70.2 MB (70229653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a2ee178e82d7a724d90e3a8d8e37e8f09ccb10b47b1b62479653c997cb1df0`  
		Last Modified: Wed, 14 Jul 2021 02:30:20 GMT  
		Size: 269.6 KB (269609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b958a59ce23c95988f3219849b668a9b70003fa348726a8d3f88d1f5281a4715`  
		Last Modified: Wed, 14 Jul 2021 02:30:35 GMT  
		Size: 75.0 MB (74994876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f8ea3cc6e40968b9269ae85659b70394812d64bc9bf7e41a2e48e7bd47924e`  
		Last Modified: Wed, 14 Jul 2021 02:31:58 GMT  
		Size: 305.1 MB (305119158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:531c5b1f694fe9241b487531af0ad04d0630e2a086eaeb6901a88b84e8b2d24c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.8 MB (645753605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb39a9052fc864479baf00515e9f9873ba014f65779d4143cb70654f3f3a713`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:20:43 GMT
ADD file:f065167f188d5bc319e42f0d3fb26520247ed8e38db629af17856b6f9e2f0cf0 in / 
# Tue, 13 Jul 2021 23:20:45 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:49:56 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:13 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:50:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 14 Jul 2021 00:50:18 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LANG=C.UTF-8
# Wed, 14 Jul 2021 00:50:19 GMT
ENV LC_ALL=C.UTF-8
# Wed, 14 Jul 2021 00:50:20 GMT
ENV ROS_DISTRO=melodic
# Wed, 14 Jul 2021 00:53:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:53:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 14 Jul 2021 00:53:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 14 Jul 2021 00:53:30 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 00:54:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:54:39 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 14 Jul 2021 00:55:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 00:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13c5fbe08fe2049e9effbe0d00319cfb1efa5d363e64f222a8bb747a01143fbd`  
		Last Modified: Tue, 13 Jul 2021 23:25:48 GMT  
		Size: 22.3 MB (22304073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42872bf962a1c39ef027f457cefdef3c14b61de5a2e4eb23c3cd86de2ddf9554`  
		Last Modified: Wed, 14 Jul 2021 01:11:43 GMT  
		Size: 841.4 KB (841422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d86d64b6163277a8faa0275b3fcba0855d5af76a2212503e755cba50cb08d4d`  
		Last Modified: Wed, 14 Jul 2021 01:11:42 GMT  
		Size: 4.1 MB (4085737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c8f9089545ebc81b78035f6c8bcc9757f8574fc623e07301fbc6081e76d1ee`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a241e304ad2761062f5ec7258e0a2490ccfb82ee70d01cca739111e2656605a0`  
		Last Modified: Wed, 14 Jul 2021 01:11:39 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6434ded48ed96eaf7f1622cc6d4a0d69212f24911da077bb3e36b45f85e1487`  
		Last Modified: Wed, 14 Jul 2021 01:14:19 GMT  
		Size: 238.9 MB (238929302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193577023dae8fd6d36536414dd47eb98a483fdcf9d56fb523ac3cd9b4b80f06`  
		Last Modified: Wed, 14 Jul 2021 01:11:40 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bf1f931a8a0bada54ddb1868696700aed914f2205fcf2d217323a06a12897c`  
		Last Modified: Wed, 14 Jul 2021 01:15:03 GMT  
		Size: 54.7 MB (54695702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dc768f3e4222fe29a227fe190b7dff33b4c25fc8c8423d81dc83f47634fbb3`  
		Last Modified: Wed, 14 Jul 2021 01:14:33 GMT  
		Size: 269.7 KB (269680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e632e952bcaf0807284b647dec165289d61395139d9d50307f600e4ae928d0b`  
		Last Modified: Wed, 14 Jul 2021 01:15:19 GMT  
		Size: 64.7 MB (64746099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4700cd0e55ec4689d10f8da0b292b3b58a8f52b07d10b0ff28072467263a9c39`  
		Last Modified: Wed, 14 Jul 2021 01:18:51 GMT  
		Size: 259.9 MB (259879173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:06a8877d06ee3d43cae4db4115f77c90941979182204247a10666a157dd51dfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.4 MB (703408937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa83fb8faa0ed8cf731122e6195d0bbc27cf22642b27c7c9bb5d2d32bdeea1f2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:49 GMT
ADD file:e87e065765ef99e8db25307f469c7481ab480ac5fe6353ae4caf402766f14045 in / 
# Mon, 26 Jul 2021 21:48:50 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:58:27 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:58:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Mon, 26 Jul 2021 22:58:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LANG=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV LC_ALL=C.UTF-8
# Mon, 26 Jul 2021 22:58:38 GMT
ENV ROS_DISTRO=melodic
# Mon, 26 Jul 2021 22:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:59:55 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Mon, 26 Jul 2021 22:59:55 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 26 Jul 2021 22:59:55 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:00:23 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:00:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 26 Jul 2021 23:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:03:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fda1cca7a3cc2b66c161597f27e151a9b1cab79d73c7c0c2706606813a3e58cf`  
		Last Modified: Mon, 26 Jul 2021 21:50:37 GMT  
		Size: 23.7 MB (23731597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec48fab32c57250a0a316617993b1f19f17f7e3eb1f5b4b632c9e249bb8be37`  
		Last Modified: Mon, 26 Jul 2021 23:17:30 GMT  
		Size: 841.3 KB (841297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cda3a4d02e2669921c5de51d652aabfb73f4df2b82620e22cee0613358f560c`  
		Last Modified: Mon, 26 Jul 2021 23:17:28 GMT  
		Size: 4.5 MB (4453714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc312c19bce6f60c0e01ada675f9b439a2c4e6e65fdc361f6d9dfa88a88968`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f078b2e134b3bbc567abf387a039e07d7e9b62a44937b65e4486b11a93d0fa`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bb5e0dcebd403b1631077c2bf6f918a579e8261929dd592e97c3599825d707`  
		Last Modified: Mon, 26 Jul 2021 23:18:13 GMT  
		Size: 252.4 MB (252370080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262db146cf4cceac59a83a88e61705c701c9d85f669bade5fb3551c8f1cee8e3`  
		Last Modified: Mon, 26 Jul 2021 23:17:27 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab725edf1b9f4a135356a05ee3965e94a8d870362463cfa1fdd8b121ae62082`  
		Last Modified: Mon, 26 Jul 2021 23:18:36 GMT  
		Size: 63.1 MB (63058039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7c0963f89fcec01a24152c167c502a6ea1d71b33c04b6c7446ca5c665813a4`  
		Last Modified: Mon, 26 Jul 2021 23:18:25 GMT  
		Size: 270.4 KB (270436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44737e66a0fd9299314b82210b7ef1b09c9ec7087b11e374538c570a10ef4e62`  
		Last Modified: Mon, 26 Jul 2021 23:18:39 GMT  
		Size: 67.2 MB (67222081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11602763d81471ccb881ff943ad79df93f3f835646e285b1b1c71a97c4cceb8`  
		Last Modified: Mon, 26 Jul 2021 23:20:05 GMT  
		Size: 291.5 MB (291459283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
