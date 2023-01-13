## `ros:galactic-ros-core`

```console
$ docker pull ros@sha256:db6cd6f52305444b6b62e3504c24e9de45132b9fe564eba9f5846fee496d0a2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:galactic-ros-core` - linux; amd64

```console
$ docker pull ros@sha256:74fef32ef7b9d25830ddff85b4463027f469b34b8783ff3b6f8ffb824a8d875e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.3 MB (139301397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19b3243e3cf1befd33dea790fab5e8dd3ac26fa1a30e25d6963966caf1142f48`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:05:57 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 04:56:29 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 23:20:30 GMT
RUN echo "deb http://snapshots.ros.org/galactic/final/ubuntu focal main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 12 Jan 2023 23:20:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 12 Jan 2023 23:20:31 GMT
ENV LANG=C.UTF-8
# Thu, 12 Jan 2023 23:20:31 GMT
ENV LC_ALL=C.UTF-8
# Thu, 12 Jan 2023 23:20:31 GMT
ENV ROS_DISTRO=galactic
# Thu, 12 Jan 2023 23:22:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 23:22:28 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 12 Jan 2023 23:22:28 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 12 Jan 2023 23:22:28 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caabce4ffd25edf36993bf0280efcd423502afe7b8c7b2da5782388b72f81a89`  
		Last Modified: Fri, 09 Dec 2022 02:17:31 GMT  
		Size: 1.2 MB (1154736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5c569c2442d05771daee8e23d1b056915b3dc9dd15887bfc5723720f10c7a6`  
		Last Modified: Fri, 09 Dec 2022 05:34:20 GMT  
		Size: 5.6 MB (5551517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18533ac4b95004ac48f1ae8e3cd0f52b628285c5c99212a9ccaf8309191fc2b4`  
		Last Modified: Thu, 12 Jan 2023 23:27:05 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f73489d6d95d231ecd0b99ba2939cfc514babae220fee00a8f1d80ef672c52`  
		Last Modified: Thu, 12 Jan 2023 23:27:05 GMT  
		Size: 2.4 KB (2400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48804199734bb0d8cd7c3acbc6d13b6081ffb975eed61ed44ed2e224edb57f19`  
		Last Modified: Thu, 12 Jan 2023 23:27:22 GMT  
		Size: 104.0 MB (104015431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790366988bec99064529cc4474b7f53f27ffe8c92d9cef9567b6a4740afebd34`  
		Last Modified: Thu, 12 Jan 2023 23:27:05 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:galactic-ros-core` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:0171d2f071497cb534f22bcb84621189b998e00d8464f3e982c2b8ea82f60f85
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134318720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84c4d6c10dbb74ff3e6bcd101682868a4bca2b4eac97494bacd17ade98245e2`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:43:45 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 02:43:50 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 22:47:38 GMT
RUN echo "deb http://snapshots.ros.org/galactic/final/ubuntu focal main" > /etc/apt/sources.list.d/ros2-snapshots.list
# Thu, 12 Jan 2023 22:47:40 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 4B63CF8FDE49746E98FA01DDAD19BAB3CBF125EA
# Thu, 12 Jan 2023 22:47:40 GMT
ENV LANG=C.UTF-8
# Thu, 12 Jan 2023 22:47:40 GMT
ENV LC_ALL=C.UTF-8
# Thu, 12 Jan 2023 22:47:40 GMT
ENV ROS_DISTRO=galactic
# Thu, 12 Jan 2023 22:49:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-galactic-ros-core=0.9.3-2*     && rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 22:49:46 GMT
COPY file:ec5b16a0e777d7d7d041a72ffc817bf5f7b375662afa0c404f3ca36fad1afb90 in / 
# Thu, 12 Jan 2023 22:49:46 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 12 Jan 2023 22:49:47 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757fb2fe2f280d64cc7c0734dadd7f72dfcd73d70d14dce449f6ec2e6834b66f`  
		Last Modified: Fri, 09 Dec 2022 03:22:59 GMT  
		Size: 1.2 MB (1154754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34108aa9b6e179025d554465ed41e434532d83865bdc22a0b4ea074748d69d1e`  
		Last Modified: Fri, 09 Dec 2022 03:22:58 GMT  
		Size: 5.5 MB (5531057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7cf1cc80ad37b196dcfab47ce981ee43aee45d8adce1fe8783373db322f4f7`  
		Last Modified: Thu, 12 Jan 2023 22:54:45 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffc6fa3e2aa1aa444e384d7b35e8fb1c4b52228f2e538fd942fd1d04d68ff9e`  
		Last Modified: Thu, 12 Jan 2023 22:54:45 GMT  
		Size: 2.4 KB (2399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84dd4a45fa6f8dfc5845bfa1fba3da4f4b8ec7b350322177e531ef8e8123d5e`  
		Last Modified: Thu, 12 Jan 2023 22:54:58 GMT  
		Size: 100.4 MB (100436911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9512977316ac0bcb88c6cbcd892f02cea92cb2085b9bcebdfa1ee802d64fd09c`  
		Last Modified: Thu, 12 Jan 2023 22:54:45 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
