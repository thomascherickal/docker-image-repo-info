## `gazebo:libgazebo9-stretch`

```console
$ docker pull gazebo@sha256:f87f3c4a6a8cdba7c84ca35a57f3f9c868f1f167c8843a1c0d978cfa0e1dbe87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:a6f0368196c160ce823fb99883e7fdfa336f0b8121c2e978f5af7bf6608166c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **651.0 MB (650967047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7af8b712222ef20460947b61afd9e58e00628ee0c15563153f10a0eb6b453989`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 31 Mar 2020 01:23:50 GMT
ADD file:774b5e2033bb42ad97daa64267a5f041124cc0b05ec0198f1b5578ceea5a48e4 in / 
# Tue, 31 Mar 2020 01:23:51 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:00:28 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:00:32 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 31 Mar 2020 03:00:33 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Tue, 31 Mar 2020 03:02:09 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.12.0-1*     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:02:10 GMT
EXPOSE 11345
# Tue, 31 Mar 2020 03:02:11 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Tue, 31 Mar 2020 03:02:11 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Tue, 31 Mar 2020 03:02:11 GMT
CMD ["gzserver"]
# Tue, 31 Mar 2020 03:03:56 GMT
RUN apt-get update && apt-get install -q -y     libgazebo9-dev=9.12.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56da78ce36e97a8ba1f860575bb1422d1cb6ab4dade70b06ddf1651302dde955`  
		Last Modified: Tue, 31 Mar 2020 01:29:15 GMT  
		Size: 45.4 MB (45375928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e92ca761da7f6f719acf4b66fa2990e5acced3d4ac082537a32a58ef50fcf2`  
		Last Modified: Tue, 31 Mar 2020 03:04:53 GMT  
		Size: 21.1 MB (21095187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea065aed5bfb6ede5ca8ae4ffd621df98ad95309396eeac3875a05c06b2ebba8`  
		Last Modified: Tue, 31 Mar 2020 03:04:46 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f3d81549277fd1a48226b35bfcef19ea68f0d1fb39435f06de099b975b936b`  
		Last Modified: Tue, 31 Mar 2020 03:04:46 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05f66a744a02fff2f10c4f75ef6bf2b917597c5fe60d1d01126b58d80e4168e`  
		Last Modified: Tue, 31 Mar 2020 03:05:44 GMT  
		Size: 279.9 MB (279871558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e223e73cb4f8098504db8efe2d354ed3808b04234e2c873daa42b72ca1fe52b9`  
		Last Modified: Tue, 31 Mar 2020 03:04:46 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfff87286c5188ad5c3aa0cf045e73b67620116ec6aeacf8f3bbe279297a3cb`  
		Last Modified: Tue, 31 Mar 2020 03:06:59 GMT  
		Size: 304.6 MB (304617785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
