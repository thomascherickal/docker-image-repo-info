## `gazebo:gzserver11-bionic`

```console
$ docker pull gazebo@sha256:aea505a8cb88f29fee94751bd898d45f603ea031013d2cab8f67f5b70bdcffae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:gzserver11-bionic` - linux; amd64

```console
$ docker pull gazebo@sha256:5916ae36fb4c94fd6e5d0b44bda38d11c3fbee333a89321b3dcf5bf6a4b99b24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.4 MB (277448367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04cef62a6398203f048a3e6cfee536b27aff061d97e718f5195434e0938b0050`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:23:14 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:23:32 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:23:34 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Fri, 18 Jun 2021 01:23:35 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 24 Jun 2021 19:31:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.6.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 19:31:04 GMT
EXPOSE 11345
# Thu, 24 Jun 2021 19:31:04 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 24 Jun 2021 19:31:04 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 24 Jun 2021 19:31:04 GMT
CMD ["gzserver"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da448bd4f8f4db94a9b5039505342a7b53dd81b10fd374d2def1098fb0ac84d1`  
		Last Modified: Fri, 18 Jun 2021 02:24:11 GMT  
		Size: 841.3 KB (841252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c9bccca2de788969af6d6e387abb084c66ce0679c41ca4712bf3787173a3b8`  
		Last Modified: Thu, 24 Jun 2021 19:43:56 GMT  
		Size: 14.7 MB (14702322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97918488cc093177c1052f8a9ec4c7729f138fe79a40137d1a3198f8ac2de6e`  
		Last Modified: Thu, 24 Jun 2021 19:43:53 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389903f5c318711646c39cd700afeaea7d7beac2750a1953f8325917e500ffcb`  
		Last Modified: Thu, 24 Jun 2021 19:43:53 GMT  
		Size: 5.5 KB (5459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64084ff7bf85aca85a1eaad9d0f81e01bdd1cb5f6de5e0036382719f3049ba81`  
		Last Modified: Thu, 24 Jun 2021 19:45:37 GMT  
		Size: 235.2 MB (235197001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fa6b1dac68d4aada315b152ed08388996ee8075c68f54d1513b33c76b5767e`  
		Last Modified: Thu, 24 Jun 2021 19:45:07 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
