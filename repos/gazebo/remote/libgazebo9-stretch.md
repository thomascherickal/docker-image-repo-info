## `gazebo:libgazebo9-stretch`

```console
$ docker pull gazebo@sha256:ebed75620a07548664594602d756f55946e581492f5e52ed02cbdbddd348ba4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:c9251543492187f1cfab3ccfb2c1be8e08f8c8301b2329a158f705c905c35898
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **569.8 MB (569808812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eca5d385cfce90dc0108040ff97114822300d5be7bf905375dc218ddc1e497b7`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 04 Aug 2020 15:45:32 GMT
ADD file:a28d8a949b7577768d87fcbac346797fc5f7bad0539625339edcd09a32d6bf77 in / 
# Tue, 04 Aug 2020 15:45:33 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 22:45:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 22:45:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 04 Aug 2020 22:45:32 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 11 Aug 2020 00:30:15 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     gazebo9=9.14.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 11 Aug 2020 00:30:16 GMT
EXPOSE 11345
# Tue, 11 Aug 2020 00:30:16 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 11 Aug 2020 00:30:16 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 11 Aug 2020 00:30:16 GMT
CMD ["gzserver"]
# Tue, 11 Aug 2020 00:31:33 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     libgazebo9-dev=9.14.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:419e7ae5bb1e4875c367f3249b7bb7f8f39dd27dfceb4ee9d6a92191ed1c452f`  
		Last Modified: Tue, 04 Aug 2020 15:52:05 GMT  
		Size: 45.4 MB (45366706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9362859687a2d84c177a1f5dced4161a8c7c4b26ba928f113d95d153b24ea13`  
		Last Modified: Tue, 04 Aug 2020 22:50:24 GMT  
		Size: 18.5 MB (18514064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5637391b288d62be110136b1be071741c95edb378755e4401b398b826b9f718`  
		Last Modified: Tue, 04 Aug 2020 22:50:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce69c2f0891ae2abe2f10f2eab367c3f4aaa94179a17575962179b9c4e67e62`  
		Last Modified: Tue, 04 Aug 2020 22:50:19 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee63b51780b3dea2b20121f60aa92ed243ea1c1ec8bfc05f4b70c304533ed5f6`  
		Last Modified: Tue, 11 Aug 2020 00:35:12 GMT  
		Size: 202.1 MB (202071947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efc12b05c821e245b453cb3d0a1c5a9d7aa12a909e91a6260bce81103a2f45c`  
		Last Modified: Tue, 11 Aug 2020 00:34:46 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd107e89e015ee55f8222bab4a7e8225f27c6964a07e85db34121dc0220f3ab1`  
		Last Modified: Tue, 11 Aug 2020 00:36:06 GMT  
		Size: 303.8 MB (303849507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
