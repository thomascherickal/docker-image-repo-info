## `gazebo:libgazebo9-stretch`

```console
$ docker pull gazebo@sha256:40d6e3cfe4085e4f5678a89f6331ae99fcba55cb0aaea98cb70e35918a3364fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gazebo:libgazebo9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:b72ab440769008cfbe7d5d0a3343a4d833aa4c758792fbc3b840edbdc1365bfd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **570.2 MB (570238310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f127abea4deb4f4e56e5f8645b0a13149be636902e14eb83bebc92f4d4efa76`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:41 GMT
ADD file:e3d37689e896a83d39040f2c95091ff88f3899b5b410dbf76908dd6c938b8cb5 in / 
# Sat, 10 Apr 2021 01:21:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:24:05 GMT
RUN apt-get update && apt-get install -q -y --no-install-recommends     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:24:09 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Sat, 10 Apr 2021 06:24:10 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Sat, 10 Apr 2021 06:24:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     gazebo9=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:24:52 GMT
EXPOSE 11345
# Sat, 10 Apr 2021 06:24:52 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Sat, 10 Apr 2021 06:24:53 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Sat, 10 Apr 2021 06:24:53 GMT
CMD ["gzserver"]
# Sat, 10 Apr 2021 06:26:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends     libgazebo9-dev=9.16.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76b8ef87096fa726adbe8f073ef69bb5664bac19474c5cce4dd69e08a234903b`  
		Last Modified: Sat, 10 Apr 2021 01:27:52 GMT  
		Size: 45.4 MB (45380037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076c2848c0f62a03b335a23fcdf7b4a09b96de530a291468ebdf88bbef1ced90`  
		Last Modified: Sat, 10 Apr 2021 06:27:51 GMT  
		Size: 18.5 MB (18511169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23ca0e9c6fd3161e166facc173b7030ba8591bc1a6d5ae69970bfbcd1e05f85`  
		Last Modified: Sat, 10 Apr 2021 06:27:41 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fd00cc40f4220324a4d6b05a3d27cf9e966213a770480d61fb8b71c9eacef8`  
		Last Modified: Sat, 10 Apr 2021 06:27:41 GMT  
		Size: 5.0 KB (5015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e396c43061b4b7c79a4a32a637b5e7455e580b7e4bb4e77aa26489d4fe6d2a00`  
		Last Modified: Sat, 10 Apr 2021 06:28:14 GMT  
		Size: 202.3 MB (202283449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b74ef5fe9af0a6ff244ae819b0e914ddeda7a68eefda3108b2b292c51fe9bc7`  
		Last Modified: Sat, 10 Apr 2021 06:27:47 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3480698358b64ff52798ce9a935e33afcff333966e0e0a401e3cd543356b2df`  
		Last Modified: Sat, 10 Apr 2021 06:29:17 GMT  
		Size: 304.1 MB (304057030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
