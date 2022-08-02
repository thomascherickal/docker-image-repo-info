## `ros:noetic-robot-focal`

```console
$ docker pull ros@sha256:ac69bc791c9dbd251df38f00bb9aa3b8284703b28eff3348dc54a4f36e99a0be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot-focal` - linux; amd64

```console
$ docker pull ros@sha256:db42b54ef7554d262ac6398dfdaf2ceb5d7eb59420f9ae4a23bf6029e921996f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359027107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b091aa21da0fbc744566faba05547001227262d90ab5c67291570aab854a8ae`
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
# Tue, 02 Aug 2022 13:16:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:8e723cb9b102de21090742e561236e03f5e341ca0d0a088210da2a9f7ee0c37b`  
		Last Modified: Tue, 02 Aug 2022 13:56:35 GMT  
		Size: 15.9 MB (15860162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:bc0eeeb1ee5510804a8ab8133fd705d2b03cad8b652fa75b65e42a6091ceb0bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303381184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a152a8065c0a7d864e1c89ff62ee286f491b4bb34e10ca6e23c6e6507f0c78`
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
# Mon, 11 Jul 2022 23:08:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:aa289c2880f665c3c543268ddd1ad35cda3671b682b38f5824306b3756aae84e`  
		Last Modified: Mon, 11 Jul 2022 23:20:55 GMT  
		Size: 14.1 MB (14064697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:cbf96a4814f0622276c20a8784485394803d69bf74112b688d42f4d53c23d507
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.7 MB (337705306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edfc6f5a44b36caad2da24b73c2cd341ec290ea3316aa626c59ffc6c210cff24`
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
# Mon, 11 Jul 2022 23:49:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:5fbc5b84ce4478bbeb4077ed68dc1476c730ef3acd8d52f5990e91f57b2b8490`  
		Last Modified: Tue, 12 Jul 2022 00:13:05 GMT  
		Size: 15.4 MB (15448704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
