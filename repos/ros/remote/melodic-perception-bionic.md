## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:12d369bf08ffb81b2dae838f7861fa7bba940bc7e3a35fc15a7060f80eb0d610
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:b2adfb2e10b8a32e49ee4c83cabe2dea965551d3f244475776f4f9d6b0dfd68a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.7 MB (742710450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2748759a07ed8c009098ab380cc2e4dc73f2e981035929b7247147ef0e9c6ed4`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:42 GMT
ADD file:8a4ddbd462c1dd2016c64bd71ea6b5dba2ac4934bfd235a04d55b364666b67d1 in / 
# Tue, 05 Apr 2022 22:20:43 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:41:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:12:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:12:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 06 Apr 2022 02:12:29 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 02:12:29 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 02:12:29 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 02:12:29 GMT
ENV ROS_DISTRO=melodic
# Wed, 06 Apr 2022 02:14:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:15:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 06 Apr 2022 02:15:03 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 02:15:03 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 02:15:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:15:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 06 Apr 2022 02:16:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 02:22:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08a6abff89437fab99b52abbefed82ea907f12845c30eeb94f6b93c69be93166`  
		Last Modified: Tue, 05 Apr 2022 13:10:59 GMT  
		Size: 26.7 MB (26708938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b732c52c0461890d4114ac1d6f5a90dc52c395a65c4bd758b0c8ec6d738eac1`  
		Last Modified: Tue, 05 Apr 2022 23:59:27 GMT  
		Size: 838.9 KB (838902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656b41acd8def5851e0236575b2ccbf5ee29c14393fdb041320f87b027121b91`  
		Last Modified: Wed, 06 Apr 2022 02:43:13 GMT  
		Size: 4.9 MB (4872183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c31bef3c8aea03bf71158539e4a26a0e727f69f59f36cad07a341c67386dbe`  
		Last Modified: Wed, 06 Apr 2022 02:43:12 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d8f3301e951a7dfb9cdbab62a9aac23cb0a8a720896539c823bc63779b6dc0`  
		Last Modified: Wed, 06 Apr 2022 02:43:11 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20428422782224ecc939df68824f15aa7ee865a5d8e9f903d7b937641b4f123`  
		Last Modified: Wed, 06 Apr 2022 02:44:00 GMT  
		Size: 259.5 MB (259456999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac8708c288ed99d371db1e1762210ab955ce82139acb17447766a6f8ce668db0`  
		Last Modified: Wed, 06 Apr 2022 02:43:12 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8071d972208b130fac8a8556d8c4774ead4c69961365025c75420768c114afa`  
		Last Modified: Wed, 06 Apr 2022 02:44:21 GMT  
		Size: 70.2 MB (70235486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc5c642c10259cd56251f58188a600e2e4bb0a661f35d14011ba7c541dc0734`  
		Last Modified: Wed, 06 Apr 2022 02:44:10 GMT  
		Size: 278.3 KB (278313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab084b52e6dd8c0fa3cde1613c1d6853e5bcf9a385cb8b4d5e0c736a4c8d370`  
		Last Modified: Wed, 06 Apr 2022 02:44:27 GMT  
		Size: 75.0 MB (74994999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfa6de21717b08f8c78589d6d3dac8a48aa76c57383e5d20caae3452e932ad1`  
		Last Modified: Wed, 06 Apr 2022 02:45:47 GMT  
		Size: 305.3 MB (305322215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:97d8589f4ebb646983a5334343eb2f23b272f8925f965899375b56a2f9f7addb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.9 MB (645938091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93799e84e5e200aad01cf1890e5490d70c00a94e934e698c5891e787e4e87f42`
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
# Wed, 06 Apr 2022 04:31:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:a417a939e068bc731c30f257ca0440e58bb024db95162b6a12fee935f00847a2`  
		Last Modified: Wed, 06 Apr 2022 04:51:12 GMT  
		Size: 260.0 MB (260043843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:4d4788b58d6b684a00fcac947f4a54c801987126c4ceb05cced4136b322518df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.0 MB (702957155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70d4b785d830ddb640d56f4d7197770bb93cb041288041aedc648903d359bd53`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:40:51 GMT
ADD file:bb36cf2c131b65fcf3f10eac5cb640ad749d77110482b30bff982a284aa9e9ec in / 
# Tue, 05 Apr 2022 22:40:51 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:02:01 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:02:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:02:12 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 06 Apr 2022 00:02:14 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 06 Apr 2022 00:02:15 GMT
ENV LANG=C.UTF-8
# Wed, 06 Apr 2022 00:02:16 GMT
ENV LC_ALL=C.UTF-8
# Wed, 06 Apr 2022 00:02:17 GMT
ENV ROS_DISTRO=melodic
# Wed, 06 Apr 2022 00:03:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:03:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 06 Apr 2022 00:03:40 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 06 Apr 2022 00:03:41 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:04:10 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:04:21 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 06 Apr 2022 00:04:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:07:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d35feac4abe85b38af36ec148f2c2dc7a795f9862a0b6dcf2a1511b752a44996`  
		Last Modified: Tue, 05 Apr 2022 13:11:37 GMT  
		Size: 23.7 MB (23730866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cafe3bc9ff724c70f720ff738c3e724cfa285eacc5756b11e4ec83f883d345`  
		Last Modified: Wed, 06 Apr 2022 00:22:28 GMT  
		Size: 839.7 KB (839677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e7b86a897351a28097247359d6d356b04139c42ff35871c740b3a2a7a5380`  
		Last Modified: Wed, 06 Apr 2022 00:22:26 GMT  
		Size: 4.3 MB (4264068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7784583ca0c82d8e7c3c30fc4def03aea35cd0704da7b1abe916b5de2a264e4a`  
		Last Modified: Wed, 06 Apr 2022 00:22:26 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7ec1168691379152172f56c4f702252d305664a82ff13917f0bda00c26c15`  
		Last Modified: Wed, 06 Apr 2022 00:22:26 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2e5728f7c984b33f56560ff16dedaafc3e2a66fecb6f35f06ba609e8ee8f71`  
		Last Modified: Wed, 06 Apr 2022 00:23:02 GMT  
		Size: 252.4 MB (252381175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de082d48add89480d196d0adce610edec0e7c4b754f7dd74ab3c0b9943398c5e`  
		Last Modified: Wed, 06 Apr 2022 00:22:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7cabadf307e3b30ad929b1c5354282831aef4071313385f549814286a4a461`  
		Last Modified: Wed, 06 Apr 2022 00:23:22 GMT  
		Size: 63.1 MB (63067720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7f3a2803b1d91eaee8153f5e2820fbafa6d79ce3a261303d6a12e65a3d6d54`  
		Last Modified: Wed, 06 Apr 2022 00:23:13 GMT  
		Size: 278.3 KB (278266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab52156ca5b28385aa0fd74c771480aa176395d2ceeb2b2962ec63e7b66398e7`  
		Last Modified: Wed, 06 Apr 2022 00:23:24 GMT  
		Size: 67.0 MB (67002171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff8acc336509fdc1d8bcf22c251fb07a46af685ccb2e29e681b446048fc3a7a`  
		Last Modified: Wed, 06 Apr 2022 00:24:34 GMT  
		Size: 291.4 MB (291390845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
