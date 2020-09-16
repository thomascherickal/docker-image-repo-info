## `swarm:latest`

```console
$ docker pull swarm@sha256:2de8883e2933840ed7ee7360ea1eed314bf8aeac37c0692b9ca651630fde3b7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `swarm:latest` - linux; amd64

```console
$ docker pull swarm@sha256:b09c61cb20e925723210a2d2504043766381d59751079ca6e57ca9c4a71ebe3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3849920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a5eb59a410faeff5de495f07553845624ad3278ac59ac066107564bdd14bf48`
-	Entrypoint: `["\/swarm"]`
-	Default Command: `["--help"]`

```dockerfile
# Wed, 16 Sep 2020 20:15:18 GMT
COPY file:baf765dce7d83eed89fb4848147c416423cc42bf07523d8d93b72ed539bf7e1d in /swarm 
# Wed, 16 Sep 2020 20:15:19 GMT
COPY file:542309c051962f73f8ace49c3bc97bfd3743b6f105ae8fd920186dde62b7481f in /etc/ssl/certs/ca-certificates.crt 
# Wed, 16 Sep 2020 20:15:20 GMT
COPY dir:9d1a4b75a1813e208a4ef5f72a74f6b9b14c74574a2e191d9e800a4698e2174e in /tmp 
# Wed, 16 Sep 2020 20:15:20 GMT
ENV SWARM_HOST=:2375
# Wed, 16 Sep 2020 20:15:20 GMT
EXPOSE 2375
# Wed, 16 Sep 2020 20:15:21 GMT
VOLUME [/.swarm]
# Wed, 16 Sep 2020 20:15:21 GMT
ENTRYPOINT ["/swarm"]
# Wed, 16 Sep 2020 20:15:21 GMT
CMD ["--help"]
```

-	Layers:
	-	`sha256:38e5683d7755d5390caf8ef4e7b3d52e81f592cee695ba41dd696efa685b3657`  
		Last Modified: Wed, 16 Sep 2020 20:15:31 GMT  
		Size: 3.7 MB (3693031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083aff16360665b6a2e34da65173bfa2b005b7cb77327239984b4f3f3a2d0b0e`  
		Last Modified: Wed, 16 Sep 2020 20:15:30 GMT  
		Size: 156.8 KB (156761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2064f1a73c6be65f86bab532e48f884e20f3ebda94c23207166ebcf1f6ba48ee`  
		Last Modified: Wed, 16 Sep 2020 20:15:30 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
