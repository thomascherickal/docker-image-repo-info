## `gazebo:gzserver11-bionic`

```console
$ docker pull gazebo@sha256:bed1bc413a553af6a05f7889e30a63b10a7d38c4f841cb338ace7f424641d278
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:gzserver11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:4e7f26abbabf0227b9ea93e52a1d1858e0c7a4f5ba26af224dda2220d9b87fe5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.8 MB (277834175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ef926b871fcd73f3738d9fc8249fee1815360c033fbc0e9455e4084ce3ae8f`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:28 GMT
ADD file:fc5d658c47ede58827812b75a311353be776e41e2dd339b8906839527c9b5247 in / 
# Tue, 25 Oct 2022 01:53:28 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:51:42 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 16:13:39 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 16:13:41 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 25 Oct 2022 16:13:41 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 25 Oct 2022 16:20:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 16:20:48 GMT
EXPOSE 11345
# Tue, 25 Oct 2022 16:20:48 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 25 Oct 2022 16:20:48 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 25 Oct 2022 16:20:48 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:a404e54162968593b8d92b571f3cdd673e4c9eab5d9be28d7c494595c0aa6682`  
		Last Modified: Wed, 19 Oct 2022 22:03:02 GMT  
		Size: 26.7 MB (26712500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1955214fb5b152d9d9fa8ce9a39b19a4e6e8ea487bc617e76c0b7b33e1881bc`  
		Last Modified: Tue, 25 Oct 2022 07:50:06 GMT  
		Size: 831.1 KB (831118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166914147cb39d9ad693b063b8ea6022015e3203dca13b3bf8c3be6951e232c1`  
		Last Modified: Tue, 25 Oct 2022 16:32:23 GMT  
		Size: 14.7 MB (14712241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db34c22a0ae7f25ca1839bd6ac277829806dbfb1afd9ce9381deb51f654d1392`  
		Last Modified: Tue, 25 Oct 2022 16:32:20 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6c417d473038c6eae574a73a9c2d657949a178503aeca99922d3efe0b8ebc6`  
		Last Modified: Tue, 25 Oct 2022 16:32:21 GMT  
		Size: 5.5 KB (5459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d140684d7286ac25e6d9becc9c5579811497dc2e5645527048d5734890cb53`  
		Last Modified: Wed, 26 Oct 2022 16:36:32 GMT  
		Size: 235.6 MB (235571229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e1e55979059e3ffe01638645c63347648a3643fd8dfdddc5683e3e748b429c`  
		Last Modified: Wed, 26 Oct 2022 16:36:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
