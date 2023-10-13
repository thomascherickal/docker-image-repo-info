## `gazebo:libgazebo11-focal`

```console
$ docker pull gazebo@sha256:e75ee052587a007b3ef83fea3abd53840572f7344009cbfc19c2f63af0e29575
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo11-focal` - linux; amd64

```console
$ docker pull gazebo@sha256:d0b990bf563c79922a253e2dee35a25010e124f7fdacaca6eb22e96912d997db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.5 MB (610537806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b408db230000fd63ba469b95af7ac2bc21059b32f667dbb2fb0cd3eda689c335`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 08:18:46 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 08:19:09 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 08:19:11 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 13 Oct 2023 08:19:11 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 13 Oct 2023 08:22:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.14.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 08:22:33 GMT
EXPOSE 11345
# Fri, 13 Oct 2023 08:22:34 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 13 Oct 2023 08:22:34 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 13 Oct 2023 08:22:34 GMT
CMD ["gzserver"]
# Fri, 13 Oct 2023 08:27:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.14.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5335424d66dbb0ed84c3c6fa8b1d6d5d39dd2f8470a58b1b417fe9f4edad07`  
		Last Modified: Fri, 13 Oct 2023 08:27:45 GMT  
		Size: 1.2 MB (1198710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e97ee7f447a57e107eccf927d5c6972913b2f460fb4e612d81a18a827d70d0`  
		Last Modified: Fri, 13 Oct 2023 08:27:45 GMT  
		Size: 16.2 MB (16177130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078880be30cf4bf619889ad445c5b5fad24720a16ff291819b752d8d842a13c1`  
		Last Modified: Fri, 13 Oct 2023 08:27:42 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55f6b5283a1d195c7d9754b82f599e7d8ebfa57d8afda314bd23ffb97087525`  
		Last Modified: Fri, 13 Oct 2023 08:27:42 GMT  
		Size: 5.5 KB (5502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794e82e837076758558d73f254b194e9a0cfb91604ff2a6b4a64a888cacf948`  
		Last Modified: Fri, 13 Oct 2023 08:28:13 GMT  
		Size: 276.1 MB (276064344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e86ade25cc6aaf921596ef98f126c036d8e023fdfd099054e1b76bf645ce9a1`  
		Last Modified: Fri, 13 Oct 2023 08:27:42 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6102a6865ec9aa11e980cda186c82ab52a0a14ba5e9c82112d34c4e806455fbc`  
		Last Modified: Fri, 13 Oct 2023 08:29:07 GMT  
		Size: 288.5 MB (288509815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
