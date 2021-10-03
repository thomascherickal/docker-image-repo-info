## `ros:melodic-perception-bionic`

```console
$ docker pull ros@sha256:5bb85a9f40433a9e0357c5a115d231469a934f08be614ff1bc5ef4ddcf0dbd65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-perception-bionic` - linux; amd64

```console
$ docker pull ros@sha256:073274ee3ed4b8853373529777dc094d60f8a7690085cd8789f67e16608e3762
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **742.5 MB (742504012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eb9859ebf79cd993bb8f61e0a64932761983cf954bb32eb0dfb1220002a0958`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:27 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:50:28 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 05:50:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 05:50:38 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 05:50:39 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 05:52:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 05:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 05:52:54 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:53:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:53:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 05:55:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 06:01:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1f1a2e289084ae7331c7d324ec0bdb4af258b35f6d415aa2a78464eea323f9`  
		Last Modified: Fri, 01 Oct 2021 06:22:10 GMT  
		Size: 4.9 MB (4872323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66e9143ca30cc349e28aaa680240c521074deafbfe5e607c1edddef9ff9b7e`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6333b668b4a22fa1cdec0303e29239d19d5da3da1233dce934bbf3e0b0a29c3f`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0d79c3d72ce11cacaac9a60a2a7a56df2d70ce72d76aecb0848c0c7ea69877`  
		Last Modified: Fri, 01 Oct 2021 06:22:44 GMT  
		Size: 259.5 MB (259455264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d7485b62d0716c5d117121940b0470fb16b3221d38dfb324bfe80b8bd40ea84`  
		Last Modified: Fri, 01 Oct 2021 06:22:09 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96d623e8dfff6321c98e2dc21ca6c60c27088565e0bc86da9f05fbec02803a5`  
		Last Modified: Fri, 01 Oct 2021 06:23:05 GMT  
		Size: 70.2 MB (70231150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296f19f55cae6979901def357825f36e69141b265ad585c9bf5326cb2b91ca63`  
		Last Modified: Fri, 01 Oct 2021 06:22:54 GMT  
		Size: 273.0 KB (272993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8fc01b5f326bafa63ce40161d166e1f5578f5f2d87989a2e5008cd9e812bd`  
		Last Modified: Fri, 01 Oct 2021 06:23:06 GMT  
		Size: 75.0 MB (74994903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d2455ea11a3f51289e515125af2fd29538c49291c3d9de5bf605c367fd146c`  
		Last Modified: Fri, 01 Oct 2021 06:24:17 GMT  
		Size: 305.1 MB (305129149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:18983de90a8231f4772cbb4bd48f42d91307993c015347f3fd066acf16977f38
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **645.7 MB (645744934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a57a275ef59016aa164b8013b4711ca65473bd2a171b44db6e165f690075900a`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:32 GMT
ADD file:ec8cec062962fe6498197aa4bfaf1953505e272985dda8d5e81465521d850fac in / 
# Sat, 02 Oct 2021 05:58:33 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:47:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:48:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 02 Oct 2021 22:48:17 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LANG=C.UTF-8
# Sat, 02 Oct 2021 22:48:18 GMT
ENV LC_ALL=C.UTF-8
# Sat, 02 Oct 2021 22:48:19 GMT
ENV ROS_DISTRO=melodic
# Sat, 02 Oct 2021 22:51:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:51:33 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 02 Oct 2021 22:51:34 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 02 Oct 2021 22:51:34 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:52:21 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:52:37 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 02 Oct 2021 22:53:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:57:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fe312f6db8a357ff205c74a1649d8c36186a76057c3223acbd31367e2dfd049`  
		Last Modified: Sat, 02 Oct 2021 06:02:32 GMT  
		Size: 22.3 MB (22304304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056c4e1c45e7370c0a89001ce3f27b8cb29dda1a3045cd21b5feb45b86814cc7`  
		Last Modified: Sat, 02 Oct 2021 23:10:35 GMT  
		Size: 841.6 KB (841600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761ddc01c5cd4707b222831b5c898c4b7c72dedbdf08c7c034c52e27d8fb48df`  
		Last Modified: Sat, 02 Oct 2021 23:10:34 GMT  
		Size: 4.1 MB (4085877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffb81f09de324d7eafb7dc79196a2d1a0aaaaeff8cf5ac7d677a48cca9b9c11`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348110f0ae217262ab74d39bdb78bc24d293b05a66c566e992e393aa8636729f`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35cea75c843f202719e12d6c0b65b06a1a2743414d67560aa090dfab89f781a`  
		Last Modified: Sat, 02 Oct 2021 23:13:03 GMT  
		Size: 238.9 MB (238932373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4a908a0a89a54ec468746bc176e64be9430edab2bf39917df6e1f5bebad7d8`  
		Last Modified: Sat, 02 Oct 2021 23:10:32 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ef458d73013d5c9b799742848a41a1f9cbd78cbde326a39b803252e573e99d`  
		Last Modified: Sat, 02 Oct 2021 23:13:45 GMT  
		Size: 54.7 MB (54696354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bca198f4909aba3f932611e3d650c626d3d048ef94761ee6c32858e7e4b54e`  
		Last Modified: Sat, 02 Oct 2021 23:13:15 GMT  
		Size: 273.0 KB (273025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61086c7dd1564bcc465f85db1b7f2909f76c12955724943f3cc231f86fb8d123`  
		Last Modified: Sat, 02 Oct 2021 23:13:59 GMT  
		Size: 64.7 MB (64746332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16465df1d782cdcb744de354dd6c511ba96fc0c32309b7bccba13b42675d8113`  
		Last Modified: Sat, 02 Oct 2021 23:17:16 GMT  
		Size: 259.9 MB (259862654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:90cbdcadb40a69fb9c9af3076c43913647e0decfabab70796c571b35fea4fd15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **703.4 MB (703413809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2b8dff296c7ff902c567db32969e245f3f6c73814572a8512817fdb32991f3b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:40 GMT
ADD file:35e2504756850fc1add00516fa89b0499b59c348457a96708eedb61313e7b25e in / 
# Fri, 01 Oct 2021 02:43:41 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:00:38 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:46 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:00:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 01 Oct 2021 04:00:54 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LANG=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV LC_ALL=C.UTF-8
# Fri, 01 Oct 2021 04:00:54 GMT
ENV ROS_DISTRO=melodic
# Fri, 01 Oct 2021 04:02:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:09 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 01 Oct 2021 04:02:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 01 Oct 2021 04:02:09 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:02:45 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:02:52 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Fri, 01 Oct 2021 04:03:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:05:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f46992f278c2dd50c481ff60ce8528b6eb59016ac6243e1a7fb385c79c5944b9`  
		Last Modified: Fri, 01 Oct 2021 02:45:30 GMT  
		Size: 23.7 MB (23727476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0703f9076c62d6a07ee4ac54a13d0cfcd29417e872bc88f5c170a4e31b2ee627`  
		Last Modified: Fri, 01 Oct 2021 04:18:40 GMT  
		Size: 841.5 KB (841467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f51453d2a9542a8e5552ed549fba6110526e6bba0d7dea78077ce930818d1`  
		Last Modified: Fri, 01 Oct 2021 04:18:39 GMT  
		Size: 4.5 MB (4453801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb854bd2d2160569f154fad52e3911260b4110a70c0410645d76246ddfd97ff5`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9766db03a07190e4dc3fa1dee3a3ae601d2ff84f341678f1e723e096b1af877f`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91559fa0ccbc5993e820912de1e62ef86dde1022279bf6c2ea3ce22578dea1b4`  
		Last Modified: Fri, 01 Oct 2021 04:19:20 GMT  
		Size: 252.4 MB (252369365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022e4617917637f78d14e5e0ff5a67b9753ffd80528ab27ecc82078077d34d5c`  
		Last Modified: Fri, 01 Oct 2021 04:18:38 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b78d023404d4cc6eb0e0116d7fe33f110d3d0037ab5a281daa0d867334ca48`  
		Last Modified: Fri, 01 Oct 2021 04:19:41 GMT  
		Size: 63.1 MB (63059707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a48409877036295323cd98bb5f3afdc9846c782bcea495aa268883a29d486aa`  
		Last Modified: Fri, 01 Oct 2021 04:19:32 GMT  
		Size: 273.0 KB (272994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb389997238be58731cc3f21699b7db36a2acba2c488fa7407bad3d48a40ec1e`  
		Last Modified: Fri, 01 Oct 2021 04:19:43 GMT  
		Size: 67.2 MB (67222055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c42f2f049dbe2df2b2e9101fd5b273df3b006c906cc94a31e261a4802b5e060`  
		Last Modified: Fri, 01 Oct 2021 04:21:00 GMT  
		Size: 291.5 MB (291464530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
