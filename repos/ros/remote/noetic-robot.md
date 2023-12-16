## `ros:noetic-robot`

```console
$ docker pull ros@sha256:e2d1a9dc51a7b660d307e977062203c39bcb9209e8cc5eeb701d1274b244a92f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ros:noetic-robot` - linux; amd64

```console
$ docker pull ros@sha256:02af0855315492649518532844615e4e9a52f376507a99e62cbc95f6d2955148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (359036286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b2e0ef7eb7bc61c979bdcd559d8b847bb3f611d14b4c65a38997f4a83dafe21`
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
# Sat, 16 Dec 2023 09:40:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:03fc26c0942e6ea571edbaa2b6dc7ca635460243636f430c0548ac8941b2eac8`  
		Last Modified: Sat, 16 Dec 2023 10:06:10 GMT  
		Size: 15.9 MB (15865302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm variant v7

```console
$ docker pull ros@sha256:6b36005461cc659673ed1692889f039d16f52c2abd8ec3039e0501b08bf108f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.3 MB (303324544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cfb5f820bb7aba5ea28aade0eb2360f82e7de54e803d144424ba97b15dd335e`
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
# Sat, 16 Dec 2023 09:42:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:bf539cad1625afd5268e42be8ea819a4579655da66af147aaa75ef57d51e3d44`  
		Last Modified: Sat, 16 Dec 2023 09:51:06 GMT  
		Size: 14.1 MB (14069258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ros:noetic-robot` - linux; arm64 variant v8

```console
$ docker pull ros@sha256:43347a2ac47c58ebd11388f40a1af573ee4f0703f731731681037830deca509f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.3 MB (338303525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f79917304bc06857fdb97f38c4a20430944f26a70b362d5ad2811929ce85c853`
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
# Sat, 16 Dec 2023 11:10:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     ros-noetic-robot=1.5.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:9f35ef0b517d008c0bbbd57786a4d275672f78051360dfb63ae3c865601e007f`  
		Last Modified: Sat, 16 Dec 2023 11:37:51 GMT  
		Size: 15.5 MB (15459746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
