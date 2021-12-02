## `ros:noetic-ros-core-buster`

```console
$ docker pull ros@sha256:147106b8c9e55d4db6acade7406e8e0ab109a658d5cfa1a6091a20bce3ae5a40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `ros:noetic-ros-core-buster` - linux; amd64

```console
$ docker pull ros@sha256:747edb277b85b1f91527abfc6e8605421d4d3ef3ad182935544515bd86c0bf01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.4 MB (300417508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b77b2e243fd1ddbb99163e0ddc534aae92cce608c45592f437f01dd1121b05b`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:31 GMT
ADD file:f077e1a42fb919be2af67820782ceee3b46ffd13d7ab6949bea9921217d12813 in / 
# Thu, 02 Dec 2021 02:48:32 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:36:34 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:36:35 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Dec 2021 17:36:42 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Dec 2021 17:36:42 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 17:36:42 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Dec 2021 17:36:42 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Dec 2021 17:38:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:38:12 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 02 Dec 2021 17:38:13 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Dec 2021 17:38:13 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c4cc477c22ba7abce860198107408434dd7bd73ddbaf82f1e69ab941b9979405`  
		Last Modified: Thu, 02 Dec 2021 02:54:07 GMT  
		Size: 50.4 MB (50437113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0d27c0bb5c1a8e650467428d5b560f993c0bad524a2467341f4cacf7271bbf`  
		Last Modified: Thu, 02 Dec 2021 17:44:38 GMT  
		Size: 10.9 MB (10891906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2c6185cd0bc5d1c21571501b856e5450c1278d6cd97f3e28dc28761992bef1`  
		Last Modified: Thu, 02 Dec 2021 17:44:37 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973fda33325f33a869db336e1d0f9a03409932db709b37c54e2732d7405c338b`  
		Last Modified: Thu, 02 Dec 2021 17:44:37 GMT  
		Size: 2.0 KB (1991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ac5ff5b2ed72b39d61b4408c6423b2989711475b64022bb5ebbda5a60ff157`  
		Last Modified: Thu, 02 Dec 2021 17:45:15 GMT  
		Size: 239.1 MB (239086073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3acd7fde20a8702e863ddbe045987e72bc6fa11bf0d5524b344d7c0207b140`  
		Last Modified: Thu, 02 Dec 2021 17:44:37 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-ros-core-buster` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:a8fb3f5cd851acbd8709afda777515f2333c9ccb3fb689176b71bcf1d1a38551
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.2 MB (244215029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fcc8d12e363caeadad4015fdfa946ab9074370766cdc836909e980add4fe3d0`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:20 GMT
ADD file:82c1819d8416d9d44564980e25e98a081f813bc2ee8ad2789114fe37e802848f in / 
# Thu, 02 Dec 2021 08:08:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:09:40 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 14:09:41 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu buster main" > /etc/apt/sources.list.d/ros1-latest.list
# Thu, 02 Dec 2021 14:09:48 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Thu, 02 Dec 2021 14:09:49 GMT
ENV LANG=C.UTF-8
# Thu, 02 Dec 2021 14:09:50 GMT
ENV LC_ALL=C.UTF-8
# Thu, 02 Dec 2021 14:09:51 GMT
ENV ROS_DISTRO=noetic
# Thu, 02 Dec 2021 14:10:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 14:10:56 GMT
COPY file:cbbaa0f5d6a276512315f5b4d7347e94a120cefbda9058ebb0d678847ff4837f in / 
# Thu, 02 Dec 2021 14:10:58 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Thu, 02 Dec 2021 14:10:59 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:39e4f823356a9e2dbba530f9d363b4d76beaff75a13bad788d38eebeae67e5b0`  
		Last Modified: Thu, 02 Dec 2021 08:41:08 GMT  
		Size: 49.2 MB (49223045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e8f1f129dad6b169099626334d47f33bb82f4b4bb0546404f0e3ff9f29f589`  
		Last Modified: Thu, 02 Dec 2021 14:18:09 GMT  
		Size: 10.7 MB (10688015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a995ef6e0affa0efea1e9bab7ccb010f6b50dc0dd518f955224c42c80ca4625`  
		Last Modified: Thu, 02 Dec 2021 14:18:07 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1a144f0e750af7280088604a588b33ca097d137deb1e9c165832bcc112ff12`  
		Last Modified: Thu, 02 Dec 2021 14:18:07 GMT  
		Size: 1.9 KB (1948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509ff02a2b334915606915d72debb67ed7feaef6ab150ded7a474ed2a3847bab`  
		Last Modified: Thu, 02 Dec 2021 14:18:39 GMT  
		Size: 184.3 MB (184301599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4546300f0a7a750dcd6fdf3c875bbd66d4444983e525a6fab1105911104a496`  
		Last Modified: Thu, 02 Dec 2021 14:18:08 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
