## `gazebo:libgazebo11-focal`

```console
$ docker pull gazebo@sha256:37aaa7f08866e05b667fb2454c7306350a6edd743047f09ece2cb278e5ac3de4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `gazebo:libgazebo11-focal` - linux; amd64

```console
$ docker pull gazebo@sha256:94d8664acbfd5ca0b62fa72ed7ed42f1588b81d7416ef25476df951c968545e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **607.1 MB (607060434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883b0e37d771466277aaca22bbf68c524da8567751a86cbf24fc64abb5824319`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:48:54 GMT
RUN echo 'Etc/UTC' > /etc/timezone &&     ln -s /usr/share/zoneinfo/Etc/UTC /etc/localtime &&     apt-get update &&     apt-get install -q -y --no-install-recommends tzdata &&     rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:49:28 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 23:49:31 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Mon, 26 Jul 2021 23:49:33 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Mon, 30 Aug 2021 21:32:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo11=11.8.1-1*     && rm -rf /var/lib/apt/lists/*
# Mon, 30 Aug 2021 21:32:53 GMT
EXPOSE 11345
# Mon, 30 Aug 2021 21:32:53 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Mon, 30 Aug 2021 21:32:54 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Mon, 30 Aug 2021 21:32:54 GMT
CMD ["gzserver"]
# Mon, 30 Aug 2021 21:38:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo11-dev=11.8.1-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ec889c2abce161c5ac65f816c63d528f9b38633bcdcb93759283fd6bd28064`  
		Last Modified: Tue, 27 Jul 2021 00:03:14 GMT  
		Size: 1.2 MB (1182475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52fa7f2bbaf9fdabe2f4f44c9c14e354edb50cbf9d14d543c25068e3bac43f3`  
		Last Modified: Tue, 27 Jul 2021 00:03:13 GMT  
		Size: 16.2 MB (16166865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82b78dfba60e8c933ef391fb029a1696247906bdb721ab7b16f27384a190896`  
		Last Modified: Tue, 27 Jul 2021 00:03:11 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc640b65e76d09c20486b01253367703fec36621d99d69308307a3e4d62531f`  
		Last Modified: Tue, 27 Jul 2021 00:03:10 GMT  
		Size: 5.5 KB (5500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8cd4acd28c8308eb79bbbd036db1a4d55906569cbd3673e333a9ac4c5cb71d`  
		Last Modified: Mon, 30 Aug 2021 21:40:47 GMT  
		Size: 274.9 MB (274907766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7779125c1a30540435b5906ed022af81b8192a291f3caa2612ba3eb7b0a67cec`  
		Last Modified: Mon, 30 Aug 2021 21:40:13 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3857779084d786e8b90ab473ce0a3bdb6cce3093e3f606bc0094a661b33b54f0`  
		Last Modified: Mon, 30 Aug 2021 21:41:52 GMT  
		Size: 286.2 MB (286228252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
