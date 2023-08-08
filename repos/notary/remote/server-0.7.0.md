## `notary:server-0.7.0`

```console
$ docker pull notary@sha256:497f67ada517229cef8861dc0f3b6868d1a4b3b5c9ed23317f4244f78d52c148
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

### `notary:server-0.7.0` - linux; amd64

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

### `notary:server-0.7.0` - unknown; unknown

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

### `notary:server-0.7.0` - linux; arm variant v6

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

### `notary:server-0.7.0` - linux; arm64 variant v8

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

### `notary:server-0.7.0` - unknown; unknown

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

### `notary:server-0.7.0` - linux; 386

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

### `notary:server-0.7.0` - unknown; unknown

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

### `notary:server-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:45ca8fd4de3a1b8c6981d7237f9158a14fc29ec22d2d67510f40fe775a2a8faf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7443614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af28e6b9b522a35047a4261ae895a906716441751c1a9176f9190c582373947`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:b30c2945bf4c873440b2e390c7120f16abe08ec41b10c2fb248b9b1a7ad223fa in / 
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
	-	`sha256:cc1a557f8d111cc8c11359cd168abb441e150c9dc42a046349c5e51132461a47`  
		Last Modified: Mon, 07 Aug 2023 20:17:53 GMT  
		Size: 2.8 MB (2802326 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c4d9f67868be443e2c2f090de7caea30272fbfa297b89c353c3ad9a3047b1b6`  
		Last Modified: Tue, 08 Aug 2023 01:08:52 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6a142ff761db1df086e666a3b69b35cd4106e93592f900cc3b76d2d76b1399f`  
		Last Modified: Tue, 08 Aug 2023 01:08:51 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:23852e81f7d884e270dc9bda64a0a19667821e912203466850d3487407ab148e`  
		Last Modified: Tue, 08 Aug 2023 01:08:52 GMT  
		Size: 4.6 MB (4639154 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5494c8e99bfc8addd3828ed280ef3c9c3217d35aeb79e08acda6ec04c1d59cd1`  
		Last Modified: Tue, 08 Aug 2023 01:08:53 GMT  
		Size: 420.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f2d6c9532ca0f0dab6d785d1823407632bb7512b524b8d12c75ccca39b02d357`  
		Last Modified: Tue, 08 Aug 2023 01:08:53 GMT  
		Size: 377.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:server-0.7.0` - unknown; unknown

```console
$ docker pull notary@sha256:d1fb1aad865534d7c9d3566b083fc8ddda2011f05cda2c1f324aca2610d4f74e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 KB (129658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06831e0701a211bf080e17fac7a7f847ff085bd6f78ab144fe54154ec8b1cd42`

```dockerfile
```

-	Layers:
	-	`sha256:6e489af8319856f95d152d089b630904d98de7ca0ec332cfb5ebe99d0c5d07c7`  
		Last Modified: Tue, 08 Aug 2023 01:08:52 GMT  
		Size: 111.0 KB (111037 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c4b40f82604a7b5b336f5c78d151441e55a091350857b2f2c23e9e31ca1ea655`  
		Last Modified: Tue, 08 Aug 2023 01:08:52 GMT  
		Size: 18.6 KB (18621 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:server-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:d1e72c424482060b7779d9776023874287d059644af495a94f9bf7d30493830f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7570354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5547bc15c32a972261ced143dc05c99cabc078586b07defc03eae161bf6cf804`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:39bfe995aa06bc953f4887751caefaa4576f3dfe63f0020b8989bb8b0a09c28f in / 
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
	-	`sha256:e5761c1ed80af1ea48f655cdeb0fa9a89fe7d3903985d9ea08286e940a4f30dd`  
		Last Modified: Mon, 07 Aug 2023 19:42:55 GMT  
		Size: 2.6 MB (2591728 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f55e3cbca2287bf936764f7cf3d3b0b4e12e954928cb0652b427c0f83cf162c`  
		Last Modified: Tue, 08 Aug 2023 05:26:46 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8e593822092e94f68a1e55cc1042d360e1c590ab8447d859122cc25a9456787`  
		Last Modified: Tue, 08 Aug 2023 05:26:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ddf217811d8edc379710881aceac7ba3e7175bd8336398e8a11b3788234625b6`  
		Last Modified: Tue, 08 Aug 2023 05:26:46 GMT  
		Size: 5.0 MB (4976495 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:483c151497f6252ea96df4ac234160917d6911427d6798c993e6a9a427268439`  
		Last Modified: Tue, 08 Aug 2023 05:26:47 GMT  
		Size: 419.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:33b2097a71fe86b39696fea28da91125bc63c807b7bc6f41c05e9e0dc5d822c8`  
		Last Modified: Tue, 08 Aug 2023 05:26:47 GMT  
		Size: 378.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:server-0.7.0` - unknown; unknown

```console
$ docker pull notary@sha256:fb77e4dd3502ffc5c54c1cb0591edbed7380639afd707853add98178dd0dc275
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 KB (129571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dec5c91ed119d8fb3bb1c8a96e4dafa5ea1dff3ef9b63cf0f8ae727054f21079`

```dockerfile
```

-	Layers:
	-	`sha256:972ad4fcfc8a5ed75d3268d0c7ea754f81e48e9497c5890c15174e715a0d8b8f`  
		Last Modified: Tue, 08 Aug 2023 05:26:46 GMT  
		Size: 111.0 KB (110986 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3946524db89d6bde663b41e48a85762a20c6e1963750f78fc04b86adf78fef00`  
		Last Modified: Tue, 08 Aug 2023 05:26:46 GMT  
		Size: 18.6 KB (18585 bytes)  
		MIME: application/vnd.in-toto+json
