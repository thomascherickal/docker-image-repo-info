## `notary:server`

```console
$ docker pull notary@sha256:b62e9eaac0866fa1aedd8e6fb219d78abaa9f5f4be71df512ad47f54b1baec3f
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 11
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `notary:server` - linux; amd64

```console
$ docker pull notary@sha256:8f5d352ca53b00e5dab5670a7437ba24bc95a7a0286e4d06aaf9fcc9c9e5e05b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7957636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46df970ce60c11e12b6fac13fcec172a228263147a52aa5ce187700bf3d6ffde`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-server ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-server --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./server-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d7028a7a0470b3f4f0468ef1f0a22a687ad2f6d78190ff88d2a22b93617e1e9c`  
		Last Modified: Thu, 27 Jul 2023 01:03:48 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1c160cdac34b1ecc3b02fdc9e6c8c17bff48ab9e0421360709f5e95c760bd0c`  
		Last Modified: Thu, 27 Jul 2023 01:03:48 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c3bb5c71a64b8a4d1a0a05fcd1c987fae36b4e5b6d4a1e50f93bce6dfbbddeb`  
		Last Modified: Thu, 27 Jul 2023 01:03:48 GMT  
		Size: 5.1 MB (5147833 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b9ea3ed914da65dfd52f9ebfaf8ea90dd7f1f93d44a6f8f774b3285cc41b54f`  
		Last Modified: Thu, 27 Jul 2023 01:03:49 GMT  
		Size: 418.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:55dd62877e96605f8eb94c4dc146d0fb909f14d4b61a0021bbbb401c8ae278cc`  
		Last Modified: Thu, 27 Jul 2023 01:03:49 GMT  
		Size: 378.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:server` - unknown; unknown

```console
$ docker pull notary@sha256:f4fc7c9c94c4ff44a928fcfe7580bd50ced2927ec6a60ab5c466445c1f9b6262
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 KB (129942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:305362fea1e1455c4d71b9e952866a89e51c9da5f1e5d021ca6063245a4f4efb`

```dockerfile
```

-	Layers:
	-	`sha256:31cba255c78bf2e911d81feb62af927367876f062b89eb7442c220ea7713ac9d`  
		Last Modified: Thu, 27 Jul 2023 01:03:48 GMT  
		Size: 111.3 KB (111302 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ed47664990ce188441b513218e9d1b79c111ee8a8072909728dc2edb9cb14829`  
		Last Modified: Thu, 27 Jul 2023 18:30:50 GMT  
		Size: 18.6 KB (18640 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:6e8bfe3906aa1d8df858fedb86df50c8929f340bec233eecb2b9fc1a3a1b372c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7511249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:092a594d3d7141d38477de785ff80987f9be2d185aaedcce3e0c3250f90730f9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:321b24cc0fbd39caa2d7672a740d2cd2030ba99cab16f50c22db9955bd99350b in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-server ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-server --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./server-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:dffa980f71c953938bb194a457aa62e7f1885137331eef8bf7f9403c075f711c`  
		Last Modified: Mon, 07 Aug 2023 19:50:02 GMT  
		Size: 2.6 MB (2615553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253ae7f8eb52a8ea4fe35dad1a51da8e2507ed4a7de0e040345c7f1778fa3728`  
		Last Modified: Mon, 07 Aug 2023 22:58:38 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72255fa7488becd327879a87fb05f982b3f53af4b97cdb2194f25beea2d1b41e`  
		Last Modified: Mon, 07 Aug 2023 22:58:38 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d0e62fb7740d86658ba5c16a040fe749e2d555ba760003e42151ebb0693ce5`  
		Last Modified: Mon, 07 Aug 2023 22:58:39 GMT  
		Size: 4.9 MB (4893567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617b4a0f26a7a047066943504031862ddce8766b7d29f5e2b3ef46209605afaa`  
		Last Modified: Mon, 07 Aug 2023 22:58:38 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81a7366f32b9d9a19fb73ed36f1d2ba7151f7ca0d88269869654851ad496cac`  
		Last Modified: Mon, 07 Aug 2023 22:58:38 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:d147a2dd70b2bc88049efd0032dd9cc20e01aa0833db2bc1702b2775dab2baaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7444608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f672acd668849ed1cfdb5c5e3040dd835e50b024d9491c53c6136d9cddeaa3ee`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-server ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-server --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./server-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:202c4dd0f102d31afdf745598c8b608887eb3b4142b5fbb8619d8b431ab3d348`  
		Last Modified: Mon, 07 Aug 2023 22:45:27 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:565afe3e3634f553e5e4798c9171e212127f00b3c23c93faa1eb17c3027fad79`  
		Last Modified: Mon, 07 Aug 2023 22:45:27 GMT  
		Size: 118.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee6128cc3d34da4edf1351e0397480921013481a869739484a9b6366c2a03448`  
		Last Modified: Mon, 07 Aug 2023 22:45:27 GMT  
		Size: 4.7 MB (4734458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73788bca9233077876bfb7ad08ab7e664745b8945cc9734482694a0be8bbd5e4`  
		Last Modified: Mon, 07 Aug 2023 22:45:28 GMT  
		Size: 417.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dad868bcf088e64171900901ed63038b26bb0c717b90d360356dce16d10e14ee`  
		Last Modified: Mon, 07 Aug 2023 22:45:28 GMT  
		Size: 375.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:server` - unknown; unknown

```console
$ docker pull notary@sha256:7477d6f6d1f1ee16a7438db8a317f070ba5ee42856203c7e30e3d5fdb9d26831
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 KB (131099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7670e90ab99336561b98da07281dd5b929f251c5a9410088a2513f4a97f77776`

```dockerfile
```

-	Layers:
	-	`sha256:7f2db81d358b5d674541354c82bea5d03e60fdaf2cbfdfdd1fc5270c719cf0dc`  
		Last Modified: Mon, 07 Aug 2023 22:45:26 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:cb8d7756dfe0a4b3b1034a0bfef4ac485cd34a16982e7b522abd0eb9035008ce`  
		Last Modified: Mon, 07 Aug 2023 22:45:26 GMT  
		Size: 18.6 KB (18591 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:server` - linux; 386

```console
$ docker pull notary@sha256:3ab0146afdc08a6cedd9e9bab3234a7f1a8b703ec9f27a15f27965405aac893c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7763490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95cc5bc01d86f9854a1a0c6b443a91d701d641b863f75d00b863a4ba6c25e480`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:9b22a3b9a2009266eccfbbf15fbc348f6c854a6c496df29e5c4f0a832b796c67 in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-server ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-server --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./server-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:ca79a18e143c0859a7d07fda202e645a6564d97bbda6a486c576b234535bda07`  
		Last Modified: Wed, 14 Jun 2023 22:34:09 GMT  
		Size: 2.8 MB (2810568 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d22e634d8526e4aac68e19dd6e600ef04440199ca135213416d2994d42aaa694`  
		Last Modified: Mon, 31 Jul 2023 21:52:32 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5dcc9b16f9e2294397065c092feb15c6bff3d2665ba746bdcb523eca61e769`  
		Last Modified: Mon, 31 Jul 2023 21:52:32 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bfb6308179c62700b1c9951dee418223c0fa936ad90ced39bdbc05a9b1de1af`  
		Last Modified: Mon, 31 Jul 2023 21:52:32 GMT  
		Size: 5.0 MB (4950787 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:267f7e8a48931922a9b02cca2366ccf1d359bdcc692cc11835adabbc7559360a`  
		Last Modified: Mon, 31 Jul 2023 21:52:33 GMT  
		Size: 417.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53767a87d664452943b4d6145258a847bead98af4c3b4d8fb3c991ef12739c85`  
		Last Modified: Mon, 31 Jul 2023 21:52:33 GMT  
		Size: 377.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:server` - unknown; unknown

```console
$ docker pull notary@sha256:a9ec5704cff5e3989b4f08f5d7ff7dd3ed753d7cd0c900789eb9df6a873a5279
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 KB (19197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef07f1bf32ae8804b52370616232536577d285cf0369f32afc6d19f43cbcd3cb`

```dockerfile
```

-	Layers:
	-	`sha256:61be7c81b6c391ca577438528ca712fe6a8501e915fe227418f0d8981a2d0e23`  
		Last Modified: Mon, 31 Jul 2023 21:52:31 GMT  
		Size: 19.2 KB (19197 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:server` - linux; ppc64le

```console
$ docker pull notary@sha256:12ed046f61bd5dd764fc84eea6e721f4169f02b1793c4384a07ed15665d015c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7443542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f336378263104273fb3dd923316d91702f2f4a4d756e276b4dca4ff69a6c96`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-server ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-server --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./server-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:a2010c6a5435acd9b63d7f294696ba1d313d4393be0848195e1e655583ca50af`  
		Last Modified: Thu, 15 Jun 2023 00:40:48 GMT  
		Size: 2.8 MB (2802263 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60a044ed5c864c5a2d0d1678cfa0c098b4415a2f8da48cc5885ea9dd23a55532`  
		Last Modified: Mon, 31 Jul 2023 22:27:20 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3947c0f530864364e65ff3e91a31e87441834a8f5b9ab6bd1e4237d85686ec2b`  
		Last Modified: Mon, 31 Jul 2023 22:27:20 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e172d4d27418d2025397b27535c621639ad22b1836dc041da67cf4f4394ed1f`  
		Last Modified: Mon, 31 Jul 2023 22:27:21 GMT  
		Size: 4.6 MB (4639151 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:31d38b68a51471f58deb0bfe46f70de2f69d6d4df239a03fbbd2047a391f4e28`  
		Last Modified: Mon, 31 Jul 2023 22:27:21 GMT  
		Size: 416.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f23bf7d44cb904ea6e8ab0f359575da4812dc7d6cb8022c48da7f4741aab6c1`  
		Last Modified: Mon, 31 Jul 2023 22:27:22 GMT  
		Size: 373.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:server` - unknown; unknown

```console
$ docker pull notary@sha256:0850b3c1ad874a30c79b101c369ecc5afc140159e5baec82695901d01e207e5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 KB (130544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca122f3391d80f3aabe90666ab70de53223c1287a3540c638c24dec959f1501d`

```dockerfile
```

-	Layers:
	-	`sha256:7401f0cba80351c9d6fa83d278e2959e729bd85e14a4abaa9a4a57f8ee535e80`  
		Last Modified: Mon, 31 Jul 2023 22:27:20 GMT  
		Size: 111.0 KB (111037 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0b40acd6e0916fb73f9ede6e4cab57037cf8e944ff7830ceaaaf240fad1539aa`  
		Last Modified: Mon, 31 Jul 2023 22:27:20 GMT  
		Size: 19.5 KB (19507 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:d51a1b38c5cf6e84bcd6f7cb2ff40eb62c3b5b420b36348f2c7b3bc1dadb9722
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7570356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da9276fcf57624659541e43b27859259402be783b05542eca324c0cf3ccf83fd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:16daa03175f0a8d874128d0c563e183e127bce1094ec72183deec297c28e021d in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/server
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-server ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-server --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./server-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:835f3b5b8d7d281d273a2dce84bab3df0d219e423e2de23b10fd920f68b5a40e`  
		Last Modified: Thu, 15 Jun 2023 05:31:54 GMT  
		Size: 2.6 MB (2591727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30b8eeb6b3ae61a803c9ab5f7e760889fff22e517a6aaaacd5feae7e35b06b47`  
		Last Modified: Mon, 31 Jul 2023 22:21:30 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b0e9f2d60d8e307889f552cfc39c53ce222fa4d55d4e9573d688ca912895d3e9`  
		Last Modified: Mon, 31 Jul 2023 22:21:30 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:85a0b76422048e84259bc099fe3b9dad3a28bc710b43f6de25910b1df13e7206`  
		Last Modified: Mon, 31 Jul 2023 22:21:31 GMT  
		Size: 5.0 MB (4976495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8d4eca0de24a2fa6b26847e5fe25c2c8f03ad461c9b6316576b9d618b169c65`  
		Last Modified: Mon, 31 Jul 2023 22:21:31 GMT  
		Size: 419.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22515c264fd9572272419bfe1fd8b547572f751b7074751a1eee14b7787e345f`  
		Last Modified: Mon, 31 Jul 2023 22:21:31 GMT  
		Size: 378.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:server` - unknown; unknown

```console
$ docker pull notary@sha256:bbf4bee420853b8ea7affb7bd1c018a55a876e3e3800c6f65e99308d4b8ae969
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 KB (129593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d4c20cf71d802380c74ddb291ffa560de3d6ecf8847ad2b248169a32b804c5`

```dockerfile
```

-	Layers:
	-	`sha256:ea771afa76d108f7ce06334a9cc6fa99fa4d793a7c6b32a4a0b0b222330b1035`  
		Last Modified: Mon, 31 Jul 2023 22:21:30 GMT  
		Size: 111.0 KB (110954 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2f2b9ff8e12a7c38384818bf84ef8f2e527fbd4f11090f92f16716e35778908f`  
		Last Modified: Mon, 31 Jul 2023 22:21:30 GMT  
		Size: 18.6 KB (18639 bytes)  
		MIME: application/vnd.in-toto+json
