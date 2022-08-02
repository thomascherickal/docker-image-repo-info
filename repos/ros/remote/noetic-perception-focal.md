## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:405997c50e0fa6f6330df7603d46f02d3e2df7c205205bfca958791b0e71f6ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:457af7c9a97b12ace89935dba24303c6e77d5c454eaebbfe029f41e7e515b0ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.1 MB (835138745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b22816876f9c718ecb4b11b361b0199aef666957dd676a6e0822138ba01e3d1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:10:15 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:10:36 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:10:37 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 02 Aug 2022 13:10:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 02 Aug 2022 13:10:38 GMT
ENV LANG=C.UTF-8
# Tue, 02 Aug 2022 13:10:38 GMT
ENV LC_ALL=C.UTF-8
# Tue, 02 Aug 2022 13:10:38 GMT
ENV ROS_DISTRO=noetic
# Tue, 02 Aug 2022 13:13:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:13:13 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 02 Aug 2022 13:13:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 02 Aug 2022 13:13:13 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 13:13:53 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:13:58 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 02 Aug 2022 13:15:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 13:22:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3f991215ddc16cd6d5839a01c05ba58b96914830f35c25d3d72e0495b053e7`  
		Last Modified: Tue, 02 Aug 2022 13:55:17 GMT  
		Size: 1.2 MB (1181319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aedc0c69710a5bf5069bd2509080fc6d8b47b7f817d02eb6b5c420be6abe69e`  
		Last Modified: Tue, 02 Aug 2022 13:55:15 GMT  
		Size: 5.5 MB (5546864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3519a1bb471cc6b2b4369f7cd39735754c6744b07b26c3124855dd894dcba45b`  
		Last Modified: Tue, 02 Aug 2022 13:55:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e2dfee34126a0fd475079e48bed7166ed0963c44262b6d1c8673a3cc31af08`  
		Last Modified: Tue, 02 Aug 2022 13:55:14 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825e59fe62383c77e16376834caef0bf40982defaf9019928a574c1e90132559`  
		Last Modified: Tue, 02 Aug 2022 13:55:54 GMT  
		Size: 177.0 MB (176996918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55778ffb7b3f4c8289907a297c07ad6b31e1c7ea5a410a5414c408630273346c`  
		Last Modified: Tue, 02 Aug 2022 13:55:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7e3c098d974561c8914411584759f9ec5ac5489735340137cb61a5ed6dfdca`  
		Last Modified: Tue, 02 Aug 2022 13:56:14 GMT  
		Size: 50.9 MB (50940142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde62a097a809942e493ede6b058a2b1af7c20561149da37ef0116f7250f4eb2`  
		Last Modified: Tue, 02 Aug 2022 13:56:05 GMT  
		Size: 323.5 KB (323534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a3313522d23bc6b63456324802c67644e381b81c42eab2a0fd5fccf81b324f`  
		Last Modified: Tue, 02 Aug 2022 13:56:18 GMT  
		Size: 79.6 MB (79603159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5935c43df901b4416e80cde1e4691707df0aa3d7393e2ad287d556fda18b98`  
		Last Modified: Tue, 02 Aug 2022 13:58:11 GMT  
		Size: 492.0 MB (491971800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:5874087d8190b2efab7c91cc84c5c666cb0510437df4b7643b00781ff77cd43e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.2 MB (726206634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c252a3c40ccb92883e0c452bbf8d223cd059b4014acb765415f8fe99a034fc1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 10:19:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 10:19:33 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 10:19:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 10:19:37 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 10:22:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:05:37 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 11 Jul 2022 23:05:37 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 11 Jul 2022 23:05:38 GMT
CMD ["bash"]
# Mon, 11 Jul 2022 23:06:17 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:06:29 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 11 Jul 2022 23:07:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:13:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e21254ce415ea7b490674f4a33c60349d312819e79bd953b7353e3dd7d14fea`  
		Last Modified: Tue, 07 Jun 2022 10:39:01 GMT  
		Size: 1.2 MB (1181840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48aa457454d70347a026cdb39a3d256e0969f6becf1cb485456cd0944fa7965e`  
		Last Modified: Tue, 07 Jun 2022 10:38:59 GMT  
		Size: 4.7 MB (4676394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672a3b2d46c78712db3b52ed8e3c47a9685c026d512bbf4bf05589aebd337cd`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac3050647c36fd475eac545b3dc5080db7e9f45e0871805c82cfff88c11326`  
		Last Modified: Tue, 07 Jun 2022 10:38:57 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f262fcc054725c10b56cb064f0fde57d26e36876aa8d0e0f6380250a21a79d`  
		Last Modified: Tue, 07 Jun 2022 10:41:05 GMT  
		Size: 157.4 MB (157415772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b342bdf9b11d603945c520ba34d1eb05324adb5bdcdb8870cba8fa987a2ba9c1`  
		Last Modified: Mon, 11 Jul 2022 23:19:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c046fbf5a031a4fc8b112134fc86acbf0c93d8a6af6da05bcaaf255a7aecf39`  
		Last Modified: Mon, 11 Jul 2022 23:20:11 GMT  
		Size: 40.6 MB (40643256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d7af22af4fa6b6b3bb6b3a8bbc9cf2d84563206385cc5fd4d464944fd11e16`  
		Last Modified: Mon, 11 Jul 2022 23:19:48 GMT  
		Size: 322.1 KB (322086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c959d6512be80be43cede75f20500c80a427f01f374fd31e7a7cc562466801`  
		Last Modified: Mon, 11 Jul 2022 23:20:29 GMT  
		Size: 60.5 MB (60482082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cd7610b3d7672a94207d78176c2fb8c7d6653ea4a02e442a0e5ee24538588a`  
		Last Modified: Mon, 11 Jul 2022 23:25:42 GMT  
		Size: 436.9 MB (436890147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:16e7a258f57c91d56ee5fc1a2372f22f05589dcc106bd5d6e73eb8a8542f182a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.8 MB (784791904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9357e75d3392cb0d42e5d21666083a68c2645d15a17a832bc2075172276c4679`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:05 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:14 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:15 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 07 Jun 2022 05:53:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 07 Jun 2022 05:53:18 GMT
ENV LANG=C.UTF-8
# Tue, 07 Jun 2022 05:53:19 GMT
ENV LC_ALL=C.UTF-8
# Tue, 07 Jun 2022 05:53:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 07 Jun 2022 05:54:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:47:48 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Mon, 11 Jul 2022 23:47:50 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Mon, 11 Jul 2022 23:47:51 GMT
CMD ["bash"]
# Mon, 11 Jul 2022 23:48:11 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:48:17 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Mon, 11 Jul 2022 23:48:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 11 Jul 2022 23:51:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260269f7c7c500761ab4d24037f4187c4da07bfe2287a50d134b0421fad862ac`  
		Last Modified: Tue, 07 Jun 2022 06:18:02 GMT  
		Size: 1.2 MB (1182691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3124e11618c0a455d11e98a3c2abad2b0dfa785eb7e7e709b4e9880836df1802`  
		Last Modified: Tue, 07 Jun 2022 06:18:00 GMT  
		Size: 5.3 MB (5322854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b585b092d4b03c6cfc18438bd8fae758a1faf754d6b7edb9d6e50b1c5497a0`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7925df845b292f9b56d2e9f66cdaf44241d8b3837eae5801a8b1a92dc8ee9ba9`  
		Last Modified: Tue, 07 Jun 2022 06:17:59 GMT  
		Size: 1.9 KB (1946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f914e2864654f248c7edef7ef55565585699438127fcca3bbf99cfd3928b2a2f`  
		Last Modified: Tue, 07 Jun 2022 06:18:28 GMT  
		Size: 171.3 MB (171348399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da1b00ae5b348c15e81d03e1d2081cfea916f10614ab2eb87aeb7a57a2e0680`  
		Last Modified: Tue, 12 Jul 2022 00:12:24 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df895f25f47a594fb69fc221385506b462b6721427f49bede7027853e0a059d2`  
		Last Modified: Tue, 12 Jul 2022 00:12:41 GMT  
		Size: 45.1 MB (45132483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b3e1b5161f62ed72d99a921276c534e8f7256c2b5cf1df8deb43f88a1126de`  
		Last Modified: Tue, 12 Jul 2022 00:12:34 GMT  
		Size: 322.0 KB (322037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991869ee032c5fdbd4b90f3ea8ba77128a2e59eef8e4145f300fa3cdf6b4d6d4`  
		Last Modified: Tue, 12 Jul 2022 00:12:45 GMT  
		Size: 71.8 MB (71754558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000648524589145fc922415060dc0ef2b75ac96f2ad73329ad10f511e9eeced1`  
		Last Modified: Tue, 12 Jul 2022 00:14:24 GMT  
		Size: 462.5 MB (462535302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
