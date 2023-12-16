## `gazebo:libgazebo11`

```console
$ docker pull gazebo@sha256:c7bad816fd696e25d2cb84d002fd460ca9a4e5531fd16663cae34170e9c668c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo11` - linux; amd64

```console
$ docker pull gazebo@sha256:67bfdb45d77449dfd7ab047068d3b26caec86e1d78e107b6ddf957d894743418
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.5 MB (610538936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4096389933aa7c9532d4073ff151e4741e6577ad4525012e5837ff5f7fd9cbc6`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

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
# Sat, 16 Dec 2023 10:42:21 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:42:22 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Sat, 16 Dec 2023 10:42:23 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Sat, 16 Dec 2023 10:45:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.14.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 10:45:23 GMT
EXPOSE 11345
# Sat, 16 Dec 2023 10:45:24 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Sat, 16 Dec 2023 10:45:24 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Sat, 16 Dec 2023 10:45:24 GMT
CMD ["gzserver"]
# Sat, 16 Dec 2023 10:49:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.14.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:b1d6a0860bbac33f0a5ec1445c8c0f3766ec0688b1f60c7ca72235259bc1f773`  
		Last Modified: Sat, 16 Dec 2023 10:50:09 GMT  
		Size: 16.2 MB (16160978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3e77448a2c53187d40a16536903ebb435f9972d2fd0c64bdb3dfd2124da9be`  
		Last Modified: Sat, 16 Dec 2023 10:50:06 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21b4e25ea6938c452ee91cf116d1f5844b060bfb7466767ca2e98b35f3ee3c0`  
		Last Modified: Sat, 16 Dec 2023 10:50:06 GMT  
		Size: 5.5 KB (5501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaa38e89d3b2cda3356e0e4fcee72868a47953b67bef37f7797297ba694bb2d`  
		Last Modified: Sat, 16 Dec 2023 10:50:36 GMT  
		Size: 276.1 MB (276065238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf078ee6d9007dbcc80d16d7441c306d6a16518a65be3bc8af77079d5d6c10f6`  
		Last Modified: Sat, 16 Dec 2023 10:50:06 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8415facdc74de93f3f678d4037d1d6cc5d1b0ae697bbed79f1b95d65fdf5f18c`  
		Last Modified: Sat, 16 Dec 2023 10:51:28 GMT  
		Size: 288.5 MB (288522722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
