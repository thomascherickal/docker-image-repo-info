## `ros:melodic-ros-core-bionic`

```console
$ docker pull ros@sha256:16384805bb6a985e6af821e696f9661c55cb2f79ab3f37001d4013045de89da4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:melodic-ros-core-bionic` - linux; amd64

```console
$ docker pull ros@sha256:7993411bf869c56bcae9dfe1f3e7250822ec1312e7c6d22f0e16e41de11974e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.9 MB (291895426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e79425a7677bf6ffcffe61661c336ad245d7181195bb16cbd6d7683d7e9ebe1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 05:30:26 GMT
ADD file:f554512cb0acad99508554656767804e4821ece488fac0e46fd2c643a39f7021 in / 
# Fri, 18 Mar 2022 05:30:27 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 09:07:51 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:07:58 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 09:08:26 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 09:08:26 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 09:12:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 09:13:02 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 09:13:02 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 09:13:02 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:11323ed2c65349758e68a03a8e43825ec263dc9790daea93cf83b18ad0703109`  
		Last Modified: Thu, 17 Mar 2022 11:55:05 GMT  
		Size: 26.7 MB (26708634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed186fe30ca85957e7e878753de089d2e8a5010dea43d74e99fb9771929b361`  
		Last Modified: Fri, 18 Mar 2022 09:59:31 GMT  
		Size: 839.0 KB (838975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac38668a25e5c8cb5f52e0ffdd479b065a5b768f641384a77a9dad0e5e3a452`  
		Last Modified: Fri, 18 Mar 2022 09:59:29 GMT  
		Size: 4.9 MB (4872095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3121bbb0fedc1e2db1e5b93f19539efa4d73a3d2e13dc6383e07e5f8307e18d4`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74eff7c67bd61ade3c431ca761f80a2ca2e92c123b438fc182703230d41f6d8`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f141a0064ed4688cdba0e30eb81c5f5cc6461474bf113cf9d86b369552eb1247`  
		Last Modified: Fri, 18 Mar 2022 10:00:13 GMT  
		Size: 259.5 MB (259473309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e5e41cd901de4d480b01b31605bb094d3495205a16373e06e5ecc7af3e7486`  
		Last Modified: Fri, 18 Mar 2022 09:59:28 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm variant v7

```console
$ docker pull ros@sha256:89a7740d73bfb9f34a943f770d2b2392e5381bcc607c2733031088253afd66df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266180488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d371ee251ec4166d9475e5957cbd74ddfb69fffa55dc10c60f40a6d581e608b8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:32:19 GMT
ADD file:05014e7be574a8703e7ca668f8ff20d708f1860234bc44e3ef9e9a15193ea2c2 in / 
# Fri, 18 Mar 2022 07:32:19 GMT
CMD ["bash"]
# Sun, 20 Mar 2022 06:49:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:49:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Sun, 20 Mar 2022 06:49:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LANG=C.UTF-8
# Sun, 20 Mar 2022 06:49:37 GMT
ENV LC_ALL=C.UTF-8
# Sun, 20 Mar 2022 06:49:38 GMT
ENV ROS_DISTRO=melodic
# Sun, 20 Mar 2022 06:52:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 06:52:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sun, 20 Mar 2022 06:52:54 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sun, 20 Mar 2022 06:52:54 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:d423dfb8c4fe22914d518a0a7c648903c4159e75b2ddd41c2d7dd27c5af71078`  
		Last Modified: Fri, 18 Mar 2022 07:35:55 GMT  
		Size: 22.3 MB (22308133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0309665cde8260b163c9e436387ea06be877b3c887a1365db723b937d1ac8fc`  
		Last Modified: Sun, 20 Mar 2022 07:13:01 GMT  
		Size: 840.0 KB (840016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0593d08dd549efcc955de18967872b207c683a278c5586dcb9a577891dc9c1d7`  
		Last Modified: Sun, 20 Mar 2022 07:13:00 GMT  
		Size: 4.1 MB (4085989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85ed4b7d5f241ebe3379b98be689c55f2e918de69df9dc49c35e2e22acc881d`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b147465263ff3ff695ba9e407284cd9970d44fd30518ac19b0734e913f245a1`  
		Last Modified: Sun, 20 Mar 2022 07:12:58 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877fa07064d973f881e0f26b3e7112a8203d28c75ceb36b4c3ce788525211152`  
		Last Modified: Sun, 20 Mar 2022 07:15:34 GMT  
		Size: 238.9 MB (238943937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc7436df57dde7519ce798a787f16a185dd05890111d2c5df42e48f19ad9750`  
		Last Modified: Sun, 20 Mar 2022 07:12:59 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-ros-core-bionic` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:87be3317cb2a6134c2086e2edbd7a5e25d0a7b2bec4dfceaec14089a1805a6fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.2 MB (281202378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c2d2946360479912556ac17a20d97a2e632ce0514f992d7857a16f9b13e61d`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:44 GMT
ADD file:3fc0139579b748872ad588bc76190747b882f6e343893c0f6e6983542ce089b9 in / 
# Fri, 18 Mar 2022 00:40:44 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 00:43:58 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:07 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:44:08 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu bionic main" > /etc/apt/sources.list.d/ros1-latest.list
# Fri, 18 Mar 2022 00:44:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Fri, 18 Mar 2022 00:44:50 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 00:44:51 GMT
ENV LC_ALL=C.UTF-8
# Fri, 18 Mar 2022 00:44:52 GMT
ENV ROS_DISTRO=melodic
# Fri, 18 Mar 2022 00:46:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 00:46:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Fri, 18 Mar 2022 00:46:20 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Fri, 18 Mar 2022 00:46:21 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:a0bce69069710cd1ada634950a38f397db06a36de45b4132a5ca244df440bc2e`  
		Last Modified: Fri, 18 Mar 2022 00:42:18 GMT  
		Size: 23.7 MB (23729104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3ab66e8231603adb03d0ab793fb0e59972981a99ffc720e57c383f793946d1`  
		Last Modified: Fri, 18 Mar 2022 01:19:05 GMT  
		Size: 839.7 KB (839706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205e19bfaf7b34cc3a9b24062d2decf853a9385f3fef4d92087fb5f722c192f`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 4.3 MB (4264013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ecfed1d8156c3c766d1cf52767451b94c4bddebf47c6077a252748e8a8efe14`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944bedb1f36c611f0fb39e835b936986f1dff2992e5b1af78dd788f93c8935ec`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01676100b2c71e8cba083dac9fa5b52bcc5bb6ce3e9f6aa8e7df42107bee34ab`  
		Last Modified: Fri, 18 Mar 2022 01:19:38 GMT  
		Size: 252.4 MB (252367186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fbf59c647844e4d4b6adb832d7aa654d99f008356bfa2e20f9326b02133b43`  
		Last Modified: Fri, 18 Mar 2022 01:19:03 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
