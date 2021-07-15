## `ros:noetic-robot-buster`

```console
$ docker pull ros@sha256:d3c2c83940885aa9fc2d2f1f477022dfb06d7b3b8982a22f5bef51d78432c076
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-robot-buster` - linux; amd64

```console
$ docker pull ros@sha256:ffcbf02b129bfb3faa964d9f10e97f1cc501435a4c1fd3747a5bf0378e438498
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.4 MB (484437125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d30dabe6f695c3c478711677f35aeb261300c2420b136bb31d816d2378d2720`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:54:04 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:54:05 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 23 Jun 2021 16:54:07 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 23 Jun 2021 16:54:07 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 16:54:07 GMT
ENV LC_ALL=C.UTF-8
# Wed, 23 Jun 2021 16:54:07 GMT
ENV ROS_DISTRO=noetic
# Wed, 23 Jun 2021 16:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:55:11 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 23 Jun 2021 16:55:11 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 23 Jun 2021 16:55:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:55:43 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:55:48 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 23 Jun 2021 16:56:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 16:56:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368710b5d60bd3571596105db24587dc7641662961cd8565f0ab308ea71c8716`  
		Last Modified: Wed, 23 Jun 2021 17:00:59 GMT  
		Size: 10.9 MB (10891785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c851fa0b21cd231e582f810f8c19cefe3e82acfd0b381ee63df5ad2ea6d405`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d911fa207ab982f2d18b595a9cbd025da0e7d7b99a38329c00d496ae74e5c57`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf3cb86fc6e74480b1bed2f10d298288eaef33b5c4a44e36c5723bed2d7d603`  
		Last Modified: Wed, 23 Jun 2021 17:01:36 GMT  
		Size: 239.0 MB (239043542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6807ff55dd30ea5a41adf5345578639e51e44f6cac1d76453af573795d8367d9`  
		Last Modified: Wed, 23 Jun 2021 17:00:57 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda640c7cc970da7dc489bbd348f6d10ca8aadea00bb348b143454fef3f798f1`  
		Last Modified: Wed, 23 Jun 2021 17:01:59 GMT  
		Size: 86.6 MB (86566646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6b8e0c86f409efb0b6383db70437892d4daca00797115f65c9c22a2ed27322`  
		Last Modified: Wed, 23 Jun 2021 17:01:45 GMT  
		Size: 302.4 KB (302359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aeca0ec3c658ebff801eb589b5d7083dafb559be63ecbf3a4f0ed4cb127398`  
		Last Modified: Wed, 23 Jun 2021 17:02:00 GMT  
		Size: 76.0 MB (75974809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228c8ed43e25be90ca823b4c143449a5b504b22c238a1ddc117569532f373d5`  
		Last Modified: Wed, 23 Jun 2021 17:02:11 GMT  
		Size: 21.2 MB (21219955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:f3a211482cd13444032d6e0fd52b1ed4cda50d89bedb91082fa3dc0ed773415a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.0 MB (423977337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5c76dcf42f26e71f7f4551754bed4945433dfa588ec12a4065360e0454d8eb8`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:34:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:34:34 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Wed, 23 Jun 2021 12:34:36 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Wed, 23 Jun 2021 12:34:36 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 12:34:36 GMT
ENV LC_ALL=C.UTF-8
# Wed, 23 Jun 2021 12:34:36 GMT
ENV ROS_DISTRO=noetic
# Wed, 23 Jun 2021 12:35:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:35:36 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Wed, 23 Jun 2021 12:35:36 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Wed, 23 Jun 2021 12:35:37 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:35:57 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:36:08 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Wed, 23 Jun 2021 12:36:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:36:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a6d0fd3d166254b7e229d1f59f216a508567a9850665d123014684e30eeb4c`  
		Last Modified: Wed, 23 Jun 2021 12:42:27 GMT  
		Size: 10.9 MB (10883414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a054e7e8c0b332fb66dc5088973cbcb57d8a1ce5e8249443fef3856a708478`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee9c05970568fc6fe659f9305867a4b6425bed7f4237de3516cf3dc553f0238`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df81d3dac71b04be5d0a51a53296f7f7dd6d0aa6d6387c7229191cb57889b58`  
		Last Modified: Wed, 23 Jun 2021 12:43:01 GMT  
		Size: 184.2 MB (184226666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce9ec19f2ee8191d40e2ceea8d6bd89e9e0f8133c049808b0548557b9b71f65`  
		Last Modified: Wed, 23 Jun 2021 12:42:26 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b320ffadbb584163174053ad9da711044b8679fc2a8de068ee4732f53449edec`  
		Last Modified: Wed, 23 Jun 2021 12:43:23 GMT  
		Size: 84.4 MB (84357037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9607df761ad999a479ca2c254d645b6cc0426d0805ed9e5106482e2eb75b334`  
		Last Modified: Wed, 23 Jun 2021 12:43:10 GMT  
		Size: 302.1 KB (302127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6589ea28fd69f1bbfdce955f0e3598a503017bc915334e4405b7373d17320b8`  
		Last Modified: Wed, 23 Jun 2021 12:43:21 GMT  
		Size: 74.1 MB (74088042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d77fdf0e185059de6a2bcdc1db66a1eecaab06ef847415856f281d4b94575`  
		Last Modified: Wed, 23 Jun 2021 12:43:34 GMT  
		Size: 20.9 MB (20895648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
