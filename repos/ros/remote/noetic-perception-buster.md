## `ros:noetic-perception-buster`

```console
$ docker pull ros@sha256:93f41973e2701efd66d80512e6018bc7e36150ba908b4497099a3012eaa7cceb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-perception-buster` - linux; amd64

```console
$ docker pull ros@sha256:3dc735aa282843a7c175ab25a6ea9b650733d7e2586f796f9a507be73c13874b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **967.7 MB (967671794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57d4dfbca5e3c87961bf904b804cb2f63537410586fd5f0144c89f40789cae17`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:40 GMT
ADD file:8f75f11b2bd2d50e5912359ae750de06a7b49506df3756c19baf4cc63d900c4f in / 
# Tue, 09 Feb 2021 02:20:40 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:31:35 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:31:37 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 09 Feb 2021 11:31:38 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 09 Feb 2021 11:31:38 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 11:31:38 GMT
ENV LC_ALL=C.UTF-8
# Tue, 09 Feb 2021 11:31:39 GMT
ENV ROS_DISTRO=noetic
# Tue, 09 Feb 2021 11:33:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:33:14 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 09 Feb 2021 11:33:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 09 Feb 2021 11:33:15 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:34:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:34:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 09 Feb 2021 11:34:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:38:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0ecb575e629cd60aa802266a3bc6847dcf4073aa2a6d7d43f717dd61e7b90e0b`  
		Last Modified: Tue, 09 Feb 2021 02:26:22 GMT  
		Size: 50.4 MB (50400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b0d5528d4d10129063ca7f720f24b759ff2414147dc9acb4ce80df4042a60c`  
		Last Modified: Tue, 09 Feb 2021 11:45:02 GMT  
		Size: 10.9 MB (10890381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fa6dc1339a6d69805730444ca620a9a352afd3a7004102f807586d106f5d23`  
		Last Modified: Tue, 09 Feb 2021 11:45:00 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bbc1372440291fec04a189068eb2efaae76309c52126e7b243b4090f8b2bf0`  
		Last Modified: Tue, 09 Feb 2021 11:45:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c81b0773c3edd5e22f0d91661eb80b37b903b5c0d65fe00824b4414ed49690`  
		Last Modified: Tue, 09 Feb 2021 11:46:10 GMT  
		Size: 239.0 MB (238965006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb19dc30e7e64621f1fe2ec3c32280cf324c0e58cf772744426debd15fc3ae3`  
		Last Modified: Tue, 09 Feb 2021 11:45:00 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce894a3ca817b79ed4942f240675048b110277f1210e32393674430d7f89f88`  
		Last Modified: Tue, 09 Feb 2021 11:46:42 GMT  
		Size: 86.6 MB (86563808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f0fb09c754a09ff6584dc9772046b55cc02e6d766bcf93f7a5c245b178153`  
		Last Modified: Tue, 09 Feb 2021 11:46:14 GMT  
		Size: 265.4 KB (265403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba79683d6e5abc56820da992383dcca1a9d7020af18307967bd372fd68c8237b`  
		Last Modified: Tue, 09 Feb 2021 11:46:43 GMT  
		Size: 76.0 MB (75966915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c1d0e58374e9de8bf242c89f61068e002f3f97252ba3f2f5dec053e8528756`  
		Last Modified: Tue, 09 Feb 2021 11:49:31 GMT  
		Size: 504.6 MB (504618246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ef36f75e510571e904cda19aa94c1d3307d920cbd41e9d9c5ea53d218e6fbcc2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **884.6 MB (884594361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50ba0f29a308bb9239c39373450c7956d5da9b722fd109e98b8c1f979cc30d3d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Feb 2021 02:40:45 GMT
ADD file:78412ee35e3dc6fb5fdfce41eb05dd273ba1d49328ab327465639bfa4821aa51 in / 
# Tue, 09 Feb 2021 02:40:50 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:56:12 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:56:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 09 Feb 2021 17:56:18 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 09 Feb 2021 17:56:19 GMT
ENV LANG=C.UTF-8
# Tue, 09 Feb 2021 17:56:20 GMT
ENV LC_ALL=C.UTF-8
# Tue, 09 Feb 2021 17:56:20 GMT
ENV ROS_DISTRO=noetic
# Tue, 09 Feb 2021 17:58:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:58:48 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 09 Feb 2021 17:58:49 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 09 Feb 2021 17:58:49 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 17:59:37 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 17:59:51 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 09 Feb 2021 18:00:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 18:07:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c78c297fb0d010ee085f95ae439636ecb167b050c1acb4273bd576998cf94a83`  
		Last Modified: Tue, 09 Feb 2021 02:47:03 GMT  
		Size: 49.2 MB (49183229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7dc7e7c1a8c9728249478a065c8cbfb7b26a4ffcb6f0b8d2241f6af8e52bc0`  
		Last Modified: Tue, 09 Feb 2021 18:14:07 GMT  
		Size: 10.9 MB (10883298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94eec5caa2ce9024a59191b2c94308fe2f8cab9cea9031dc8de51fe09b658b9b`  
		Last Modified: Tue, 09 Feb 2021 18:14:05 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3affe42ffed8a74195454befbffcb5181f154b98092d214bc56ca825fc614162`  
		Last Modified: Tue, 09 Feb 2021 18:14:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569558cbdfd3b1304e6ccc1a802a2634583633f160a18c3e34ff32c204a1ae1a`  
		Last Modified: Tue, 09 Feb 2021 18:15:00 GMT  
		Size: 184.2 MB (184192209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eec434d09b660bdf210b479e8ab10f8dec24da00f6361f141deba874b5a5dd4`  
		Last Modified: Tue, 09 Feb 2021 18:14:05 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66f27b22b6974f56118d930deb6207e44e7e8add8cbc82f0829ddee0f10f4da`  
		Last Modified: Tue, 09 Feb 2021 18:15:25 GMT  
		Size: 84.4 MB (84356272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6a8a6171a7e04f96481d49b3c664ea44cd3ccc5cf3db48a643cc5acbaa6d13`  
		Last Modified: Tue, 09 Feb 2021 18:15:07 GMT  
		Size: 265.5 KB (265464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226656fcbaca78e8c1a4c422cc3c1555f3a03c699d36a9a6e59869ca28e5171b`  
		Last Modified: Tue, 09 Feb 2021 18:15:25 GMT  
		Size: 74.1 MB (74088828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2673ce1184062860032d45df00fb5a22e12c86a4d994b874bd44e3b91ed7c8ed`  
		Last Modified: Tue, 09 Feb 2021 18:17:40 GMT  
		Size: 481.6 MB (481623222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
