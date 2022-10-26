## `gazebo:libgazebo9-bionic`

```console
$ docker pull gazebo@sha256:9a2e102226139067ffc06c2690429cabdaa309dcf928c7195f2bb5174947fad5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo9-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:b640a7647d18f1ff97cd5496e3b08da0dc83c3a3782514f70c073e60d630cb21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.8 MB (413820345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476e871a6089fbc197e5eb594195fb22f677989d331420aeff27ef9d6dd063a5`
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
# Tue, 25 Oct 2022 16:16:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 16:16:44 GMT
EXPOSE 11345
# Tue, 25 Oct 2022 16:16:44 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 25 Oct 2022 16:16:44 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 25 Oct 2022 16:16:44 GMT
CMD ["gzserver"]
# Tue, 25 Oct 2022 16:19:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo9-dev=9.19.0-1*     && rm -rf /var/lib/apt/lists/*
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
	-	`sha256:66bb9d146a9a99b7f3fbdd4492394f4e1927649da69ffa49ded071c583856763`  
		Last Modified: Tue, 25 Oct 2022 16:32:48 GMT  
		Size: 226.2 MB (226196904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fed2a8c65ea5fef22aefc03f99298082a8e786bb0092ba10f7352ca01b45dc`  
		Last Modified: Tue, 25 Oct 2022 16:32:20 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7919bd3bc9037db6d69fd40829111e60226605a495e39bda50730a0d3892c7a7`  
		Last Modified: Wed, 26 Oct 2022 16:35:50 GMT  
		Size: 145.4 MB (145360496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
