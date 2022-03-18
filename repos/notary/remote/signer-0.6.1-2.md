## `notary:signer-0.6.1-2`

```console
$ docker pull notary@sha256:10f02909863a5be5c9fdda953f9ef68a5c989c013d76930a417246b97f6d4398
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:signer-0.6.1-2` - linux; amd64

```console
$ docker pull notary@sha256:7cd15517d615b5af1cda1296f28a31a50d463d2ec4e66d47807ea963a5a9ae0a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7688823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c6cc8c94cf061e07d741926ded6f6345780868f1d598e31e86ca4f1e5182a0c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 18:03:57 GMT
ENV TAG=v0.6.1
# Thu, 17 Mar 2022 18:03:57 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 17 Mar 2022 18:04:20 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 17 Mar 2022 18:04:20 GMT
EXPOSE 4444
# Thu, 17 Mar 2022 18:04:20 GMT
EXPOSE 7899
# Thu, 17 Mar 2022 18:04:20 GMT
WORKDIR /notary/signer
# Thu, 17 Mar 2022 18:04:46 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Thu, 17 Mar 2022 18:04:46 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Thu, 17 Mar 2022 18:04:47 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Thu, 17 Mar 2022 18:04:48 GMT
RUN adduser -D -H -g "" notary
# Thu, 17 Mar 2022 18:04:48 GMT
USER notary
# Thu, 17 Mar 2022 18:04:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 17 Mar 2022 18:04:48 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 17 Mar 2022 18:04:48 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9f5ddc70ebf753823067c484e479e7525c999e2864663475e73ef49c4b7fbb`  
		Last Modified: Thu, 17 Mar 2022 18:05:21 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1631c06e13bed06385f804bdaed5bb983016e85648f3e580a79a34961697a6`  
		Last Modified: Thu, 17 Mar 2022 18:05:22 GMT  
		Size: 4.9 MB (4869589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d5aaab4e07d0b7bc2e43648cc06fb718e82ef12812eecc98cf986fe7f33f3b`  
		Last Modified: Thu, 17 Mar 2022 18:05:21 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55c99bb7ce6b42af8b1a6729f77f6a758f6a9bf6a3e0cca9d5aa6f5ebc38b18`  
		Last Modified: Thu, 17 Mar 2022 18:05:21 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8bc1d1d60e2d7a3d67e21f60aabf81d07d762d0f3ff0bd446f36a9ee1c81ad`  
		Last Modified: Thu, 17 Mar 2022 18:05:21 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; arm variant v6

```console
$ docker pull notary@sha256:f02b6731b76ee5f30e5863716264c5040ed35f6cae02a3d3689305d9bc7d7598
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7185127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b2d35e37ca0a874a961232379a5f754678d48cdd957b46c2f7742b3031e3b73`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:48:36 GMT
ENV TAG=v0.6.1
# Thu, 17 Mar 2022 15:48:37 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 17 Mar 2022 15:49:20 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 17 Mar 2022 15:49:20 GMT
EXPOSE 4444
# Thu, 17 Mar 2022 15:49:21 GMT
EXPOSE 7899
# Thu, 17 Mar 2022 15:49:21 GMT
WORKDIR /notary/signer
# Thu, 17 Mar 2022 15:49:45 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Thu, 17 Mar 2022 15:49:45 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Thu, 17 Mar 2022 15:49:46 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Thu, 17 Mar 2022 15:49:47 GMT
RUN adduser -D -H -g "" notary
# Thu, 17 Mar 2022 15:49:48 GMT
USER notary
# Thu, 17 Mar 2022 15:49:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 17 Mar 2022 15:49:49 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 17 Mar 2022 15:49:49 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0219162766422e3078573c2bedb3e58a6c382a030a341c0bb5cc7c809483e5`  
		Last Modified: Thu, 17 Mar 2022 15:50:37 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0baa806a6307efe203e4cc07104f988519047d5e54e588eabd17413a65ac63`  
		Last Modified: Thu, 17 Mar 2022 15:50:41 GMT  
		Size: 4.6 MB (4555144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2df18c0e7de69a12d8ed338050d124adb610886e7f132f89b534dc9f4ff08a7`  
		Last Modified: Thu, 17 Mar 2022 15:50:37 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9666ead86a141412e43831ebd717f9899d1d3d36f5d97cc878be13cb584916e`  
		Last Modified: Thu, 17 Mar 2022 15:50:37 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7f77d2a1cb189e2a82c3566cee8a48f598a6ba6209f5c562ae8c63de3c721e`  
		Last Modified: Thu, 17 Mar 2022 15:50:37 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:6fefe152b56505b59cfd4e97cebbfd7514d1e8685dc9810c756f79fa6f697c9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7182203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ade0436dde6056ffa83df7107a2af83084291618c1e1d4749b943e2b42f0250`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 00:13:38 GMT
ENV TAG=v0.6.1
# Sat, 13 Nov 2021 00:13:39 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 13 Nov 2021 00:14:09 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 13 Nov 2021 00:14:10 GMT
EXPOSE 4444
# Sat, 13 Nov 2021 00:14:11 GMT
EXPOSE 7899
# Sat, 13 Nov 2021 00:14:12 GMT
WORKDIR /notary/signer
# Sat, 13 Nov 2021 00:14:25 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Sat, 13 Nov 2021 00:14:27 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 13 Nov 2021 00:14:28 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 13 Nov 2021 00:14:28 GMT
RUN adduser -D -H -g "" notary
# Sat, 13 Nov 2021 00:14:29 GMT
USER notary
# Sat, 13 Nov 2021 00:14:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 13 Nov 2021 00:14:31 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 13 Nov 2021 00:14:32 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73c68a67445be4c877ecd7986db3857403f81b0cbe4b276300309b7c953d1bd`  
		Last Modified: Sat, 13 Nov 2021 00:15:04 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8ad0750bbda32429d887e25820911a19ef9034a569020bae511ba5425fd7f9`  
		Last Modified: Sat, 13 Nov 2021 00:15:05 GMT  
		Size: 4.5 MB (4460538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb140f321bcfa502e9644d0bbdefa46dbb3c613c4d15846be69394dbf49bdef`  
		Last Modified: Sat, 13 Nov 2021 00:15:04 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c4c1544d842ec5effc5fa006170c896ffc224754c701b25c089d89caa2bfae`  
		Last Modified: Sat, 13 Nov 2021 00:15:04 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97f073fab2f7a16c2b02d0032b3a3b108086dca2d0b8f1c9beb95630caa5888`  
		Last Modified: Sat, 13 Nov 2021 00:15:05 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; 386

