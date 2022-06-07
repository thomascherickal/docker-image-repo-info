## `gazebo:latest`

```console
$ docker pull gazebo@sha256:8f904171395e73d06e6109daf844096498401a099306dcd52757df7801b39e3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:latest` - linux; amd64

```console
$ docker pull gazebo@sha256:fd7850ffbca6aee27daf5b1f081226a285e00a036f4fc5908d38f74bb670e577
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **610.2 MB (610182153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:520dd1bb9396419cc4806d0d488c6d09726ab29a4d52fc7da1bb4a6edbc01f2b`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 01:10:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:39:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:39:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 07 Jun 2022 02:39:41 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 07 Jun 2022 02:42:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.11.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:43:01 GMT
EXPOSE 11345
# Tue, 07 Jun 2022 02:43:01 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 07 Jun 2022 02:43:01 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 07 Jun 2022 02:43:01 GMT
CMD ["gzserver"]
# Tue, 07 Jun 2022 02:47:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.11.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1e38681d9b6d153af3be7e0550217dc0dfb994512346ebc7d9a7a602651e74`  
		Last Modified: Tue, 07 Jun 2022 01:47:20 GMT  
		Size: 1.2 MB (1181179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d4c8cdf1599b6113f017c9b8640498c7ca7e8bd333906a8762ccec91113f2`  
		Last Modified: Tue, 07 Jun 2022 02:50:47 GMT  
		Size: 16.2 MB (16170345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739cdaa045d1969853310db99b4f8e7264df3ded02193e5a4f19ece199e29910`  
		Last Modified: Tue, 07 Jun 2022 02:50:44 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6fae702b107d5779d0f3e20b426886fe6847e711d83c20bbbda128bb1390a1`  
		Last Modified: Tue, 07 Jun 2022 02:50:44 GMT  
		Size: 5.5 KB (5501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e311e3aba0fd0ad27f4e8709b2f449556b2f6696da715d1af0f69946584a532c`  
		Last Modified: Tue, 07 Jun 2022 02:51:18 GMT  
		Size: 275.9 MB (275930385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb87f1d22df33176b0b10d8516c2480564c5f84b4d924b2aad61dbb494f3df13`  
		Last Modified: Tue, 07 Jun 2022 02:50:44 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217626badbd901a61913fea8dc959e1fdcf2f8b3f599d8eb36d83fb00ab54095`  
		Last Modified: Tue, 07 Jun 2022 02:52:17 GMT  
		Size: 288.3 MB (288320484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
