<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `registry`

-	[`registry:2`](#registry2)
-	[`registry:2.7`](#registry27)
-	[`registry:2.7.1`](#registry271)
-	[`registry:latest`](#registrylatest)

## `registry:2`

```console
$ docker pull registry@sha256:d5459fcb27aecc752520df4b492b08358a1912fcdfa454f7d2101d4b09991daa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `registry:2` - linux; amd64

```console
$ docker pull registry@sha256:a0dd61073ad21122e5f1517682800272ef29df52041aaea7ee29e92a5d22aa28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9938926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678dfa38fcfa349ccbdb1b6d52ac113ace67d5746794b36dfbad9dd96a9d1c43`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:13:59 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Thu, 17 Dec 2020 13:14:00 GMT
COPY file:21256ff7df5369f7ad2e19c6d020a644303aded200bdbec4d46648f38d55df78 in /bin/registry 
# Thu, 17 Dec 2020 13:14:00 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 17 Dec 2020 13:14:01 GMT
VOLUME [/var/lib/registry]
# Thu, 17 Dec 2020 13:14:01 GMT
EXPOSE 5000
# Thu, 17 Dec 2020 13:14:02 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:14:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:14:02 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d550a247d74fe258880d43f82ce0679ad2bef73b5833e3fc63e4326aa51c1418`  
		Last Modified: Thu, 17 Dec 2020 13:14:17 GMT  
		Size: 299.5 KB (299548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a938458ca360e0d59e750b7f55d786b0cdc54250a800d52d9000d601edb1505`  
		Last Modified: Thu, 17 Dec 2020 13:14:20 GMT  
		Size: 6.8 MB (6823928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd758c36fc9019145bd7e2f8222bc6abe8d864d727b79f9adade6ad2eccbf36`  
		Last Modified: Thu, 17 Dec 2020 13:14:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af6d68b484a730daaa243a546283a8c01db8c8e2cb28a9c114130bfc7b00e81`  
		Last Modified: Thu, 17 Dec 2020 13:14:17 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; arm variant v6

```console
$ docker pull registry@sha256:c8c97b4d572c33156da59bae82f6b833abf5ceaa69bb18d002406c2891fce4a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9312382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2126abe3746bfb8bd3bccc38ecc00d331a3bad9db38232c473ddf04e92c2078a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:52:08 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Thu, 17 Dec 2020 07:52:09 GMT
COPY file:29c6c1625420a558a03cc7ed253192f8138cba6212b64e30217fb6488af668e2 in /bin/registry 
# Thu, 17 Dec 2020 07:52:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 17 Dec 2020 07:52:12 GMT
VOLUME [/var/lib/registry]
# Thu, 17 Dec 2020 07:52:13 GMT
EXPOSE 5000
# Thu, 17 Dec 2020 07:52:14 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 17 Dec 2020 07:52:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 07:52:16 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7cc14966ceb5e5b46be135c16f21f7af42f270518ed92962f9514d0874ce7d`  
		Last Modified: Thu, 17 Dec 2020 07:52:29 GMT  
		Size: 299.9 KB (299919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96618f9c1a201fedc2049c85c36fc0b4a817442c4f712140f49d76310034d2f7`  
		Last Modified: Thu, 17 Dec 2020 07:52:33 GMT  
		Size: 6.4 MB (6391083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acb2c1463288a9621bede426350b5e343e6beb7639ab71ea9be3cd67599bb52`  
		Last Modified: Thu, 17 Dec 2020 07:52:28 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9b1ea70368acb9d8c55ea555a87c799805882309d54ad7af9aa7d8e1d8b366`  
		Last Modified: Thu, 17 Dec 2020 07:52:29 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:d42f9d2035ce5b9181ae8cc81d5646a2070a33c8125e21dc0d9e8dbddba97d69
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9266098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357aab9e21a8d6c2810a3fe7ad21db85d1a46a367aae3d4479d6c606810c3999`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:52:07 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Thu, 17 Dec 2020 08:52:09 GMT
COPY file:51a441e6eceff49ef32609e7070b64e8d5690648e4f915cc825274e6fe37aed2 in /bin/registry 
# Thu, 17 Dec 2020 08:52:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 17 Dec 2020 08:52:12 GMT
VOLUME [/var/lib/registry]
# Thu, 17 Dec 2020 08:52:12 GMT
EXPOSE 5000
# Thu, 17 Dec 2020 08:52:13 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 17 Dec 2020 08:52:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 08:52:15 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354f1e88083af06aeab8d62885a9fc4837e4dd4df7401e88d2dad92cf5d3d380`  
		Last Modified: Thu, 17 Dec 2020 08:52:30 GMT  
		Size: 300.1 KB (300071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2dc4de40f59228ac116ecb91079d2619ad49846d335db1f936625f0f334313`  
		Last Modified: Thu, 17 Dec 2020 08:52:31 GMT  
		Size: 6.2 MB (6240199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d14370ba8f615dba79dd19dd77cfd5cb6bbf8594dd2720a7e75f114e392ff2`  
		Last Modified: Thu, 17 Dec 2020 08:52:30 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df0f8d558c48693436cf0dcb3f2d0c3cd49cc5ecd9fbf74333bd27a0f70884f`  
		Last Modified: Thu, 17 Dec 2020 08:52:29 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:2.7`

```console
$ docker pull registry@sha256:d5459fcb27aecc752520df4b492b08358a1912fcdfa454f7d2101d4b09991daa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `registry:2.7` - linux; amd64

```console
$ docker pull registry@sha256:a0dd61073ad21122e5f1517682800272ef29df52041aaea7ee29e92a5d22aa28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9938926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678dfa38fcfa349ccbdb1b6d52ac113ace67d5746794b36dfbad9dd96a9d1c43`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:13:59 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Thu, 17 Dec 2020 13:14:00 GMT
COPY file:21256ff7df5369f7ad2e19c6d020a644303aded200bdbec4d46648f38d55df78 in /bin/registry 
# Thu, 17 Dec 2020 13:14:00 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 17 Dec 2020 13:14:01 GMT
VOLUME [/var/lib/registry]
# Thu, 17 Dec 2020 13:14:01 GMT
EXPOSE 5000
# Thu, 17 Dec 2020 13:14:02 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:14:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:14:02 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d550a247d74fe258880d43f82ce0679ad2bef73b5833e3fc63e4326aa51c1418`  
		Last Modified: Thu, 17 Dec 2020 13:14:17 GMT  
		Size: 299.5 KB (299548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a938458ca360e0d59e750b7f55d786b0cdc54250a800d52d9000d601edb1505`  
		Last Modified: Thu, 17 Dec 2020 13:14:20 GMT  
		Size: 6.8 MB (6823928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd758c36fc9019145bd7e2f8222bc6abe8d864d727b79f9adade6ad2eccbf36`  
		Last Modified: Thu, 17 Dec 2020 13:14:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af6d68b484a730daaa243a546283a8c01db8c8e2cb28a9c114130bfc7b00e81`  
		Last Modified: Thu, 17 Dec 2020 13:14:17 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.7` - linux; arm variant v6

```console
$ docker pull registry@sha256:c8c97b4d572c33156da59bae82f6b833abf5ceaa69bb18d002406c2891fce4a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9312382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2126abe3746bfb8bd3bccc38ecc00d331a3bad9db38232c473ddf04e92c2078a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:52:08 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Thu, 17 Dec 2020 07:52:09 GMT
COPY file:29c6c1625420a558a03cc7ed253192f8138cba6212b64e30217fb6488af668e2 in /bin/registry 
# Thu, 17 Dec 2020 07:52:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 17 Dec 2020 07:52:12 GMT
VOLUME [/var/lib/registry]
# Thu, 17 Dec 2020 07:52:13 GMT
EXPOSE 5000
# Thu, 17 Dec 2020 07:52:14 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 17 Dec 2020 07:52:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 07:52:16 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7cc14966ceb5e5b46be135c16f21f7af42f270518ed92962f9514d0874ce7d`  
		Last Modified: Thu, 17 Dec 2020 07:52:29 GMT  
		Size: 299.9 KB (299919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96618f9c1a201fedc2049c85c36fc0b4a817442c4f712140f49d76310034d2f7`  
		Last Modified: Thu, 17 Dec 2020 07:52:33 GMT  
		Size: 6.4 MB (6391083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acb2c1463288a9621bede426350b5e343e6beb7639ab71ea9be3cd67599bb52`  
		Last Modified: Thu, 17 Dec 2020 07:52:28 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9b1ea70368acb9d8c55ea555a87c799805882309d54ad7af9aa7d8e1d8b366`  
		Last Modified: Thu, 17 Dec 2020 07:52:29 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.7` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:d42f9d2035ce5b9181ae8cc81d5646a2070a33c8125e21dc0d9e8dbddba97d69
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9266098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357aab9e21a8d6c2810a3fe7ad21db85d1a46a367aae3d4479d6c606810c3999`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:52:07 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Thu, 17 Dec 2020 08:52:09 GMT
COPY file:51a441e6eceff49ef32609e7070b64e8d5690648e4f915cc825274e6fe37aed2 in /bin/registry 
# Thu, 17 Dec 2020 08:52:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 17 Dec 2020 08:52:12 GMT
VOLUME [/var/lib/registry]
# Thu, 17 Dec 2020 08:52:12 GMT
EXPOSE 5000
# Thu, 17 Dec 2020 08:52:13 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 17 Dec 2020 08:52:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 08:52:15 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354f1e88083af06aeab8d62885a9fc4837e4dd4df7401e88d2dad92cf5d3d380`  
		Last Modified: Thu, 17 Dec 2020 08:52:30 GMT  
		Size: 300.1 KB (300071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2dc4de40f59228ac116ecb91079d2619ad49846d335db1f936625f0f334313`  
		Last Modified: Thu, 17 Dec 2020 08:52:31 GMT  
		Size: 6.2 MB (6240199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d14370ba8f615dba79dd19dd77cfd5cb6bbf8594dd2720a7e75f114e392ff2`  
		Last Modified: Thu, 17 Dec 2020 08:52:30 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df0f8d558c48693436cf0dcb3f2d0c3cd49cc5ecd9fbf74333bd27a0f70884f`  
		Last Modified: Thu, 17 Dec 2020 08:52:29 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:2.7.1`

```console
$ docker pull registry@sha256:d5459fcb27aecc752520df4b492b08358a1912fcdfa454f7d2101d4b09991daa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `registry:2.7.1` - linux; amd64

```console
$ docker pull registry@sha256:a0dd61073ad21122e5f1517682800272ef29df52041aaea7ee29e92a5d22aa28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9938926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678dfa38fcfa349ccbdb1b6d52ac113ace67d5746794b36dfbad9dd96a9d1c43`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:13:59 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Thu, 17 Dec 2020 13:14:00 GMT
COPY file:21256ff7df5369f7ad2e19c6d020a644303aded200bdbec4d46648f38d55df78 in /bin/registry 
# Thu, 17 Dec 2020 13:14:00 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 17 Dec 2020 13:14:01 GMT
VOLUME [/var/lib/registry]
# Thu, 17 Dec 2020 13:14:01 GMT
EXPOSE 5000
# Thu, 17 Dec 2020 13:14:02 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:14:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:14:02 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d550a247d74fe258880d43f82ce0679ad2bef73b5833e3fc63e4326aa51c1418`  
		Last Modified: Thu, 17 Dec 2020 13:14:17 GMT  
		Size: 299.5 KB (299548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a938458ca360e0d59e750b7f55d786b0cdc54250a800d52d9000d601edb1505`  
		Last Modified: Thu, 17 Dec 2020 13:14:20 GMT  
		Size: 6.8 MB (6823928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd758c36fc9019145bd7e2f8222bc6abe8d864d727b79f9adade6ad2eccbf36`  
		Last Modified: Thu, 17 Dec 2020 13:14:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af6d68b484a730daaa243a546283a8c01db8c8e2cb28a9c114130bfc7b00e81`  
		Last Modified: Thu, 17 Dec 2020 13:14:17 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.7.1` - linux; arm variant v6

```console
$ docker pull registry@sha256:c8c97b4d572c33156da59bae82f6b833abf5ceaa69bb18d002406c2891fce4a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9312382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2126abe3746bfb8bd3bccc38ecc00d331a3bad9db38232c473ddf04e92c2078a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:52:08 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Thu, 17 Dec 2020 07:52:09 GMT
COPY file:29c6c1625420a558a03cc7ed253192f8138cba6212b64e30217fb6488af668e2 in /bin/registry 
# Thu, 17 Dec 2020 07:52:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 17 Dec 2020 07:52:12 GMT
VOLUME [/var/lib/registry]
# Thu, 17 Dec 2020 07:52:13 GMT
EXPOSE 5000
# Thu, 17 Dec 2020 07:52:14 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 17 Dec 2020 07:52:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 07:52:16 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7cc14966ceb5e5b46be135c16f21f7af42f270518ed92962f9514d0874ce7d`  
		Last Modified: Thu, 17 Dec 2020 07:52:29 GMT  
		Size: 299.9 KB (299919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96618f9c1a201fedc2049c85c36fc0b4a817442c4f712140f49d76310034d2f7`  
		Last Modified: Thu, 17 Dec 2020 07:52:33 GMT  
		Size: 6.4 MB (6391083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acb2c1463288a9621bede426350b5e343e6beb7639ab71ea9be3cd67599bb52`  
		Last Modified: Thu, 17 Dec 2020 07:52:28 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9b1ea70368acb9d8c55ea555a87c799805882309d54ad7af9aa7d8e1d8b366`  
		Last Modified: Thu, 17 Dec 2020 07:52:29 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:2.7.1` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:d42f9d2035ce5b9181ae8cc81d5646a2070a33c8125e21dc0d9e8dbddba97d69
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9266098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357aab9e21a8d6c2810a3fe7ad21db85d1a46a367aae3d4479d6c606810c3999`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:52:07 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Thu, 17 Dec 2020 08:52:09 GMT
COPY file:51a441e6eceff49ef32609e7070b64e8d5690648e4f915cc825274e6fe37aed2 in /bin/registry 
# Thu, 17 Dec 2020 08:52:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 17 Dec 2020 08:52:12 GMT
VOLUME [/var/lib/registry]
# Thu, 17 Dec 2020 08:52:12 GMT
EXPOSE 5000
# Thu, 17 Dec 2020 08:52:13 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 17 Dec 2020 08:52:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 08:52:15 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354f1e88083af06aeab8d62885a9fc4837e4dd4df7401e88d2dad92cf5d3d380`  
		Last Modified: Thu, 17 Dec 2020 08:52:30 GMT  
		Size: 300.1 KB (300071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2dc4de40f59228ac116ecb91079d2619ad49846d335db1f936625f0f334313`  
		Last Modified: Thu, 17 Dec 2020 08:52:31 GMT  
		Size: 6.2 MB (6240199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d14370ba8f615dba79dd19dd77cfd5cb6bbf8594dd2720a7e75f114e392ff2`  
		Last Modified: Thu, 17 Dec 2020 08:52:30 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df0f8d558c48693436cf0dcb3f2d0c3cd49cc5ecd9fbf74333bd27a0f70884f`  
		Last Modified: Thu, 17 Dec 2020 08:52:29 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `registry:latest`

```console
$ docker pull registry@sha256:d5459fcb27aecc752520df4b492b08358a1912fcdfa454f7d2101d4b09991daa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `registry:latest` - linux; amd64

```console
$ docker pull registry@sha256:a0dd61073ad21122e5f1517682800272ef29df52041aaea7ee29e92a5d22aa28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9938926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678dfa38fcfa349ccbdb1b6d52ac113ace67d5746794b36dfbad9dd96a9d1c43`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:13:59 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Thu, 17 Dec 2020 13:14:00 GMT
COPY file:21256ff7df5369f7ad2e19c6d020a644303aded200bdbec4d46648f38d55df78 in /bin/registry 
# Thu, 17 Dec 2020 13:14:00 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 17 Dec 2020 13:14:01 GMT
VOLUME [/var/lib/registry]
# Thu, 17 Dec 2020 13:14:01 GMT
EXPOSE 5000
# Thu, 17 Dec 2020 13:14:02 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 17 Dec 2020 13:14:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 13:14:02 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d550a247d74fe258880d43f82ce0679ad2bef73b5833e3fc63e4326aa51c1418`  
		Last Modified: Thu, 17 Dec 2020 13:14:17 GMT  
		Size: 299.5 KB (299548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a938458ca360e0d59e750b7f55d786b0cdc54250a800d52d9000d601edb1505`  
		Last Modified: Thu, 17 Dec 2020 13:14:20 GMT  
		Size: 6.8 MB (6823928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd758c36fc9019145bd7e2f8222bc6abe8d864d727b79f9adade6ad2eccbf36`  
		Last Modified: Thu, 17 Dec 2020 13:14:17 GMT  
		Size: 371.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af6d68b484a730daaa243a546283a8c01db8c8e2cb28a9c114130bfc7b00e81`  
		Last Modified: Thu, 17 Dec 2020 13:14:17 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm variant v6

```console
$ docker pull registry@sha256:c8c97b4d572c33156da59bae82f6b833abf5ceaa69bb18d002406c2891fce4a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9312382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2126abe3746bfb8bd3bccc38ecc00d331a3bad9db38232c473ddf04e92c2078a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:53 GMT
ADD file:e3a6f7566ee3c2ba61d27d801d3522e045a4be64a42f32ee52d933b68338d06f in / 
# Wed, 16 Dec 2020 23:49:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:52:08 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Thu, 17 Dec 2020 07:52:09 GMT
COPY file:29c6c1625420a558a03cc7ed253192f8138cba6212b64e30217fb6488af668e2 in /bin/registry 
# Thu, 17 Dec 2020 07:52:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 17 Dec 2020 07:52:12 GMT
VOLUME [/var/lib/registry]
# Thu, 17 Dec 2020 07:52:13 GMT
EXPOSE 5000
# Thu, 17 Dec 2020 07:52:14 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 17 Dec 2020 07:52:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 07:52:16 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:56fec67ad66eea034cf5b7d0d0ffd355c0fe87611bad132ac5a952fcaa52138b`  
		Last Modified: Wed, 16 Dec 2020 23:50:34 GMT  
		Size: 2.6 MB (2620769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7cc14966ceb5e5b46be135c16f21f7af42f270518ed92962f9514d0874ce7d`  
		Last Modified: Thu, 17 Dec 2020 07:52:29 GMT  
		Size: 299.9 KB (299919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96618f9c1a201fedc2049c85c36fc0b4a817442c4f712140f49d76310034d2f7`  
		Last Modified: Thu, 17 Dec 2020 07:52:33 GMT  
		Size: 6.4 MB (6391083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acb2c1463288a9621bede426350b5e343e6beb7639ab71ea9be3cd67599bb52`  
		Last Modified: Thu, 17 Dec 2020 07:52:28 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9b1ea70368acb9d8c55ea555a87c799805882309d54ad7af9aa7d8e1d8b366`  
		Last Modified: Thu, 17 Dec 2020 07:52:29 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `registry:latest` - linux; arm64 variant v8

```console
$ docker pull registry@sha256:d42f9d2035ce5b9181ae8cc81d5646a2070a33c8125e21dc0d9e8dbddba97d69
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9266098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:357aab9e21a8d6c2810a3fe7ad21db85d1a46a367aae3d4479d6c606810c3999`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["\/etc\/docker\/registry\/config.yml"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:52:07 GMT
RUN set -ex     && apk add --no-cache ca-certificates
# Thu, 17 Dec 2020 08:52:09 GMT
COPY file:51a441e6eceff49ef32609e7070b64e8d5690648e4f915cc825274e6fe37aed2 in /bin/registry 
# Thu, 17 Dec 2020 08:52:10 GMT
COPY file:4544cc1555469403b322faecc1cf1ca584667c43a6a60b17300f97840c04196e in /etc/docker/registry/config.yml 
# Thu, 17 Dec 2020 08:52:12 GMT
VOLUME [/var/lib/registry]
# Thu, 17 Dec 2020 08:52:12 GMT
EXPOSE 5000
# Thu, 17 Dec 2020 08:52:13 GMT
COPY file:507caa54f88c1f3862e5876e09a108b2083630ba24c57ad124e356a2de861d62 in /entrypoint.sh 
# Thu, 17 Dec 2020 08:52:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Dec 2020 08:52:15 GMT
CMD ["/etc/docker/registry/config.yml"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354f1e88083af06aeab8d62885a9fc4837e4dd4df7401e88d2dad92cf5d3d380`  
		Last Modified: Thu, 17 Dec 2020 08:52:30 GMT  
		Size: 300.1 KB (300071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e2dc4de40f59228ac116ecb91079d2619ad49846d335db1f936625f0f334313`  
		Last Modified: Thu, 17 Dec 2020 08:52:31 GMT  
		Size: 6.2 MB (6240199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d14370ba8f615dba79dd19dd77cfd5cb6bbf8594dd2720a7e75f114e392ff2`  
		Last Modified: Thu, 17 Dec 2020 08:52:30 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df0f8d558c48693436cf0dcb3f2d0c3cd49cc5ecd9fbf74333bd27a0f70884f`  
		Last Modified: Thu, 17 Dec 2020 08:52:29 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
