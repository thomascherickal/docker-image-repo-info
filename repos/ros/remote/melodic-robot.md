## `ros:melodic-robot`

```console
$ docker pull ros@sha256:29177934cada73859021580c05d99fc4e0fd0d9c3d9208aeefb3ed987756ab59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot` - linux; amd64

```console
$ docker pull ros@sha256:ad2b0f62192244a09c899d3eb2db7c3e9ee256af2a1b3eb1dd00802f60b2f343
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.6 MB (448598867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e419202b9af9cd0dca24ceebce291a6026b258cd5ff89c8df101d4b0b1bbf32`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:42 GMT
ADD file:0eb7f0555d03ff4f0755bba2c3d133e68737888f41390c17710f64b70c8e662a in / 
# Tue, 02 Aug 2022 01:30:42 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:57:32 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:57:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 12:57:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 02 Aug 2022 12:57:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 02 Aug 2022 12:57:48 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 12:57:48 GMT
ENV LC_ALL=C.UTF-8
# Tue, 02 Aug 2022 12:57:48 GMT
ENV ROS_DISTRO=melodic
# Tue, 02 Aug 2022 13:01:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:01:53 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 02 Aug 2022 13:01:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 02 Aug 2022 13:01:53 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:02:40 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:02:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 02 Aug 2022 13:04:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:04:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c5ef60a68e3fa0bd8df52f48470e836e823434a3bead43e35e87098a0b01fa`  
		Last Modified: Mon, 01 Aug 2022 16:03:08 GMT  
		Size: 26.7 MB (26710270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa6fbe30fbafa2fd890f1a634056fab84382d475fe85716949a1a44cc77f087`  
		Last Modified: Tue, 02 Aug 2022 13:52:33 GMT  
		Size: 839.1 KB (839126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7d6485ffdcfd34d9790c5e9f1e3deb6f1e01cd88b3ed1c2c4bfd798ce679c6`  
		Last Modified: Tue, 02 Aug 2022 13:52:31 GMT  
		Size: 4.9 MB (4873542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37d651da90ea517b4e41ab1754a0657cd17842014153817571fad7f62a21dd8`  
		Last Modified: Tue, 02 Aug 2022 13:52:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8310f03235adb2a56f2ca99fcd6f4bf9c29d94663f625b160ef3534ffc2630bc`  
		Last Modified: Tue, 02 Aug 2022 13:52:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f613727d0890c231f392123401bfc2194872d710cd8d8a8740db383fc8a599f4`  
		Last Modified: Tue, 02 Aug 2022 13:53:17 GMT  
		Size: 259.6 MB (259551224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ab03995e2e9bff9b259a370e6c30525ec9bc8cb87b98f29e3d3de46a99b36e`  
		Last Modified: Tue, 02 Aug 2022 13:52:30 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0b7f91cbaa1e44e2ecae278c9b9bcec5d83eb8397cfd098ce9f394ca3642d2`  
		Last Modified: Tue, 02 Aug 2022 13:53:39 GMT  
		Size: 70.3 MB (70259542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e26ed31df7e549f55f79f7b17b78d0ba6d56d1cf0cd9a4f352729bc4be37f67`  
		Last Modified: Tue, 02 Aug 2022 13:53:27 GMT  
		Size: 283.1 KB (283134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99508511f69fc265efef3003c1bd53483ecc3d71f1bf6cdb319a64a2946042b0`  
		Last Modified: Tue, 02 Aug 2022 13:53:43 GMT  
		Size: 75.0 MB (74994419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eed61fe44d161864b1f15921748fdd6a0e864e30298dfb574cdf474b54b7691`  
		Last Modified: Tue, 02 Aug 2022 13:53:58 GMT  
		Size: 11.1 MB (11085765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:7f4b7e824e2c2d884a5fb5a2c9b781342f4cf8aa705a8a43780f57b072fceb77
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.1 MB (396120708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d09ce3f49835d2c880946babd1f27d25bd83fed4169ab6f73ef3ed6972266945`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:38:47 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:39:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 03 Aug 2022 22:39:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LANG=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV LC_ALL=C.UTF-8
# Wed, 03 Aug 2022 22:39:35 GMT
ENV ROS_DISTRO=melodic
# Wed, 03 Aug 2022 22:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:42:42 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Wed, 03 Aug 2022 22:42:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 03 Aug 2022 22:42:42 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 22:43:50 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:44:00 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 03 Aug 2022 22:46:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 22:47:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad475a95b77752b25dc36bec810d7cc2000f86bc50ea57592b8f988605fc4c6`  
		Last Modified: Wed, 03 Aug 2022 23:06:53 GMT  
		Size: 840.0 KB (839977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d76a2f1b035d0df7e2f785a3199e9e86fdeeda1c9f6087f594f2d8a42f0cfb`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 4.1 MB (4087975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acdc23d18c079581f3391d042b65fd7ae55d75333914fd8cdcd0b8acdd6bf10`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3a86db6f1e409fa1d0b2018d788c0539b214c365337f886b86db7e860ee482`  
		Last Modified: Wed, 03 Aug 2022 23:06:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79c58cc0918adb02a33e27d7ad4e74c5e0463844a26e99fb60557c3594324b5`  
		Last Modified: Wed, 03 Aug 2022 23:07:34 GMT  
		Size: 239.0 MB (239014439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094e568816932729edf86ebafaaeb847af8bda6ade01fb926c6a121f6b825974`  
		Last Modified: Wed, 03 Aug 2022 23:06:50 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23d14b221e943bfa66059662f80e5ae90e6e1f053ed424ca6b2a40c15876113`  
		Last Modified: Wed, 03 Aug 2022 23:07:57 GMT  
		Size: 54.7 MB (54720659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:537d299c243ea0c73b05e8b607aa42ec071f847fbfa98d9ab5463a6594a04406`  
		Last Modified: Wed, 03 Aug 2022 23:07:46 GMT  
		Size: 283.1 KB (283112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d03bb1219b316469e8bd9f059ea35bbe07e5c60596349c1a2f46c2230f51e2`  
		Last Modified: Wed, 03 Aug 2022 23:08:02 GMT  
		Size: 64.7 MB (64743513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a494ed3d310625a6aa0f4889bc59e46085f1933560b3cf30b478de3be02dae6`  
		Last Modified: Wed, 03 Aug 2022 23:08:20 GMT  
		Size: 10.1 MB (10123573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:3e6c59936fec78be28a82061db3e9537d38de8be5cc48b3206ab80d6d2b88e57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.5 MB (422454040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5e19c4cf364dd50aa1b03a9be7ab0b56d5590c1f90619f74a262d39596aede6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 15:03:25 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 15:03:35 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 15:03:36 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 02 Aug 2022 15:03:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 02 Aug 2022 15:03:39 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 15:03:40 GMT
ENV LC_ALL=C.UTF-8
# Tue, 02 Aug 2022 15:03:41 GMT
ENV ROS_DISTRO=melodic
# Tue, 02 Aug 2022 15:05:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 15:05:05 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 02 Aug 2022 15:05:07 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 02 Aug 2022 15:05:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 15:05:33 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 15:05:40 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 02 Aug 2022 15:06:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 15:06:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87c7d887e7b961ba6c9db72dd6419c5ac455dd43d49b194dbc43680f849a6ef`  
		Last Modified: Tue, 02 Aug 2022 15:38:49 GMT  
		Size: 839.8 KB (839769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51fe758bc1275edfa803da680fe43894a9e4bdb69d83153ccca2d60ba34bbee`  
		Last Modified: Tue, 02 Aug 2022 15:38:47 GMT  
		Size: 4.3 MB (4265854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9646eaa84fc50bf88a2bca0599491e795cf8122e6fe16671e23fd8b87804e823`  
		Last Modified: Tue, 02 Aug 2022 15:38:46 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4ce991e1d0bf36ab7c0c7db9323c2cc620b0d96c88f26c619287aee7598666`  
		Last Modified: Tue, 02 Aug 2022 15:38:46 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a101d7b97c7577b747e3cc14cb64c408587e6489c4b2420aad7fa1dbbd8fe189`  
		Last Modified: Tue, 02 Aug 2022 15:39:22 GMT  
		Size: 252.5 MB (252503681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c716f26c3c2a680d90778a974e99dc5d04bf9e4fbd9077cdb619b311ff4f0d24`  
		Last Modified: Tue, 02 Aug 2022 15:38:46 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b66bed859b212ff9f65c306618bc607825b531e9a79843b4d75f5e870b3195`  
		Last Modified: Tue, 02 Aug 2022 15:39:42 GMT  
		Size: 63.1 MB (63088414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee909ec215bcdf8f5cd2e47e3aaf397ef01b2695fd292ea49920505e539f80c9`  
		Last Modified: Tue, 02 Aug 2022 15:39:34 GMT  
		Size: 283.1 KB (283086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884a1a0922cfe088904523812cfa7b3897bc3fc1b7eb0f266e99c75d92662a17`  
		Last Modified: Tue, 02 Aug 2022 15:39:44 GMT  
		Size: 67.0 MB (67000963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1236989f1fcde790f9d9aeda9bfc9ae97a4c7f11b790b4fb3cbd2e6872f13861`  
		Last Modified: Tue, 02 Aug 2022 15:40:05 GMT  
		Size: 10.7 MB (10735758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
