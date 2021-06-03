## `ros:melodic-ros-core-stretch`

```console
$ docker pull ros@sha256:40abae9f00f3ebd0548495a11b32cd022530a3210b2fb3acf7d182f89f201bb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-stretch` - linux; amd64

```console
$ docker pull ros@sha256:42a46006fdf4b5119465add4243aa67644ed70b6e326baded3008cb54fd392d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322305407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bf933924e8466d07f2cb3a2286a08b717d59335c1e4492832522043397f13c0`
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

### `ros:melodic-ros-core-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:ff0bed51bf09c8bc294d1596bbc6578daff8ae22382b633e4c77b7aa0e183d46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.7 MB (274743670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ecc1ec6b7fcb5eaffa6ff4618cde3c40a6be94fc21a45a23e56c8b68cefc2ff`
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
