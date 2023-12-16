## `ros:noetic-perception-focal`

```console
$ docker pull ros@sha256:e9a5a7e01c331f8ec1c330798ba0df669915dbc7ce9a0d4fe0702b6c208b6922
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-perception-focal` - linux; amd64

```console
$ docker pull ros@sha256:fa708c31c015be5e78e4a9bda39a726156b361020acf035d80c06076bbfab9b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **835.2 MB (835231372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73475f3f165b59772361e2ba0e88a3d134affb9861987f02e34850b7a7e8cda1`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:27:43 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:27:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:27:44 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:27:45 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Wed, 13 Dec 2023 10:27:45 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:35:28 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:44 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:35:45 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:35:45 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:35:46 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:38:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:08 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:38:09 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:38:09 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:38:39 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:45 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:40:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:46:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:521f275cc58bdab90307a5929f8a6d197368b8c214edbc7f06fc1aaf48cfff3e`  
		Last Modified: Wed, 13 Dec 2023 14:46:20 GMT  
		Size: 28.6 MB (28584024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0425e951c42dd00ccb058ef6938f79b69db58bf09271ae9462bd5852cfd1353c`  
		Last Modified: Sat, 16 Dec 2023 10:05:10 GMT  
		Size: 1.2 MB (1198846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42aba2266c05b2025e53b1daad133978c157924dd56b92b27baac4c2b131ac49`  
		Last Modified: Sat, 16 Dec 2023 10:05:08 GMT  
		Size: 5.6 MB (5553944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da082b0fcdb0e926380c93badeb52429200982b64c2886589a087e11ada6826`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bc03d4300aebd1e01a1bbb2281172eee19cd2e9729ff0035fb2504dc536e32`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307477be25c4a96d631a6b63babb9347b6135862ce19b60048cbff55c280d179`  
		Last Modified: Sat, 16 Dec 2023 10:05:35 GMT  
		Size: 177.0 MB (176962968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db26ad757af2ab1db77cea22c3559b1a93d8efa9890510f708a7fe05c28f5fe2`  
		Last Modified: Sat, 16 Dec 2023 10:05:07 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b296290a0b7485d1f8672c8bd730f9a988374c02b9aa1b44d426683e13463e`  
		Last Modified: Sat, 16 Dec 2023 10:05:52 GMT  
		Size: 50.9 MB (50941170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c97955e78d4b5d35849ebaa6e03664552e66de89a179f90cb181e5682e4cdfa`  
		Last Modified: Sat, 16 Dec 2023 10:05:44 GMT  
		Size: 311.3 KB (311298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8991dddd9b2f661c7710e6ccb2cf128eb8c80547efb3b8a1a3d9252155c0ea81`  
		Last Modified: Sat, 16 Dec 2023 10:05:55 GMT  
		Size: 79.6 MB (79616327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccf1510df268376694568f812f9f639b378476209ab0731483dab043b2500fc`  
		Last Modified: Sat, 16 Dec 2023 10:07:26 GMT  
		Size: 492.1 MB (492060388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm variant v7

```console
$ docker pull ros@sha256:0e23576a6710c1d26a02e2b4393d24e92cedb7b6ba7f35882b840897ccad15df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **726.3 MB (726265125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:351c4ffb7f029799e927a50613997af5468eb27ce8afd706c940e49b5290ab61`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:37:05 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:37:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:37:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:37:06 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:37:14 GMT
ADD file:195375389d64193c828c6d3f379c7e35ea85256eb1c51d2bfeab73432ea46064 in / 
# Wed, 13 Dec 2023 10:37:15 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 09:37:52 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:37:58 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:38:00 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 09:38:00 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 09:38:00 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 09:40:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:14 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 09:40:14 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 09:40:14 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 09:40:36 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:40:42 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 09:42:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 09:49:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba68304511cfd178c72d64196a05b1343fbdbed6093d7b4db0c0d223510c40ab`  
		Last Modified: Sat, 16 Dec 2023 09:27:50 GMT  
		Size: 24.6 MB (24600972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5373ad55d8e8c0ab26bca9b592d8809358e69e59cff53121bcdd908a9f9639c`  
		Last Modified: Sat, 16 Dec 2023 09:50:09 GMT  
		Size: 1.2 MB (1199062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc25b246e660d5421dff1c723cfa2d5dfaa9c2ccfe1976b8fce4d4d1fedc8f5`  
		Last Modified: Sat, 16 Dec 2023 09:50:07 GMT  
		Size: 4.7 MB (4679510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb4107a21097c89ac49236bbde53efe45ed4c81f1e01e65c2f0358d02b73486`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70488c95ce2761e3460cec20b973e12284798d5b20d16b9009f4352584dafdc6`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecfe88b9d5bac2517d37b869da63ba8b7baa4f12ca28f6d66809dd278d3b48b`  
		Last Modified: Sat, 16 Dec 2023 09:50:35 GMT  
		Size: 157.5 MB (157458423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53b4028622de95be917a19e8013de1c97bde72b70b7382298556d8cf850713e`  
		Last Modified: Sat, 16 Dec 2023 09:50:06 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2341748b0485b9245a864429765e19ae950f9c356eb506df8d842670477ff2`  
		Last Modified: Sat, 16 Dec 2023 09:50:48 GMT  
		Size: 40.5 MB (40504005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660415962c143fc9e45d4e1c2054c79634e094b208c845bbd583cc003fa989b0`  
		Last Modified: Sat, 16 Dec 2023 09:50:43 GMT  
		Size: 311.3 KB (311302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5fd3825c19baab04ff606134bca9de817bb604a6b321072dc1193209a7d4a3`  
		Last Modified: Sat, 16 Dec 2023 09:50:52 GMT  
		Size: 60.5 MB (60499602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95d8a7cb341a7266eed7a5be48d80d9a87edab798791d784447db400dda8e0d`  
		Last Modified: Sat, 16 Dec 2023 09:52:15 GMT  
		Size: 437.0 MB (437009839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-perception-focal` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:961d74b9b4783ab58a163a3b04f673d19bf9a84959d4021c6348cd9c92488ef0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **785.5 MB (785526217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32a3ef3c7656107a98b411c2bd6415f2a92c0874fa2c890b76d18de3822f1805`
-	Entrypoint: `["\/ros_entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:29:33 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:29:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:29:34 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:29:41 GMT
ADD file:9ec8b7bbb2fbc8c90f1f24e19ab22130e03be1cc4727459e1265d2ed652377a1 in / 
# Wed, 13 Dec 2023 10:29:42 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 11:05:09 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:05:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:05:16 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
# Sat, 16 Dec 2023 11:05:16 GMT
RUN echo "deb http://packages.ros.org/ros/ubuntu focal main" > /etc/apt/sources.list.d/ros1-latest.list
# Sat, 16 Dec 2023 11:05:16 GMT
ENV LANG=C.UTF-8
# Sat, 16 Dec 2023 11:05:16 GMT
ENV LC_ALL=C.UTF-8
# Sat, 16 Dec 2023 11:05:16 GMT
ENV ROS_DISTRO=noetic
# Sat, 16 Dec 2023 11:07:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-core=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:07:30 GMT
COPY file:b48a3fff5008212a0bcdc238d0e8be930aa89d2336e357e1f628c98db523efeb in / 
# Sat, 16 Dec 2023 11:07:31 GMT
ENTRYPOINT ["/ros_entrypoint.sh"]
# Sat, 16 Dec 2023 11:07:31 GMT
CMD ["bash"]
# Sat, 16 Dec 2023 11:07:58 GMT
RUN apt-get update && apt-get install --no-install-recommends -y     build-essential     python3-rosdep     python3-rosinstall     python3-vcstools     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:08:03 GMT
RUN rosdep init &&   rosdep update --rosdistro $ROS_DISTRO
# Sat, 16 Dec 2023 11:09:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-ros-base=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 11:17:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-perception=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5319f8e5f3f0f8f6e663c807041d5294b7c309e06b86d115409bbdb4c9d7165`  
		Last Modified: Thu, 14 Dec 2023 13:03:55 GMT  
		Size: 27.2 MB (27203144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3055ab3450adf267aaa7449c6ffccfda8d80fe8870d76661cd5a7a1a979091`  
		Last Modified: Sat, 16 Dec 2023 11:36:49 GMT  
		Size: 1.2 MB (1198805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1234d731199ddd7a60d617e9518f9d1a2a27906869acddfce95b4038e2fde55`  
		Last Modified: Sat, 16 Dec 2023 11:36:48 GMT  
		Size: 5.5 MB (5532123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfa5e73751fb5bd60970eb8780a8ae9ed72f87c95b69b7e0c6329ef023b7de7`  
		Last Modified: Sat, 16 Dec 2023 11:36:46 GMT  
		Size: 2.0 KB (1990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506530cfef7001ed44a0ff97c7fec5ba9a7ce7e7a070755429218cfb01995283`  
		Last Modified: Sat, 16 Dec 2023 11:36:47 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f891826adf07752408bddb6189d021d6d5c7f5bd197dea346bc0a13519d70d`  
		Last Modified: Sat, 16 Dec 2023 11:37:21 GMT  
		Size: 171.4 MB (171416941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0526cad7dfdeb97687cdf3a3541381b207fa0478aad04209fb6a1b23a0165126`  
		Last Modified: Sat, 16 Dec 2023 11:36:47 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9105e544ab5794bfa7b0acdfea1377dfa4de6956ea4099f299d2114be4f7b151`  
		Last Modified: Sat, 16 Dec 2023 11:37:35 GMT  
		Size: 45.2 MB (45206619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8f3230714468cd2b28f53622948398319d93298771e58674b070ade9c1164c`  
		Last Modified: Sat, 16 Dec 2023 11:37:29 GMT  
		Size: 311.3 KB (311292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5405a4edfd87a03463f37e240b93a085378302c5e203e49666551e8bfdb6dd3d`  
		Last Modified: Sat, 16 Dec 2023 11:37:38 GMT  
		Size: 72.0 MB (71972449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b9454d0c4ac3b44e5baa78635964e160295d08dafe796cf4eaea56d7a8ec57`  
		Last Modified: Sat, 16 Dec 2023 11:39:00 GMT  
		Size: 462.7 MB (462682438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
