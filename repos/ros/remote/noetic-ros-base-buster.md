## `ros:noetic-ros-base-buster`

```console
$ docker pull ros@sha256:55865f166dc3d467f11b106729724409801c1c4b2d8786936aea09d53c7b7b1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-base-buster` - linux; amd64

```console
$ docker pull ros@sha256:0562cc97b056eb1e665438bf2c68a5686fbedd7990ff6788f2da5c30d45665f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.3 MB (463275883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e294c766aaf32edb1a2885f0482b1848b8c496b16a4e2d0c469e4eea1d4157f`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:22:41 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:22:42 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 12 Oct 2021 04:22:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 12 Oct 2021 04:22:45 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 04:22:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 12 Oct 2021 04:22:46 GMT
ENV ROS_DISTRO=noetic
# Tue, 12 Oct 2021 04:24:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:24:29 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 12 Oct 2021 04:24:30 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 12 Oct 2021 04:24:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:25:07 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:25:13 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 12 Oct 2021 04:25:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1879fc7dd1b539861f67f1a1f2560ac72901b2ec692bcd502d7dbd78747aec`  
		Last Modified: Tue, 12 Oct 2021 04:30:11 GMT  
		Size: 10.9 MB (10891815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6513f455c2f9ae29007328538218f9e3fb1ad2f676464032ac997367c06bd20f`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acccdf05e200940e857fda740a50ca8637c81a0035ec822e0bd50a4a0f869adf`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4f3f2e3176a668407560bf65a733da19af24e22a7017e0b28b27cc775aecdc`  
		Last Modified: Tue, 12 Oct 2021 04:30:46 GMT  
		Size: 239.1 MB (239086052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7276317c1b25ab860c01a572280c0f14572628e108816c4971ff0e711979e2`  
		Last Modified: Tue, 12 Oct 2021 04:30:10 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cd7ef11df9f4c2994b6c766b52d97136fd40ddf75f985c0256383ff4c20c09`  
		Last Modified: Tue, 12 Oct 2021 04:31:10 GMT  
		Size: 86.6 MB (86566451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76df43754e281f9238cf8d03034b1548ed88b4b2fc4010c703439cdeeec0ff8`  
		Last Modified: Tue, 12 Oct 2021 04:30:54 GMT  
		Size: 317.2 KB (317177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899a51b12df1bc48c66b5be9054bdaea88bbde4fbf2eb0be77273b2aa54eb5b3`  
		Last Modified: Tue, 12 Oct 2021 04:31:05 GMT  
		Size: 76.0 MB (75975282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-base-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:2ead67f2f4e708b83ba09ee7e4b274882ddd397f9574aaa8f26af03199977b28
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **402.8 MB (402750993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90dde0ba9a1344c26edaeacb4e64fe2315ac51bb119bbc9b9fbfcfee9a5464e0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:55:30 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:55:30 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 17 Nov 2021 09:55:38 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 17 Nov 2021 09:55:39 GMT
ENV LANG=C.UTF-8
# Wed, 17 Nov 2021 09:55:40 GMT
ENV LC_ALL=C.UTF-8
# Wed, 17 Nov 2021 09:55:41 GMT
ENV ROS_DISTRO=noetic
# Wed, 17 Nov 2021 09:57:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:57:06 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 17 Nov 2021 09:57:08 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 17 Nov 2021 09:57:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:57:41 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:57:54 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 17 Nov 2021 09:58:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6567e1e1e6c972c4d10ef0b28be7441b9faba756aef9d8502c13834239097e49`  
		Last Modified: Wed, 17 Nov 2021 10:05:24 GMT  
		Size: 10.7 MB (10688089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1a10d650dd3ccec5c33cb88fd591b4d3377d74b6bc192bfc5703c3377d2490`  
		Last Modified: Wed, 17 Nov 2021 10:05:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5555e0dff8030a1664f72dbd55c2ccb0f9643856a0543a792754ce07a9a295`  
		Last Modified: Wed, 17 Nov 2021 10:05:22 GMT  
		Size: 1.9 KB (1949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aba732adf84216832ef6ac06de2d7a0f183d75a35f86164d76ad6c20b84e81d`  
		Last Modified: Wed, 17 Nov 2021 10:05:54 GMT  
		Size: 184.3 MB (184302665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77ffa64df86146e7a47c4de87957d94a0df3a134a9c3b631ac299b4ac79f716`  
		Last Modified: Wed, 17 Nov 2021 10:05:23 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8cbbefff3909b904d5a6b9278f2706cb037366625e701143f47f2d9171ac36`  
		Last Modified: Wed, 17 Nov 2021 10:06:13 GMT  
		Size: 84.4 MB (84350861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8330a922777eecbb2b62936269690eff07ec9f74763739d6c64c216921bcb1`  
		Last Modified: Wed, 17 Nov 2021 10:06:02 GMT  
		Size: 319.6 KB (319619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a208bf616b1d8d934b041d89a2c229baac87ab27ba204fa7abc72d8d152427f`  
		Last Modified: Wed, 17 Nov 2021 10:06:12 GMT  
		Size: 73.9 MB (73864399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
