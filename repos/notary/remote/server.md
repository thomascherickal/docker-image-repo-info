## `notary:server`

```console
$ docker pull notary@sha256:ccfabff9cb2beb4f56aa55743d7b3220e5779f8ac64185506ca878c1847b1018
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
$ docker pull notary@sha256:29fb83361d437d4698dd71e56546ba1fbcd2df36cdb1e9b626c555a83a0e4d92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7957659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39e81a68d6bf45f5905246fddb18ae4056d80ee19dcd7969da1562ae235583bb`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
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
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ea910673cb007c738d4370eeab62b64baaccc940e09fb3b653de03ebf1f6503`  
		Last Modified: Tue, 17 Oct 2023 20:01:20 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2aedeb4989c8b40b58b9e81be652f3c59e93f1d65b742747098ddc19e14ba00c`  
		Last Modified: Tue, 17 Oct 2023 20:01:20 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfee6149d49b6fde822181048539fdfacf1099ea4dced794e484cf7d94f700f3`  
		Last Modified: Tue, 17 Oct 2023 20:01:20 GMT  
		Size: 5.1 MB (5147841 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf5b976d0c7b47bd7ce0f4e55edb09c0419d8d7d2bcdedb6dc60a52f08b6dee3`  
		Last Modified: Tue, 17 Oct 2023 20:01:20 GMT  
		Size: 418.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0121fb7db1309fa742c1a765de3709e9941c2ef2cbb8ee591dd690ee6d684ce`  
		Last Modified: Tue, 17 Oct 2023 20:01:21 GMT  
		Size: 377.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:server` - unknown; unknown

```console
$ docker pull notary@sha256:df8943904b8c68318490457575b68963b44f5b0167b6001fbb073f7aac204324
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 KB (110724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f46c0d28d54d812258ffb69afefcc995f8e7f410a9c27235078db9b9a66d023`

```dockerfile
```

-	Layers:
	-	`sha256:ff8c5a30154c1f3d930cb67169075887885f6555d68ecc4482a68d64fbc4e7b2`  
		Last Modified: Tue, 17 Oct 2023 20:01:20 GMT  
		Size: 91.5 KB (91494 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d5686a74e06b8231826b22fc56150e27d9d081ee52973f24e2959d5819441fe4`  
		Last Modified: Tue, 17 Oct 2023 20:01:20 GMT  
		Size: 19.2 KB (19230 bytes)  
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
$ docker pull notary@sha256:2dde0ea7564373ff977abd5a03af7adae5459d7bfca5e8106f7f8cbd4abe5462
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 KB (109918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5164b3b1e32bde933e4f3fb90aa6b0cc87ef8a2f1a28b66470fd7528e973ab43`

```dockerfile
```

-	Layers:
	-	`sha256:c5e21a9ebe71e38ee55dfa7571bd14d011af379320ec54dfbea371c42ddba1ba`  
		Last Modified: Tue, 17 Oct 2023 20:05:04 GMT  
		Size: 91.5 KB (91503 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:30b40bcdcaceed0964ba033068a0997859daa570f689c80a594c44c40ace101d`  
		Last Modified: Tue, 17 Oct 2023 20:05:04 GMT  
		Size: 18.4 KB (18415 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:server` - linux; 386

```console
$ docker pull notary@sha256:9d3d4b1aa6185b8da72a0e97e7a8a4156287ce89479edc87f77633ded278e567
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7763475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f1ead4bf0ac898f792abd5585cb36385ee20dc3d39e6cb78a436dc4829c565`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:c06b4f6991638e506d4d0a4d70c4a78ba30b971767802af4c6b837cdf59d4303 in / 
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
	-	`sha256:be0d19c155de823c6b37eaaba7cdec9085e8f1e39b1dd5982a19acb6c8c97cc5`  
		Last Modified: Mon, 07 Aug 2023 19:39:20 GMT  
		Size: 2.8 MB (2810553 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26f5e07cf5dd2ddef185d26fcd872c6ea88a977881e1ae912091ac7e0c58352a`  
		Last Modified: Tue, 17 Oct 2023 18:59:59 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:284bb3fb32d977ba57e02dd08118bff966afe825f4fdf6077ef41b8133bd8128`  
		Last Modified: Tue, 17 Oct 2023 18:59:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9bed0c7971721a02c14ed33f5192db014c950291eb24de851fdaf1f8e8514163`  
		Last Modified: Tue, 17 Oct 2023 19:00:00 GMT  
		Size: 5.0 MB (4950790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd2c554b9ba2aa841b79ec575972569cdb690ee928dc74a607600c9ef2943094`  
		Last Modified: Tue, 17 Oct 2023 18:59:59 GMT  
		Size: 417.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22abeb4c57a42516cce9452f32a3da9f0be57623f5c8d3f459024a76fd0f79bb`  
		Last Modified: Tue, 17 Oct 2023 19:00:00 GMT  
		Size: 376.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:server` - unknown; unknown

```console
$ docker pull notary@sha256:e153fe40e9c6609781db699d49882ba1ba3b5601d6924e4ead6ec278d02d651a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.0 KB (18986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b322c21f5f52b15e50942a957fdd2457c4edb0908c3758bbf12d67844e4831a3`

```dockerfile
```

-	Layers:
	-	`sha256:ae75b198267a3c988fd304e1eed6c176324f92c3c08808c146879b901b618edf`  
		Last Modified: Tue, 17 Oct 2023 18:59:59 GMT  
		Size: 19.0 KB (18986 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:server` - linux; ppc64le

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

### `notary:server` - unknown; unknown

```console
$ docker pull notary@sha256:af2f77d8884ae489f552085ffd8638becd99444f9c27dadb88724aedbcb9765a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 KB (108041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07d08b9032cbfce25674a1feec921abc2979739150457bd6e59d9a34a40d919d`

```dockerfile
```

-	Layers:
	-	`sha256:abe44435533137bcc6c8b02697b59e0754aa7d499bd376bc5a73c6b2b88082c4`  
		Last Modified: Tue, 17 Oct 2023 19:00:14 GMT  
		Size: 89.6 KB (89596 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bf5ed658a666ffb02e4a4c43e52f1d260e6d320197b51e9b9c4605050cb5d465`  
		Last Modified: Tue, 17 Oct 2023 19:00:14 GMT  
		Size: 18.4 KB (18445 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:server` - linux; s390x

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

### `notary:server` - unknown; unknown

```console
$ docker pull notary@sha256:81f4310b12759f0b7036f150776b7b31374616ee4ab2263dfe38c1887fb9017b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 KB (107971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fcc3b305e1a2608ca0e535fb96a843c955236e38f15efc63a1eab7b3d79a9b0`

```dockerfile
```

-	Layers:
	-	`sha256:115780dc1d4bb9826cbb9b89e6a100e2537216c4850c4ee5f8f5725536c2bb82`  
		Last Modified: Tue, 17 Oct 2023 18:59:15 GMT  
		Size: 89.6 KB (89562 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:438d8e2a6ba50440e24c8137a0d9c78741df51253a35e69be8fa60bcea1ee10c`  
		Last Modified: Tue, 17 Oct 2023 18:59:15 GMT  
		Size: 18.4 KB (18409 bytes)  
		MIME: application/vnd.in-toto+json
