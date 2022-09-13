## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:803c1a3241eb27ba8152897265a35e60969edb6960690579e46fe10278cc8711
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:c51ebbf0745f509ade1bc49ca105819df54df7253d6f4f4b5adfeb9de560c7b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300632469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:310a552d1d9c68ac645cbaf4134573a401cd9b5524b6aef6abc65bc65932ed83`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:38 GMT
ADD file:4649a893b2859f2ff51182a13c9c8eeaeaea866161b3f4a1c4f0bb48bc01d007 in / 
# Tue, 13 Sep 2022 00:56:38 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 12:21:19 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:21:20 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 13 Sep 2022 12:21:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 13 Sep 2022 12:21:22 GMT
ENV LANG=C.UTF-8
# Tue, 13 Sep 2022 12:21:22 GMT
ENV LC_ALL=C.UTF-8
# Tue, 13 Sep 2022 12:21:22 GMT
ENV ROS_DISTRO=noetic
# Tue, 13 Sep 2022 12:22:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:22:32 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 13 Sep 2022 12:22:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 13 Sep 2022 12:22:32 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:86467c57892b6bb48d563cb5940c68b69c431b2e79c3547df60d1c761c21c156`  
		Last Modified: Tue, 13 Sep 2022 01:00:51 GMT  
		Size: 50.4 MB (50440374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf49330e6dcf4631b745f36390b6924eb52faae3ca4914217e00162bc6c68356`  
		Last Modified: Tue, 13 Sep 2022 12:28:00 GMT  
		Size: 10.9 MB (10893556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6b84e60758dcc196c2a43988dc174dd7bd73986a0b408d81c15f2e4a6e0175`  
		Last Modified: Tue, 13 Sep 2022 12:27:59 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cdeac817655f3902a59a9aaba2a64e30b481f0d568014ad88b358c952c86b7`  
		Last Modified: Tue, 13 Sep 2022 12:27:59 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755c74d4c66edd4c0e0ef512b7283105748b0bb49535591e26bdcdbd0da47303`  
		Last Modified: Tue, 13 Sep 2022 12:28:32 GMT  
		Size: 239.3 MB (239296126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d4c11830d9370e64c516d2974473ec5b9d5e51353531304367a1150f122ff`  
		Last Modified: Tue, 13 Sep 2022 12:27:59 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:687fee6b2af63282d4dbe53efdda56050275871d83d939268c2cea363b9bdc05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.4 MB (244382992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b08dd03d0f694d4725f4b54758825a8aa653d29108aed76c46cf6e32caec47e0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:06 GMT
ADD file:304a544562f139d7ab96511b7f1e059966cf90169117e835072f132468bf91c8 in / 
# Tue, 13 Sep 2022 02:11:07 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 12:56:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:56:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 13 Sep 2022 12:56:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 13 Sep 2022 12:56:44 GMT
ENV LANG=C.UTF-8
# Tue, 13 Sep 2022 12:56:45 GMT
ENV LC_ALL=C.UTF-8
# Tue, 13 Sep 2022 12:56:46 GMT
ENV ROS_DISTRO=noetic
# Tue, 13 Sep 2022 12:58:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:58:13 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Tue, 13 Sep 2022 12:58:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 13 Sep 2022 12:58:16 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:e2406a452ad23ba9085e0708f5e15309206a618eb828aa307becbb239414392f`  
		Last Modified: Tue, 13 Sep 2022 02:16:42 GMT  
		Size: 49.2 MB (49228261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ec060bafb85a1c4fb32a456ed970628f926c8b985fb90ed243d4c7d4d96d6f`  
		Last Modified: Tue, 13 Sep 2022 13:06:39 GMT  
		Size: 10.7 MB (10689346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f272eefce84866a380e21ef07b830d72077f566702b1dc8432c9bd460423b18`  
		Last Modified: Tue, 13 Sep 2022 13:06:37 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4d36aa5f5718c160f03a683078a7a6a33c621f22763243a6cba5a31fec922`  
		Last Modified: Tue, 13 Sep 2022 13:06:37 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c4b761086d86c468aad5c1c5a5a8b2904284754e9efa06d510edcc4b50a638`  
		Last Modified: Tue, 13 Sep 2022 13:07:08 GMT  
		Size: 184.5 MB (184463015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15616e1c2e135cd3c48087cab44685dcd6953ceeb63f92b3ae64f09578961f44`  
		Last Modified: Tue, 13 Sep 2022 13:06:37 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
