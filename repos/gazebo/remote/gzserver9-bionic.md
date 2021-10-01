## `gazebo:gzserver9-bionic`

```console
$ docker pull gazebo@sha256:770f0daf23028c972e66b0fd345706a6eea1bbb1c0e1bee25ecf4462edab62cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver9-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:b92f5ab9d5faa9f19a69871d9866aac570692be76c47b433fb2d0a6d7ca9319b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.4 MB (268422686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1aa85b45a6502c2e17a4d3077c1023db4fa3f43e6e859aba42d6856e1bace3`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:23 GMT
ADD file:0d82cd095966e8ee78b593cb47a352eec842edb7bd9d9468e8a70154522447d1 in / 
# Fri, 01 Oct 2021 02:23:24 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 04:52:50 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:53:03 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:53:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 01 Oct 2021 04:53:10 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Fri, 01 Oct 2021 04:56:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:56:23 GMT
EXPOSE 11345
# Fri, 01 Oct 2021 04:56:23 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Fri, 01 Oct 2021 04:56:24 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Fri, 01 Oct 2021 04:56:24 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:284055322776031bac33723839acb0db2d063a525ba4fa1fd268a831c7553b26`  
		Last Modified: Fri, 01 Oct 2021 02:25:02 GMT  
		Size: 26.7 MB (26705075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be57c60580131e55159e03672358dbc415078de9b8d6b73691837b848489424`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 840.7 KB (840739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385846ca0d15120a037d2cc3a853015e25edde30cd5be1a40ef2fb7d9f8c2a11`  
		Last Modified: Fri, 01 Oct 2021 05:12:47 GMT  
		Size: 14.7 MB (14703032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd8248f6f5fe1f59e4c79a671cb199bc9da0529b1e7c7549dc978c92eb93d81`  
		Last Modified: Fri, 01 Oct 2021 05:12:44 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ff515e08b456436e1bc3aec3fc5de6c8300bdc9ed65a4c3dbf8cc01b1e0ad7`  
		Last Modified: Fri, 01 Oct 2021 05:12:44 GMT  
		Size: 5.5 KB (5454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106389644a87f1ba99f911dd46bbcfda50b20b76a84615860329d31be3d04294`  
		Last Modified: Fri, 01 Oct 2021 05:13:13 GMT  
		Size: 226.2 MB (226166758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fc8daf44e7827128d3720bc030dafcbca87ec81dd2b4dd19178d317e08af21`  
		Last Modified: Fri, 01 Oct 2021 05:12:44 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
