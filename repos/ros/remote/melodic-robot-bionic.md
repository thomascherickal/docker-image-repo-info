## `ros:melodic-robot-bionic`

```console
$ docker pull ros@sha256:271a1794a33756d165ef0e9575f746f3709230cbe1716110310d706f5fc293a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-robot-bionic` - linux; amd64

```console
$ docker pull ros@sha256:0081d2a47b1008f2f9e6341ec525d9b48ab20218c21f31001fcd583c16763043
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **448.4 MB (448434037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35978ed9f55ca96736d256b081ae740020d7250016a6b4f948c67489cf80fcc3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:23:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:02 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:43:03 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:43:04 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:43:04 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:43:05 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:47:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:47:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:47:29 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:47:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:48:29 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:48:35 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:50:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:50:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da448bd4f8f4db94a9b5039505342a7b53dd81b10fd374d2def1098fb0ac84d1`  
		Last Modified: Fri, 18 Jun 2021 02:24:11 GMT  
		Size: 841.3 KB (841252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cb58c650b055fb67176d207f9fd10ae383daf8d9bc32c1c8645edaaa9e12ad`  
		Last Modified: Fri, 18 Jun 2021 02:24:09 GMT  
		Size: 4.9 MB (4872799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f28e24aa10e6102264c6409a16774cf0a40f28345825ce31c150b0a8c5f983`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4f503114f27f913b940aef53658909f71731db052648f1e5a2beb2efe74c0`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9cdac581f4ca50f0b20691c7055dfeddbee9c41742de717f9343c0d558319`  
		Last Modified: Fri, 18 Jun 2021 02:24:54 GMT  
		Size: 259.4 MB (259446443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73488a07f8b3040e0131faf7b50bb9599c7de3a9bd3f5dc6755a3d41742bce20`  
		Last Modified: Fri, 18 Jun 2021 02:24:08 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e54789afeb24df301ae5930e5d94fb4ec25ff344550c42fc13ffe6a0aed17d`  
		Last Modified: Fri, 18 Jun 2021 02:25:17 GMT  
		Size: 70.2 MB (70230079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74869fd805fbdcd2d5a41cc7c1871bff9efe9adc5ed9d1c2a259d9b43943ff8a`  
		Last Modified: Fri, 18 Jun 2021 02:25:06 GMT  
		Size: 267.5 KB (267540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5804bd4e67a972c78152ba3990c26cd0cd8a9fa1339f959924d78c56702490d9`  
		Last Modified: Fri, 18 Jun 2021 02:25:23 GMT  
		Size: 75.0 MB (74994766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840127939fedea917fa03948266ca553ba4ef961388197b323cd4530d7f9c84`  
		Last Modified: Fri, 18 Jun 2021 02:25:40 GMT  
		Size: 11.1 MB (11078038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:db70c713ff0f444bd61eaa7494f65408d1b86881021c3eb1a30993f3af9f106f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.0 MB (395985787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5eb6b3e314e488b74a6ad6f23b0e6275da7417e2edece0d2b5b1c13fcb0eac6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:56 GMT
ADD file:05900bb0318e36a0bfd913d618842e013d4cfbe1b49a1c593ef41ac8b987667a in / 
# Thu, 17 Jun 2021 23:31:57 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:43:12 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:43:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 30 Jun 2021 02:43:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 02:43:33 GMT
ENV LC_ALL=C.UTF-8
# Wed, 30 Jun 2021 02:43:34 GMT
ENV ROS_DISTRO=melodic
# Wed, 30 Jun 2021 02:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:46:37 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 30 Jun 2021 02:46:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 30 Jun 2021 02:46:38 GMT
CMD ["bash"]
# Wed, 30 Jun 2021 02:47:24 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:47:38 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 30 Jun 2021 02:48:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Jun 2021 02:49:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edc1907184e6c91ef9fe8cb06817f71679e07f89abc1f82ed7805bfa477509ed`  
		Last Modified: Thu, 17 Jun 2021 23:34:39 GMT  
		Size: 22.3 MB (22297601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41db8d0a5243fbdf90e34d0537b9c5c07c644c49a31fd81d3c2f2daf2a21232c`  
		Last Modified: Wed, 30 Jun 2021 03:12:06 GMT  
		Size: 841.4 KB (841351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25982969d47d9b905ebd3319c388ee188d0c69dc085414a1386b3fccb77efdb`  
		Last Modified: Wed, 30 Jun 2021 03:12:05 GMT  
		Size: 4.1 MB (4085722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56cc63820c603e14682d138b460c624af11548adaf61534445e941174fbb0fe`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899495dc34a34f1cd9f2e205d683c84ec0f0fe27d5febe0c7c8abcae5ded6357`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7bbc3397c7c90914f5db06b99959ada1db177f36c85f4d3c87490fd3872ad`  
		Last Modified: Wed, 30 Jun 2021 03:14:44 GMT  
		Size: 238.9 MB (238928391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1371fff7158214726f450b21ee8d22c6b58e0394c0b17e26f39e9a12a7a51e8`  
		Last Modified: Wed, 30 Jun 2021 03:12:03 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b4a35cf169f13b0864de8acce463e86b885316120329ed7874a8f779347f1a`  
		Last Modified: Wed, 30 Jun 2021 03:15:27 GMT  
		Size: 54.7 MB (54695572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50155253e32e95de619787e129ebf3b9ea3c524c22d9e524e1d39a4a4b59477`  
		Last Modified: Wed, 30 Jun 2021 03:14:57 GMT  
		Size: 268.4 KB (268350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d5e90656133aa33cecfcd863772c2d3e232e88372a7b1523aa00b8aec28c16`  
		Last Modified: Wed, 30 Jun 2021 03:15:43 GMT  
		Size: 64.7 MB (64746000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b628a790cd7515455e943c84550f5550c6253f767820dd131edf2466c6e692dd`  
		Last Modified: Wed, 30 Jun 2021 03:16:08 GMT  
		Size: 10.1 MB (10120382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-robot-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:618890bf1c9e1fc589af0b8a37289145940afd6fb689577c9c5d2371e378d2fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422675404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06888b82cccb9c52119dd61bfae8915ef668145808e717c5c703d1e3222ae36`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:12:23 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Jun 2021 01:12:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LANG=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Jun 2021 01:12:34 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Jun 2021 01:13:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:13:47 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Jun 2021 01:13:47 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Jun 2021 01:13:47 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:14:15 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:14:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 18 Jun 2021 01:14:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:15:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-robot=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac5aaa8e8d6f2718ea3399be2ceccb12c3671c0462f5b928bc29911340ad5a`  
		Last Modified: Fri, 18 Jun 2021 01:33:31 GMT  
		Size: 841.2 KB (841218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7733e5098e42a18dbf1389eeabc2d7d96a772f1b2d1d696b9bd5b048454e9856`  
		Last Modified: Fri, 18 Jun 2021 01:33:29 GMT  
		Size: 4.5 MB (4453623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86baa2b07fa5581dbc2acca8d98e5d7f054936602233e76d832060bcae884462`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f741d3ed102d529ad4de4e5e3865a0e350bec4a11ac50cb63f6e2b092726e2d1`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 2.0 KB (1986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f36bf64928ec06ec09b73241072ce39d84f27d333942a5e061e2dd06421bc6`  
		Last Modified: Fri, 18 Jun 2021 01:34:16 GMT  
		Size: 252.4 MB (252371566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61bc79117a6194e2fe81147b40cee75905865e8ff16681fe722faa33c764adc`  
		Last Modified: Fri, 18 Jun 2021 01:33:28 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4e6a4c64a1bee45b417e5b48c496770b79058fd842fd4702ce85c80cc3eccc`  
		Last Modified: Fri, 18 Jun 2021 01:34:41 GMT  
		Size: 63.1 MB (63057408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea15ff220b2dae79eb5a312dc91368a1ee8ebc57d150334d824697aa893d4db`  
		Last Modified: Fri, 18 Jun 2021 01:34:31 GMT  
		Size: 267.5 KB (267530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1626c56ec7b722f827563292a04cbe7163f36ffeadcee9da51986ea0136435`  
		Last Modified: Fri, 18 Jun 2021 01:34:45 GMT  
		Size: 67.2 MB (67222068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18da08529034abf78f8e8545cd98166a3681e28d751ae6cc847c76c0108432dc`  
		Last Modified: Fri, 18 Jun 2021 01:35:08 GMT  
		Size: 10.7 MB (10731410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
