## `ros:melodic-ros-base-bionic`

```console
$ docker pull ros@sha256:7a44a7dc552fa6ac2a060957f165fbb5d945efc3754d4b41d74e93e84db4ee60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-base-bionic` - linux; amd64

```console
$ docker pull ros@sha256:b35e906f707bf988db588f95ca6370e62514d104a193a57b4632649a0d97b48c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437394244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5023ff407aa1e7f107544b46c999a8edce6403d120be868f5edb7d852da0eb`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:12:16 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:16:22 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:16:23 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:16:23 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:18:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:18:54 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:18:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:18:54 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:19:35 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:19:41 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 03:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d08ae4a50ec7a4071fcd259c6dc2b8f3219e66e5206c2f15ee781c4691a7699`  
		Last Modified: Fri, 22 Apr 2022 02:30:38 GMT  
		Size: 839.0 KB (838982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca35b07994f608387e199fa484cf0d3a586144538b7ea207fea47c25e64441b`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 4.9 MB (4872320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e99e7d92f7a9c84f55e914a1ad549e14ba4885ce72e1422955549eb8a42412`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda5797f8b0a501462dae5d9c7c7baa2ab56476067c48007d7f7d5f28e027821`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fdb800ef4ebf782b8706d3ca51c5602217bfdaccffd3c87e146da0fd5b913a`  
		Last Modified: Fri, 22 Apr 2022 03:47:53 GMT  
		Size: 259.5 MB (259455669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1a8004d93ae4d2dcb4e49fb62c1ad152510f72453bd6d548075d99ffce4a72`  
		Last Modified: Fri, 22 Apr 2022 03:47:18 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2772d37526d353480c40bc6613660a726bae949372e0b95ff5a4e9aef62d22cc`  
		Last Modified: Fri, 22 Apr 2022 03:48:13 GMT  
		Size: 70.2 MB (70241270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b2bccc87971a9fadd6a92eb4daea27c47e122f6de0c129f9cb64e2aa64019c`  
		Last Modified: Fri, 22 Apr 2022 03:48:03 GMT  
		Size: 279.1 KB (279107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162f4d6dcfc3bd2fa9202d04bbd1d4f684046c0a525682228e9024af7ee3fee6`  
		Last Modified: Fri, 22 Apr 2022 03:48:15 GMT  
		Size: 75.0 MB (74994599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:d51f745118c1f2f871a53857d6fa43c319e1b11e05353c954b754dff1ebce246
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385894248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9755007044d18ebaf5ad0797a66860a8edf199e519078b4c8045798b5baf5af6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Apr 2022 03:25:38 GMT
ADD file:3230d8a499e37ff816595cbac3892a80005afccf8a55053c28e24989d52de08b in / 
# Wed, 06 Apr 2022 03:25:38 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:21:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:22:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:22:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 06 Apr 2022 04:22:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 04:22:08 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 04:22:08 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 04:22:08 GMT
ENV ROS_DISTRO=melodic
# Wed, 06 Apr 2022 04:25:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:25:23 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 06 Apr 2022 04:25:23 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 04:25:24 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:26:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:26:30 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 06 Apr 2022 04:27:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:419a71fa3c92c7dd0e8cfbfdf694362de1c27dafed508aeb2e5bc9ff8376fc98`  
		Last Modified: Tue, 05 Apr 2022 13:12:06 GMT  
		Size: 22.3 MB (22301415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a162be1c1e08f96d0b744482cc8ea911a59b5c915fff0f162674de69d7dfec01`  
		Last Modified: Wed, 06 Apr 2022 04:44:24 GMT  
		Size: 839.8 KB (839819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ff94372f98929867eb27c75aacf2dcb73c9ebb69048809947955507b28e457`  
		Last Modified: Wed, 06 Apr 2022 04:44:23 GMT  
		Size: 4.1 MB (4085911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0937b2511b635d32459e8503e109907f45c153c0bba95cac38bd7b919ca97df5`  
		Last Modified: Wed, 06 Apr 2022 04:44:21 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f184306a6b3e4850d73085a52f44ae5d7109134640429bb555ed064aa2ccb09f`  
		Last Modified: Wed, 06 Apr 2022 04:44:21 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e6e094f9f6f883c0c73aa3d5feac7a3f16f33d067dbe521f52633b79ad0fc7`  
		Last Modified: Wed, 06 Apr 2022 04:46:56 GMT  
		Size: 238.9 MB (238935223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886a3ef67c69ec977d8faff06a9220e6e78ff582bf828c458605a4510e0764d0`  
		Last Modified: Wed, 06 Apr 2022 04:44:21 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46293b6905d1c77e537bb2d6cde17e435f9adc3ec11bf008c6c7a778154ddff3`  
		Last Modified: Wed, 06 Apr 2022 04:47:37 GMT  
		Size: 54.7 MB (54704560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04ab1c6bd68c58a4bcac4841ed95ccd4ebfb1a1a3a9602b6343329961321d53`  
		Last Modified: Wed, 06 Apr 2022 04:47:08 GMT  
		Size: 278.3 KB (278290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba872f01c3e4f8a0a5b650ec09b911bfce81dfb79368767fe4812f23254445d`  
		Last Modified: Wed, 06 Apr 2022 04:47:53 GMT  
		Size: 64.7 MB (64746614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-base-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ef4ec58b9955078e592b2a50d64c7f8018c28cc9c0253b94f3cda56041dc5f9d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.6 MB (411582050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac3813e667132713e7951661e3eee6e90e0adbce9e3577cd548e30071b47a357`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:57:55 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:58:06 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 22 Apr 2022 03:58:08 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 22 Apr 2022 03:58:09 GMT
ENV LANG=C.UTF-8
# Fri, 22 Apr 2022 03:58:10 GMT
ENV LC_ALL=C.UTF-8
# Fri, 22 Apr 2022 03:58:11 GMT
ENV ROS_DISTRO=melodic
# Fri, 22 Apr 2022 03:59:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 03:59:35 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 22 Apr 2022 03:59:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 22 Apr 2022 03:59:37 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:00:09 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:00:15 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 22 Apr 2022 04:00:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9991268c4fa13de60874e7dd3d4c276053870b643d71a9e6808cf551cec78c69`  
		Last Modified: Fri, 22 Apr 2022 04:19:23 GMT  
		Size: 839.6 KB (839562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8217dd686adf3e2a9d1c96f4131cf1ff99981a9557c2b767389451f95719e3`  
		Last Modified: Fri, 22 Apr 2022 04:19:21 GMT  
		Size: 4.3 MB (4263955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164af0db1aea4c00740d19f1ef54d28fd8c41b57660798a7c26d4cc708654e22`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1033fb88de2a87d8a8ac97d613e57b642c09ce118387a5ccce46da5a3667d67`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643870d428d053d50273e3ca85573f30f06bcd32b4c958275aa3db0b844425d4`  
		Last Modified: Fri, 22 Apr 2022 04:19:55 GMT  
		Size: 252.4 MB (252383787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3cf54f364459cd8947339454907449795d8272a7a92962f27f4692f18bba2f`  
		Last Modified: Fri, 22 Apr 2022 04:19:20 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3168bfd2af65c12c75b36110ee9849bf17f0a8cfd2fd4deda87b4ae07783c173`  
		Last Modified: Fri, 22 Apr 2022 04:20:16 GMT  
		Size: 63.1 MB (63077142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673370a62a7d0e523c90eb7dc5ab53ff7f7515405c0db3b5cd8f2ed93328eb2f`  
		Last Modified: Fri, 22 Apr 2022 04:20:08 GMT  
		Size: 279.1 KB (279050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cae3a8e6abf8db5050c4f0924855d5aa48eda381fae3af8f9f41d7402e96571`  
		Last Modified: Fri, 22 Apr 2022 04:20:18 GMT  
		Size: 67.0 MB (67001727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