```console
$ docker pull notary@sha256:4a58e6eea69fc848388dca7dde14d188a2a18b0d2620cdfd6282272df75833ed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7439304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8340a2ee214549fc9e94e989998d45bae9c8482b9cf0b432915d05b67a6182`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Thu, 17 Mar 2022 16:34:42 GMT
ADD file:fbbd764c2b3ce734329c4dc8415d55b9cefc972125c5818e78698f7b894667da in / 
# Thu, 17 Mar 2022 16:34:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 17:41:31 GMT
ENV TAG=v0.6.1
# Thu, 17 Mar 2022 17:41:31 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 17 Mar 2022 17:41:56 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 17 Mar 2022 17:41:56 GMT
EXPOSE 4444
# Thu, 17 Mar 2022 17:41:56 GMT
EXPOSE 7899
# Thu, 17 Mar 2022 17:41:56 GMT
WORKDIR /notary/signer
# Thu, 17 Mar 2022 17:42:12 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Thu, 17 Mar 2022 17:42:12 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Thu, 17 Mar 2022 17:42:12 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Thu, 17 Mar 2022 17:42:13 GMT
RUN adduser -D -H -g "" notary
# Thu, 17 Mar 2022 17:42:13 GMT
USER notary
# Thu, 17 Mar 2022 17:42:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 17 Mar 2022 17:42:13 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 17 Mar 2022 17:42:13 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:4fcf0d6f8c0dc4a27651b1a8218d9febdd0bc510d8a2eb8474b17c87b284c5bd`  
		Last Modified: Thu, 17 Mar 2022 16:35:37 GMT  
		Size: 2.8 MB (2823620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1800e6030f10698439ecde415e5169e45ca3eb886931118fc651de44d7637c`  
		Last Modified: Thu, 17 Mar 2022 17:42:42 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c68a8fa51239b848bd66fbbfda090af0b66341751596346f45352975adac82`  
		Last Modified: Thu, 17 Mar 2022 17:42:44 GMT  
		Size: 4.6 MB (4613629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58dc787e48344b2073d46b54410c0d2a97e0fe9f7d6d7d114159cb63e49ad28`  
		Last Modified: Thu, 17 Mar 2022 17:42:43 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e64a61270a9c3d9a5633f5e17128ba6ad7714efad23c49584c00b7078119f88`  
		Last Modified: Thu, 17 Mar 2022 17:42:52 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8330c46595a8570d280a38cfa426e8a0d232b9944ef7ef7974aadc03fd79931d`  
		Last Modified: Thu, 17 Mar 2022 17:42:42 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; ppc64le

```console
$ docker pull notary@sha256:493607ba1fada0e01470e66ad860d24f4b7e8d01d2dc9dba65dd4272d0813604
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7165484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeb36cabaf3c6d9bba0bf5fe0bd64343f835b76426767942092c51f35a975a3f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:25 GMT
ADD file:f7216323de17450e653f77c86d2c1e2e8ec01e1133e93f29c515761b3e9d8f7d in / 
# Fri, 12 Nov 2021 21:18:28 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 02:54:59 GMT
ENV TAG=v0.6.1
# Sat, 13 Nov 2021 02:55:04 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Sat, 13 Nov 2021 02:56:54 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 13 Nov 2021 02:56:57 GMT
EXPOSE 4444
# Sat, 13 Nov 2021 02:57:00 GMT
EXPOSE 7899
# Sat, 13 Nov 2021 02:57:04 GMT
WORKDIR /notary/signer
# Sat, 13 Nov 2021 02:57:39 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Sat, 13 Nov 2021 02:57:44 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 13 Nov 2021 02:57:47 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 13 Nov 2021 02:58:05 GMT
RUN adduser -D -H -g "" notary
# Sat, 13 Nov 2021 02:58:12 GMT
USER notary
# Sat, 13 Nov 2021 02:58:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 13 Nov 2021 02:58:25 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 13 Nov 2021 02:58:30 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:6729720a3e6b58511df148134bb67d786ad90f9fce1c02ba5bbfd31f33055fbe`  
		Last Modified: Fri, 12 Nov 2021 21:19:49 GMT  
		Size: 2.8 MB (2820517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7806fed2d41d0755760e6717030f6aff9dc6d5c219ba7ea8e88bfeeb3104cb`  
		Last Modified: Sat, 13 Nov 2021 02:59:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17710bd31fffde751d347e6748a7dd6331b87678096d7c238c71873df8248dfe`  
		Last Modified: Sat, 13 Nov 2021 02:59:16 GMT  
		Size: 4.3 MB (4342905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8eb937120684e6a942598df616956feda3303abc0057aaf5a8d5eba3ed2fb3f`  
		Last Modified: Sat, 13 Nov 2021 02:59:15 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d6a82b8624c31634f38037f0a9d099bec7394379cb4d40a7cd1ca6ae8692bc`  
		Last Modified: Sat, 13 Nov 2021 02:59:15 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b175ad475b545323f1204fc8ad650e37b0fdfb2d3027b91bd6c54079dbf7bdf9`  
		Last Modified: Sat, 13 Nov 2021 02:59:15 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.6.1-2` - linux; s390x

```console
$ docker pull notary@sha256:8e1a224c239605e0b3ff0e45299f029fa955adbea193bd0f18e2416ac23bdd20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7314919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d12aa8a2e10c86edbd24bd1d6caf4956f278e2e2dbaad55593c0a56cc7b87414`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--help"]`

```dockerfile
# Thu, 17 Mar 2022 14:36:02 GMT
ADD file:cc3c2ea972c5b5d1135d0a82f5d1a6cc97fcc81f3006bb6c6b8580f1e9f4c238 in / 
# Thu, 17 Mar 2022 14:36:02 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 16:48:38 GMT
ENV TAG=v0.6.1
# Thu, 17 Mar 2022 16:48:39 GMT
ENV NOTARYPKG=github.com/theupdateframework/notary
# Thu, 17 Mar 2022 16:48:59 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 17 Mar 2022 16:48:59 GMT
EXPOSE 4444
# Thu, 17 Mar 2022 16:48:59 GMT
EXPOSE 7899
# Thu, 17 Mar 2022 16:48:59 GMT
WORKDIR /notary/signer
# Thu, 17 Mar 2022 16:49:10 GMT
RUN set -eux;     apk add --no-cache --virtual build-deps git go make musl-dev;     export GOPATH=/go GOCACHE=/go/cache;     mkdir -p ${GOPATH}/src/${NOTARYPKG};     git clone -b ${TAG} --depth 1 https://${NOTARYPKG} ${GOPATH}/src/${NOTARYPKG};     make -C ${GOPATH}/src/${NOTARYPKG} SKIPENVCHECK=1 PREFIX=. ./bin/static/notary-signer;     cp -vL ${GOPATH}/src/${NOTARYPKG}/bin/static/notary-signer ./;     apk del --no-network build-deps;     rm -rf ${GOPATH};     ./notary-signer --help
# Thu, 17 Mar 2022 16:49:10 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Thu, 17 Mar 2022 16:49:10 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Thu, 17 Mar 2022 16:49:11 GMT
RUN adduser -D -H -g "" notary
# Thu, 17 Mar 2022 16:49:11 GMT
USER notary
# Thu, 17 Mar 2022 16:49:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 17 Mar 2022 16:49:11 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 17 Mar 2022 16:49:11 GMT
CMD ["notary-signer" "--help"]
```

-	Layers:
	-	`sha256:3bb5875ccb136d6c7691dcf2927e52a66c831ce80fd5140d92e0a158400a4cfe`  
		Last Modified: Thu, 17 Mar 2022 14:36:53 GMT  
		Size: 2.6 MB (2606212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c965ece0ded347f0522934cfa75df1d2e16714a9443dcc7f5d38b0b7af8041b`  
		Last Modified: Thu, 17 Mar 2022 16:49:37 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dff2e6efbb33014d9f833e935ad719dff7dc9e6c074fac6b629b815030c2056`  
		Last Modified: Thu, 17 Mar 2022 16:49:38 GMT  
		Size: 4.7 MB (4706649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefeffb3ff1831061255068b4e6cba2f0d39ae66375ed18a45d5d52f44e70e4b`  
		Last Modified: Thu, 17 Mar 2022 16:49:37 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55341d4f63ac695e765283a65696d4267e5f55c448e28d93414c41d61d89883`  
		Last Modified: Thu, 17 Mar 2022 16:49:37 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39329f747ee8ad6602f00a8158f4ab462f51553147a651aedb5f1e763f6279b0`  
		Last Modified: Thu, 17 Mar 2022 16:49:37 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
