## `ros:melodic-perception-stretch`

```console
$ docker pull ros@sha256:62b265d2bad056d4a16f2a9c2cd2b436fe59d3b173f0a65f925ea63f4b5c742e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-perception-stretch` - linux; amd64

```console
$ docker pull ros@sha256:d8a43b8576c9173d29db39f6bfd0c11853bac69b5ad785549eef0e101261cd0d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **828.6 MB (828633196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238b4598debcea3ca00bbb453b10303ffc2bab5638cf5c5f76d96adca57d040d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:09:11 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:00:06 GMT
RUN echo "deb http://snapshots.ros.org/melodic/final/debian stretch main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Wed, 02 Jun 2021 19:00:10 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Wed, 02 Jun 2021 19:00:10 GMT
ENV LANG=C.UTF-8
# Wed, 02 Jun 2021 19:00:10 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Jun 2021 19:00:10 GMT
ENV ROS_DISTRO=melodic
# Wed, 02 Jun 2021 19:01:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:01:42 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 02 Jun 2021 19:01:42 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Jun 2021 19:01:42 GMT
CMD ["bash"]
# Wed, 02 Jun 2021 19:02:04 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:02:11 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Jun 2021 19:02:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:04:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a867e9d598a219f826e3b76f5280f3d106205d5fa6b8e1f2d421fd463d8fbc`  
		Last Modified: Wed, 12 May 2021 17:21:34 GMT  
		Size: 6.9 MB (6869206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806b5e34c0f9f269961b5781d9aba67f9f4183d234713f263b010f9b0d4bbbcf`  
		Last Modified: Wed, 02 Jun 2021 19:38:46 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee85c3e9eced97a3c32dd7a45e3d6ef13e607bc3b3558341e372eee43a0bfe12`  
		Last Modified: Wed, 02 Jun 2021 19:38:46 GMT  
		Size: 2.0 KB (1965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f89b811f91ec6ca8d8b14d865b71579612b632a157e59aad1a6cbdf2970de27`  
		Last Modified: Wed, 02 Jun 2021 19:39:35 GMT  
		Size: 270.1 MB (270053723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8307615d07774e7000441ddd64320d26bd29a216e8bb057553405fed414b61f`  
		Last Modified: Wed, 02 Jun 2021 19:38:46 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18de1191b262173355c8360bca74edf306649ba9239180db5e07c2478612735`  
		Last Modified: Wed, 02 Jun 2021 19:39:56 GMT  
		Size: 70.2 MB (70166157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26f6b9906a8515fc55b795191991b5c1aded9c271647277106de79b84129435`  
		Last Modified: Wed, 02 Jun 2021 19:39:44 GMT  
		Size: 265.8 KB (265841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c95c17834a9c5e893c0755ab6bff63b045d2fc0aa8b31b5d4b0c7ab0867dc1`  
		Last Modified: Wed, 02 Jun 2021 19:39:55 GMT  
		Size: 55.1 MB (55060168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53570bfffed893acf07e26dea2723ee54e5ff4a75be8f99ed17a6d3b9a0596a0`  
		Last Modified: Wed, 02 Jun 2021 19:41:21 GMT  
		Size: 380.8 MB (380835623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:9d0198cce68ab53275b798f17a53594e3482de7ea4c118634edcd43ff4bc54f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **749.8 MB (749823331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8cba986d4495a2ea0e4b0fb119e3a226bfcff827fba2df5ee6b4e7df20c20fe`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:56:12 GMT
ADD file:9582243afc9973a3708fda530270ae8f23796b20a532a9f07e4faaf245e2cdc0 in / 
# Wed, 12 May 2021 00:56:18 GMT
CMD ["bash"]
# Thu, 27 May 2021 15:04:52 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:23:59 GMT
RUN echo "deb http://snapshots.ros.org/melodic/final/debian stretch main" > /etc/apt/sources.list.d/ros1-snapshots.list
# Wed, 02 Jun 2021 19:24:02 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Wed, 02 Jun 2021 19:24:02 GMT
ENV LANG=C.UTF-8
# Wed, 02 Jun 2021 19:24:02 GMT
ENV LC_ALL=C.UTF-8
# Wed, 02 Jun 2021 19:24:03 GMT
ENV ROS_DISTRO=melodic
# Wed, 02 Jun 2021 19:25:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:25:13 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 02 Jun 2021 19:25:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 02 Jun 2021 19:25:13 GMT
CMD ["bash"]
# Wed, 02 Jun 2021 19:25:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:25:47 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 02 Jun 2021 19:26:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Jun 2021 19:28:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:41f38ce3010a5142300d74e5e19db4dea7694f4771471c330fff27c633f8ba32`  
		Last Modified: Wed, 12 May 2021 01:04:15 GMT  
		Size: 43.2 MB (43177820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a98e1e3f21a423192b7c1a0497b1b7bfc382689c0aff9a0673c2497a89c2f9f`  
		Last Modified: Thu, 27 May 2021 15:40:04 GMT  
		Size: 6.4 MB (6442854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aab821c93c95ad1917a68b3d81eb4785c5f54faf8ab8a4cc746480c8179d874`  
		Last Modified: Wed, 02 Jun 2021 19:55:39 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d70f62b3be8df920f934567e2965aed275a7afbf55d3c90063aaacd79e79188`  
		Last Modified: Wed, 02 Jun 2021 19:55:39 GMT  
		Size: 2.0 KB (1964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a7078f00f6f54181503eea8adf4a1382ac309d390e4ec5ea237dc98eb41943`  
		Last Modified: Wed, 02 Jun 2021 19:56:26 GMT  
		Size: 225.1 MB (225120605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf2345f2898602d8da70b83146cce1ac9610bfca55c09917e87cc95fd74c4ee`  
		Last Modified: Wed, 02 Jun 2021 19:55:39 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca2ace983a0e9c4f385ab16e8718b9b82220d28a12b62b76c689dcefa98c838`  
		Last Modified: Wed, 02 Jun 2021 19:56:46 GMT  
		Size: 64.8 MB (64848833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcef86dfc556ac05f408def4dbdc2dd569e5a1e432e0ae394f4a61ecae576525`  
		Last Modified: Wed, 02 Jun 2021 19:56:35 GMT  
		Size: 265.8 KB (265837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a47cf72aec1274eaa4af45e177f7c2076d593b98aef1b4ccff107e195e01d30`  
		Last Modified: Wed, 02 Jun 2021 19:56:45 GMT  
		Size: 53.2 MB (53241626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0091e7602f9348eeb3b7f86ff10abb018f1abe35f3c77a9d9ca28e50e7fd75f`  
		Last Modified: Wed, 02 Jun 2021 19:58:12 GMT  
		Size: 356.7 MB (356723365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
