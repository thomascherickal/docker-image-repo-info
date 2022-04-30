## `ros:noetic-perception`

```console
$ docker pull ros@sha256:081de7652d14d7a7945d12ad41267e402373eee4ae18090a74cbc2a22e510ffd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception` - linux; amd64

```console
$ docker pull ros@sha256:9cefaefd8524b32205ec8b0df40cd45de57e93365ee78b9e22567aa4475f50c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.0 MB (834986382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3871f0e62ec582dc4a22518618e4656c040a163e1f2b836f79efdc7cff355363`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:39:00 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:00:47 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:00:47 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 30 Apr 2022 02:00:49 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 02:00:49 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 02:00:49 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 02:00:49 GMT
ENV ROS_DISTRO=noetic
# Sat, 30 Apr 2022 02:02:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:02:39 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 30 Apr 2022 02:02:39 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 02:02:39 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:03:01 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:03:06 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 30 Apr 2022 02:04:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:11:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca43c78a9071a3a99b9aa1fe030cf8ba61c96fbf0b12adc1a85163d395cc10a1`  
		Last Modified: Sat, 30 Apr 2022 00:50:22 GMT  
		Size: 1.2 MB (1180884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695af473b1cd9e144d20d270ac7db7c1e34126fdb27db717ef1b82d4ea459397`  
		Last Modified: Sat, 30 Apr 2022 02:23:44 GMT  
		Size: 5.5 MB (5546712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1815920971612fc5c835cf5dec6114490617c1748a4eb0cecfefb26fd382e87c`  
		Last Modified: Sat, 30 Apr 2022 02:23:44 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e5ac291e57ac17859a1197a02cef05c2ce653057367d8a2d96f922092ec30c`  
		Last Modified: Sat, 30 Apr 2022 02:23:44 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538340f9393d750734eb586fcf923aad47b40141e3a03f4c5cebd0c3e93a77eb`  
		Last Modified: Sat, 30 Apr 2022 02:24:12 GMT  
		Size: 176.9 MB (176870314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d73a3870c7d327c981c7e8aec2fe20e449f17a83adfbc7109fe0bea3a64152`  
		Last Modified: Sat, 30 Apr 2022 02:23:43 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb3bed1aea6e7ac72e4a19607318f5961c006d415b72e5cb2e7e88480085730`  
		Last Modified: Sat, 30 Apr 2022 02:24:30 GMT  
		Size: 50.9 MB (50933827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de4fa1d18550f1ca14eee9ea47facbc10d96703b5d8f8502661017b6a267476`  
		Last Modified: Sat, 30 Apr 2022 02:24:22 GMT  
		Size: 315.7 KB (315669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2833a9d1502a5693dada4f3a93339db0ffe0f1e44c7971ec1273bb2adab080`  
		Last Modified: Sat, 30 Apr 2022 02:24:34 GMT  
		Size: 79.6 MB (79602544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df61effbf04da7b21b51bdd0bd445dc1a844b3abc955afc042b7af9f5a0b0a10`  
		Last Modified: Sat, 30 Apr 2022 02:26:12 GMT  
		Size: 492.0 MB (491967789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm variant v7

```console
$ docker pull ros@sha256:732a9ce14f825cacefc32886651b9a23180a0f46ef47874a17d32205450628b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **725.6 MB (725587279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ce21f86b3137fa28a954f09289263b797c9a14a186dc78e041997dbdbfbc4e5`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:46 GMT
ADD file:5f12bea85a1ebe365907ca3979b0e31e6043dccfcb9a3cdf62be46e054494147 in / 
# Fri, 29 Apr 2022 22:58:47 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:39:04 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:39:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:39:23 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 30 Apr 2022 00:39:25 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 00:39:26 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 00:39:26 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 00:39:27 GMT
ENV ROS_DISTRO=noetic
# Sat, 30 Apr 2022 00:41:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:41:53 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 30 Apr 2022 00:41:53 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 00:41:54 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:42:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:42:50 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 30 Apr 2022 00:43:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:49:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b20724a4297c7ca8b89f31d6ad53e7ead0c17c7908a4592871cdc97332193580`  
		Last Modified: Fri, 29 Apr 2022 23:03:00 GMT  
		Size: 24.1 MB (24073650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788bc5672cc0168109c03624bd9c0486dc436058f2ef6bd58aa20183c16330dc`  
		Last Modified: Sat, 30 Apr 2022 00:58:13 GMT  
		Size: 1.2 MB (1182235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02f050457c70471d51e645d9056bf76421874818d4dcb3c2d9167cc4c7c59f1`  
		Last Modified: Sat, 30 Apr 2022 00:58:12 GMT  
		Size: 4.7 MB (4676780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf102ed76521e041cbd91514e5b37b5e35694a768c899009f51ba52983b3d4d`  
		Last Modified: Sat, 30 Apr 2022 00:58:10 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b493804b771bd37872f55298ac60b41ddb64199e41c6cbd02a5bd78b13f2e17`  
		Last Modified: Sat, 30 Apr 2022 00:58:10 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf0953c9382836b5d5e61b0e28e2f23c2431ef644d2ddc2d4a5bffbadff9b15`  
		Last Modified: Sat, 30 Apr 2022 01:00:16 GMT  
		Size: 157.4 MB (157423830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5012cfe0e5842d29eb696b50431a424ba513d5c1554715f456713b05532596d`  
		Last Modified: Sat, 30 Apr 2022 00:58:10 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faae41d6b1935d771645ed3646ee3838471dd083a2f92d29b121834b2a712fab`  
		Last Modified: Sat, 30 Apr 2022 01:00:51 GMT  
		Size: 40.5 MB (40501299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dea40ff78bf9cdbb2384fb35a4bb7127dac17db236f078dcc3d9de59148a06`  
		Last Modified: Sat, 30 Apr 2022 01:00:28 GMT  
		Size: 315.7 KB (315673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d375b84b753999e87a8ed0b405d15fd34c522a1f831031dad0599a36d2f84491`  
		Last Modified: Sat, 30 Apr 2022 01:01:07 GMT  
		Size: 60.5 MB (60481908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9dc52f71902d762b0a95cfa3c0abfc4606212d101bdb1102c56046907805949`  
		Last Modified: Sat, 30 Apr 2022 01:06:14 GMT  
		Size: 436.9 MB (436929489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:37cba6b7529f06b540518f6797f71750191abcc4d1839510c6b82cf8d9d314b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.5 MB (784517811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:081f48272fe65c5d6151746f56f2f4d30a39cbbb9177a73868d875d2ca4e4533`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:20:30 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:20:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:20:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 30 Apr 2022 00:20:43 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 30 Apr 2022 00:20:44 GMT
ENV LANG=C.UTF-8
# Sat, 30 Apr 2022 00:20:45 GMT
ENV LC_ALL=C.UTF-8
# Sat, 30 Apr 2022 00:20:46 GMT
ENV ROS_DISTRO=noetic
# Sat, 30 Apr 2022 00:21:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:21:44 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Sat, 30 Apr 2022 00:21:45 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 30 Apr 2022 00:21:47 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:22:20 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:22:25 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 30 Apr 2022 00:22:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:25:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2837428b54ca227343b28e2aebf5f943eb61317acb706203bbd53ccd36b1faa`  
		Last Modified: Sat, 30 Apr 2022 00:38:20 GMT  
		Size: 1.2 MB (1182149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782caaf301f52c6f48c207e662cbaff846f5e221ff2d301aa5123d59be9f9cdc`  
		Last Modified: Sat, 30 Apr 2022 00:38:18 GMT  
		Size: 5.3 MB (5321931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd1a842c5f450bf757d4efae2d77d0b3637b2f76a02794282656ef03f45e1f1`  
		Last Modified: Sat, 30 Apr 2022 00:38:18 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e026a627567dcb9c599ab69248d8c084364d4df165bc5257f923c2709f493ab`  
		Last Modified: Sat, 30 Apr 2022 00:38:17 GMT  
		Size: 1.9 KB (1944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a527d513e9f97294799a5126bcf25e7f7b73ff93ceb27622f1b3838d580fcde9`  
		Last Modified: Sat, 30 Apr 2022 00:38:47 GMT  
		Size: 171.3 MB (171293442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc48433487f9d4e46329a07c1247899a65bab17103180e95e2da17c25f686d5`  
		Last Modified: Sat, 30 Apr 2022 00:38:17 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9776aee7c7d20a2a679ec671b31130800b8048248586171aa655e89df4b91f4a`  
		Last Modified: Sat, 30 Apr 2022 00:39:05 GMT  
		Size: 45.0 MB (44988594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890ccdeaa4aedd37f00917bbddd6365cd5dc7f1746a97c5520462003cccd6b3a`  
		Last Modified: Sat, 30 Apr 2022 00:38:58 GMT  
		Size: 315.6 KB (315611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8b7144add68575402586085ccee53c0002fd54ef7e2813f589098a7cce933e`  
		Last Modified: Sat, 30 Apr 2022 00:39:09 GMT  
		Size: 71.8 MB (71753617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f15a8b59ed9e76d31ca016fba28201e39c0b6f21f48212025ce82ac5a9162a0`  
		Last Modified: Sat, 30 Apr 2022 00:40:47 GMT  
		Size: 462.5 MB (462490713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
