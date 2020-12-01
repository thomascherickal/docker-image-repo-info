## `gazebo:gzserver9-stretch`

```console
$ docker pull gazebo@sha256:8ab8a4717f6309ceb798809690e16d4ed2e30c31b18176f21b84606991f19f2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:3827d079457ede129c68f7856f8503ac7894d02f599f1516e2ebadf534321f5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.2 MB (266160546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aa81fcacbab70065311ad1497e4ac052f3ccdc3708053b862e3b6463d15adbd`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:10 GMT
ADD file:373a8875589f170b51fa677a3bf736feeb46ea278c553950a3eb3169a2056c12 in / 
# Tue, 17 Nov 2020 20:24:11 GMT
CMD ["bash"]
# Wed, 25 Nov 2020 23:00:18 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:00:21 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Wed, 25 Nov 2020 23:00:22 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 01 Dec 2020 02:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 01 Dec 2020 02:33:27 GMT
EXPOSE 11345
# Tue, 01 Dec 2020 02:33:27 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 01 Dec 2020 02:33:27 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 01 Dec 2020 02:33:27 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:7919f5b7d60254cafc73c0d097b8ccffb72e0b6472957ece4dd5b378c5ca7cc1`  
		Last Modified: Tue, 17 Nov 2020 20:30:26 GMT  
		Size: 45.4 MB (45377037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de024813af17ed216f67e7d6d9554fdef08a7f8c488eddd467da8fc65a63cc95`  
		Last Modified: Tue, 01 Dec 2020 02:54:31 GMT  
		Size: 18.5 MB (18507886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2073549511f70d50a91bbc68d796050eb2699b74018caa76ceacc411bb3e780`  
		Last Modified: Tue, 01 Dec 2020 02:54:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c46023b74b8334e31432b592d558d7d17ecd658bec07448b38754fde9cdc93`  
		Last Modified: Tue, 01 Dec 2020 02:54:20 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a23572039ef2d076ce9abb05ed32062b55b5b2652f4c16ce77c2d4e2b0a835`  
		Last Modified: Tue, 01 Dec 2020 02:55:09 GMT  
		Size: 202.3 MB (202269032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b40f87165a28d08fd3832faebc9729ef7a6658ccc81737a7be3ab82972e89d`  
		Last Modified: Tue, 01 Dec 2020 02:54:20 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
