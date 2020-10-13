## `ros:melodic-perception-stretch`

```console
$ docker pull ros@sha256:509d48f599def7d063e18225302ce1c7a781ba954ec71b3820fe34075c652289
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:melodic-perception-stretch` - linux; amd64

```console
$ docker pull ros@sha256:e89d55fc3a3f18eeb7953c337b972eb4ce1cdbfa96ec95571a1385b1570827ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **828.4 MB (828377319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e78ce91a92378fd8884936607bfc04b7c1dd10b821aac61baf169b5654b5e6`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:13 GMT
ADD file:a8742c34bf12f231279dd5086b8ec1310224c740a95170b916217f22a68eb9a7 in / 
# Tue, 13 Oct 2020 01:44:13 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 19:17:42 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 19:17:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 13 Oct 2020 19:17:46 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 13 Oct 2020 19:17:46 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 19:17:46 GMT
ENV LC_ALL=C.UTF-8
# Tue, 13 Oct 2020 19:17:46 GMT
ENV ROS_DISTRO=melodic
# Tue, 13 Oct 2020 19:19:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 19:19:18 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 13 Oct 2020 19:19:19 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 13 Oct 2020 19:19:19 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 19:20:06 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 19:20:19 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 13 Oct 2020 19:20:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 19:23:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0400ac8f7460260a663e0e97c24d7dfd8a2c947736f0351752b45c53e26d6e02`  
		Last Modified: Tue, 13 Oct 2020 01:50:49 GMT  
		Size: 45.4 MB (45366778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e64d6a7fc5320867400c03832cf54957cbbf98b99714a200a9090f67fa0af6`  
		Last Modified: Tue, 13 Oct 2020 19:32:22 GMT  
		Size: 6.9 MB (6866999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868ec983be87cbebfea0a9dea300e1ae958cdc96a8fd550ed6ba63ceeed46116`  
		Last Modified: Tue, 13 Oct 2020 19:32:19 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7303450037ec364ecd0bff523fa0140a41fbc939b44bcb48abe60b9fe2d1fdc4`  
		Last Modified: Tue, 13 Oct 2020 19:32:19 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04058250f482c63226262abef7876d3f158f937c4535066c3bacf84b047b5f9c`  
		Last Modified: Tue, 13 Oct 2020 19:33:29 GMT  
		Size: 269.9 MB (269927678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876e825fea60d421a44ae42f1fb98d96cf6acdcf20af70678fd093ce7bc7211a`  
		Last Modified: Tue, 13 Oct 2020 19:32:19 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b3345f7bb5574ca7d580696fd7f3e8c218a503004f3eff3679e6b29efee8f4`  
		Last Modified: Tue, 13 Oct 2020 19:33:51 GMT  
		Size: 70.2 MB (70152916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad59a685afc6f0c271459de511b5c166bbced15374a2f8482920687c0181f415`  
		Last Modified: Tue, 13 Oct 2020 19:33:35 GMT  
		Size: 264.6 KB (264554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d8e96833fe2accef120b31842c4fd2a18a1f5f4685b04fe0b84ae6cbffde54`  
		Last Modified: Tue, 13 Oct 2020 19:33:49 GMT  
		Size: 55.1 MB (55053833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e887dd3df366bde99746c94f6ec85d2c55d07d4a13159923eb457b95e61683`  
		Last Modified: Tue, 13 Oct 2020 19:35:52 GMT  
		Size: 380.7 MB (380742746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:melodic-perception-stretch` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:12309f25a32a75529e29391dbc7f65033c258b12cbc92c366518882c7dab754e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **749.6 MB (749649633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:868ebfb6168851804067e4a53b58bfd8cc95b542713fc9ec96d1c828f5c853b3`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:43:49 GMT
ADD file:2752d391988f4ad7e086be863c36a83a3226e31e44ea816ca4c89d6a410727b1 in / 
# Tue, 13 Oct 2020 01:43:51 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 20:25:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 20:26:03 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Tue, 13 Oct 2020 20:26:19 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu stretch main" > /etc/apt/sources.list.d/ros1-latest.list
# Tue, 13 Oct 2020 20:26:33 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 20:26:36 GMT
ENV LC_ALL=C.UTF-8
# Tue, 13 Oct 2020 20:26:37 GMT
ENV ROS_DISTRO=melodic
# Tue, 13 Oct 2020 20:30:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-core=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 20:30:31 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Tue, 13 Oct 2020 20:30:32 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Tue, 13 Oct 2020 20:30:34 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 20:31:16 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python-rosdep     python-rosinstall     python-vcstools     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 20:31:32 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Tue, 13 Oct 2020 20:32:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-ros-base=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 20:38:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-melodic-perception=1.4.1-0*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:19e4d0e7f8f2c5cb8a0a8d0e741e9e387c34bd673da69cdcc8e758a5c4dbc106`  
		Last Modified: Tue, 13 Oct 2020 01:50:49 GMT  
		Size: 43.2 MB (43171543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0402e367b1600701da7026f5f2695c1dcf2613f4475210c5eefba2407e46e659`  
		Last Modified: Tue, 13 Oct 2020 20:56:16 GMT  
		Size: 6.4 MB (6440970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab2f165c86fef2d3d9e6ed4625300e11f3521c1b8b77e24735220e04599238c`  
		Last Modified: Tue, 13 Oct 2020 20:56:14 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a9e42ef2a29448e094d94ca77e61b1f92bbfbf407d338f8eac6ad88d7da11e`  
		Last Modified: Tue, 13 Oct 2020 20:56:15 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3201da69b0b08991ef885c5ea5daa481f9857374da40094e2fc1a63db5b7217e`  
		Last Modified: Tue, 13 Oct 2020 20:57:45 GMT  
		Size: 225.0 MB (225025090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8955121c7c004304a497f3fe0a562986a606d96a42df243a8b44dd2dab75c5a5`  
		Last Modified: Tue, 13 Oct 2020 20:56:15 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc4621d2ad4ed86ced93a9ad1c96e466ba3ba045e7346968e6c21e36a2a18ca`  
		Last Modified: Tue, 13 Oct 2020 20:58:29 GMT  
		Size: 64.8 MB (64842121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e32a4e1b3cc105841587ef4683b70e0aa443476b7d864dc6b63854f4794ab6`  
		Last Modified: Tue, 13 Oct 2020 20:58:09 GMT  
		Size: 264.6 KB (264611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc0efff98b5d8aef4ca1fe47204ef2cfadcf9b37cea0957e749e87a7309ae00`  
		Last Modified: Tue, 13 Oct 2020 20:58:27 GMT  
		Size: 53.2 MB (53242676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3dd57602d3208e2d7d6a365c17653c82fdf6e01e82d9a5aad047ba9844796dc`  
		Last Modified: Tue, 13 Oct 2020 21:00:35 GMT  
		Size: 356.7 MB (356660799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
