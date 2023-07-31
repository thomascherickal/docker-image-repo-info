<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `notary`

-	[`notary:server`](#notaryserver)
-	[`notary:server-0.7.0`](#notaryserver-070)
-	[`notary:signer`](#notarysigner)
-	[`notary:signer-0.7.0`](#notarysigner-070)

## `notary:server`

```console
$ docker pull notary@sha256:e6d36c62657b25bffdde8daac4944ab1da797dd0e43df6279f1ad0e71c46a729
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
$ docker pull notary@sha256:fb8208933cbf79e738454a623da26380adf775a8a5745d35b20e842d9c3116a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7511268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cbf35b31ab6513f3a7728521a367909f1a284a50c92b09366207857d0298e92`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:41a85835978e4acba9d92833f0d5e20084da50779e52d8832d576b003a7aa1bb in / 
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
	-	`sha256:053f9b31dd2e619ba14dc3733515fcd65e92851f612b94453db88ea1d27ab0ea`  
		Last Modified: Wed, 14 Jun 2023 18:50:10 GMT  
		Size: 2.6 MB (2615570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc088f39d60a97a6a5a0805fb7780188b0b1f2360675f7aa332c0cc037f16998`  
		Last Modified: Mon, 31 Jul 2023 22:25:15 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a513cb8f8760a8bad1a296cb91d3be5f7abd467bd3d40e94b0eb5d2a1407b8`  
		Last Modified: Mon, 31 Jul 2023 22:25:13 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50649b7cea824b9946cc777afe21942b74fd66a00c256e86ae04f73654b46283`  
		Last Modified: Mon, 31 Jul 2023 22:25:14 GMT  
		Size: 4.9 MB (4893567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a30593649da2881d0fdd7a45d0f5d7fc63306f7d45a73d7993dd10011e6db1c`  
		Last Modified: Mon, 31 Jul 2023 22:25:13 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5ed5d75897930fa343db0e4b335bbe87dfbd5b0134794b8db3e0ded8cef965`  
		Last Modified: Mon, 31 Jul 2023 22:25:13 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:64487efefca6c6d16d80f474c3bb49868f83bb4cf6f1758738a4606a93c5ecb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7444481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d738b1a73a0f005baf4caf23ffdcb9801510f63838b76405abbeb33eee337e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
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
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd268b404cb321ea63f6e8843d1e48cfb00da239533b0fa2d06c9b4d3f73b541`  
		Last Modified: Mon, 31 Jul 2023 16:30:44 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb1575d470bc983965a771f9e4f29612496f8ceacc07473e0b4320477436202f`  
		Last Modified: Mon, 31 Jul 2023 16:30:44 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8ea7fd7743c4a0a67ecafc0208f64e55e44ad87c5122e631f481145da60aa9be`  
		Last Modified: Mon, 31 Jul 2023 16:30:45 GMT  
		Size: 4.7 MB (4734446 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3120615d081efc87f51f3413ce2d6af31f259041238c49fddff47739981aa43c`  
		Last Modified: Mon, 31 Jul 2023 16:30:45 GMT  
		Size: 417.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32fb6d8b2f16eb9bf586ac2620128c9aab4efe0748ce2e9c74d4a49de44a4bda`  
		Last Modified: Mon, 31 Jul 2023 16:30:45 GMT  
		Size: 374.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:server` - unknown; unknown

```console
$ docker pull notary@sha256:a59629db419eb765933d4866804b2e8c95e5ce420ae8a132555cc6170b9eabfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 KB (130771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30b5421d8404e754486bac753306ac1a5e6182340f332607654653bede3a2c14`

```dockerfile
```

-	Layers:
	-	`sha256:11147348af8395fbbaacdc6841444a441cb712cc70d669df3b4f46b244bfab02`  
		Last Modified: Mon, 31 Jul 2023 16:30:44 GMT  
		Size: 111.3 KB (111304 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:94747e1faaabd679dd216d057da4ed98a60b39db143de323eb565253c7d10a9e`  
		Last Modified: Mon, 31 Jul 2023 16:30:44 GMT  
		Size: 19.5 KB (19467 bytes)  
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

## `notary:server-0.7.0`

```console
$ docker pull notary@sha256:e6d36c62657b25bffdde8daac4944ab1da797dd0e43df6279f1ad0e71c46a729
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
$ docker pull notary@sha256:fb8208933cbf79e738454a623da26380adf775a8a5745d35b20e842d9c3116a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7511268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cbf35b31ab6513f3a7728521a367909f1a284a50c92b09366207857d0298e92`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:41a85835978e4acba9d92833f0d5e20084da50779e52d8832d576b003a7aa1bb in / 
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
	-	`sha256:053f9b31dd2e619ba14dc3733515fcd65e92851f612b94453db88ea1d27ab0ea`  
		Last Modified: Wed, 14 Jun 2023 18:50:10 GMT  
		Size: 2.6 MB (2615570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc088f39d60a97a6a5a0805fb7780188b0b1f2360675f7aa332c0cc037f16998`  
		Last Modified: Mon, 31 Jul 2023 22:25:15 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a513cb8f8760a8bad1a296cb91d3be5f7abd467bd3d40e94b0eb5d2a1407b8`  
		Last Modified: Mon, 31 Jul 2023 22:25:13 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50649b7cea824b9946cc777afe21942b74fd66a00c256e86ae04f73654b46283`  
		Last Modified: Mon, 31 Jul 2023 22:25:14 GMT  
		Size: 4.9 MB (4893567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a30593649da2881d0fdd7a45d0f5d7fc63306f7d45a73d7993dd10011e6db1c`  
		Last Modified: Mon, 31 Jul 2023 22:25:13 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5ed5d75897930fa343db0e4b335bbe87dfbd5b0134794b8db3e0ded8cef965`  
		Last Modified: Mon, 31 Jul 2023 22:25:13 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:64487efefca6c6d16d80f474c3bb49868f83bb4cf6f1758738a4606a93c5ecb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7444481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d738b1a73a0f005baf4caf23ffdcb9801510f63838b76405abbeb33eee337e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
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
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd268b404cb321ea63f6e8843d1e48cfb00da239533b0fa2d06c9b4d3f73b541`  
		Last Modified: Mon, 31 Jul 2023 16:30:44 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb1575d470bc983965a771f9e4f29612496f8ceacc07473e0b4320477436202f`  
		Last Modified: Mon, 31 Jul 2023 16:30:44 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8ea7fd7743c4a0a67ecafc0208f64e55e44ad87c5122e631f481145da60aa9be`  
		Last Modified: Mon, 31 Jul 2023 16:30:45 GMT  
		Size: 4.7 MB (4734446 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3120615d081efc87f51f3413ce2d6af31f259041238c49fddff47739981aa43c`  
		Last Modified: Mon, 31 Jul 2023 16:30:45 GMT  
		Size: 417.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32fb6d8b2f16eb9bf586ac2620128c9aab4efe0748ce2e9c74d4a49de44a4bda`  
		Last Modified: Mon, 31 Jul 2023 16:30:45 GMT  
		Size: 374.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:server-0.7.0` - unknown; unknown

```console
$ docker pull notary@sha256:a59629db419eb765933d4866804b2e8c95e5ce420ae8a132555cc6170b9eabfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 KB (130771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30b5421d8404e754486bac753306ac1a5e6182340f332607654653bede3a2c14`

```dockerfile
```

-	Layers:
	-	`sha256:11147348af8395fbbaacdc6841444a441cb712cc70d669df3b4f46b244bfab02`  
		Last Modified: Mon, 31 Jul 2023 16:30:44 GMT  
		Size: 111.3 KB (111304 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:94747e1faaabd679dd216d057da4ed98a60b39db143de323eb565253c7d10a9e`  
		Last Modified: Mon, 31 Jul 2023 16:30:44 GMT  
		Size: 19.5 KB (19467 bytes)  
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

### `notary:server-0.7.0` - unknown; unknown

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

### `notary:server-0.7.0` - linux; s390x

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

### `notary:server-0.7.0` - unknown; unknown

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

## `notary:signer`

```console
$ docker pull notary@sha256:adbeb780e7d6e0cf9b40dc14ffef7129e8d5f67d812058cbc787c9cd7bb87723
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

### `notary:signer` - linux; amd64

```console
$ docker pull notary@sha256:e8599ff16babc2df1eacd517037bcb99b13e9c604cb949065c2fec9f5195bd64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b763659f7f9787164d6b87db1c3e8cacfaba9e919e2854f62c257f08e211c9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4444/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[7899/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-signer ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-signer --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./signer-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:29cf034d6e8ff3398b8061c5e0c5022fc1a8a315bb09d50f005413e9005313de`  
		Last Modified: Thu, 27 Jul 2023 01:06:57 GMT  
		Size: 117.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aedd335e680d05675f7d6064192254774d5aa83a5da38431ab7d84d0f9050094`  
		Last Modified: Thu, 27 Jul 2023 01:06:57 GMT  
		Size: 4.8 MB (4763094 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f6911346eea87c92024187efa5cf53c2e1cecf79d38f2e4705e08b7e7dce22d1`  
		Last Modified: Thu, 27 Jul 2023 01:06:57 GMT  
		Size: 349.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f7d069ef182b851234447ad822fb582930ed40fd0db8d07c044a2942f63ca24`  
		Last Modified: Thu, 27 Jul 2023 01:06:57 GMT  
		Size: 371.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:signer` - unknown; unknown

```console
$ docker pull notary@sha256:310081e9689c2223edb0b642551a64f03da1902100ba1242668fbaa1e5d581dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 KB (123918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7966101f0ea25b6e2e64b6f75e0c7388fb3d344a6b8dc6556e3b392469e61674`

```dockerfile
```

-	Layers:
	-	`sha256:122f346b38d2041fbec98d0a42fe70837934b8c5f86d92e31e7e0a57495df627`  
		Last Modified: Thu, 27 Jul 2023 01:06:57 GMT  
		Size: 105.3 KB (105262 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:be0a83490630d2b8bd9f10602bbd4bbdaebacbacb688d3a21e75a67a659b15b3`  
		Last Modified: Thu, 27 Jul 2023 18:31:05 GMT  
		Size: 18.7 KB (18656 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:85ca8c07234ed12692fcfc0b0544fc0c72281d717d0d37ac5460d6f4fd4f12db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02ee362e35160cc03d43698f8943ba3ecfc2b552f31fe402a5cb738236d13e79`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:41a85835978e4acba9d92833f0d5e20084da50779e52d8832d576b003a7aa1bb in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4444/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[7899/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-signer ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-signer --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./signer-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:053f9b31dd2e619ba14dc3733515fcd65e92851f612b94453db88ea1d27ab0ea`  
		Last Modified: Wed, 14 Jun 2023 18:50:10 GMT  
		Size: 2.6 MB (2615570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc088f39d60a97a6a5a0805fb7780188b0b1f2360675f7aa332c0cc037f16998`  
		Last Modified: Mon, 31 Jul 2023 22:25:15 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc12745e10c1a181ced7dab8ff555cf4ed7fa4f7f7a3fa73fef5e6b7fd349808`  
		Last Modified: Mon, 31 Jul 2023 22:25:37 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66a62b42df3386acf28da6bbaf7404ff49eff9100c8afae13bbdde735e9f4b9`  
		Last Modified: Mon, 31 Jul 2023 22:25:38 GMT  
		Size: 4.5 MB (4526080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961af7eecfc17e0cb487ba2fc979334b176dc3022fa1a61f8169c85be2f078b8`  
		Last Modified: Mon, 31 Jul 2023 22:25:37 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f81fc243c1dd1db656074f15e79b694e5368dd9103f4e9221342d16c4bf0f15`  
		Last Modified: Mon, 31 Jul 2023 22:25:37 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:4dce322bc04ae80c70e649dd881da12954b9fa339dcadf45fada0ad0ebb273a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7103033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc9495eaca4d98b84e08d87c28eeab932e019aacb89030a3c1b6f3715ae03eb9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4444/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[7899/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-signer ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-signer --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./signer-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd268b404cb321ea63f6e8843d1e48cfb00da239533b0fa2d06c9b4d3f73b541`  
		Last Modified: Mon, 31 Jul 2023 16:30:44 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e8bb61657f23c0e41753fa77b1044cb7d8d062503b3f35a5d071c486832a3d5`  
		Last Modified: Mon, 31 Jul 2023 18:28:10 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4958b2100ed765baf3ffc8dbb3b559ee13c416a8466f10487e984352642d8c94`  
		Last Modified: Mon, 31 Jul 2023 18:28:11 GMT  
		Size: 4.4 MB (4393067 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b31e14b8df4b8dfc19f6fcf664b42d3950c91760468f0d21accaf884d3baaebb`  
		Last Modified: Mon, 31 Jul 2023 18:28:10 GMT  
		Size: 350.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d1ba07a8a4d10c9ad1b92401961655f36ad4dd213fbae0e76c6b2c1d85975977`  
		Last Modified: Mon, 31 Jul 2023 18:28:10 GMT  
		Size: 372.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:signer` - unknown; unknown

```console
$ docker pull notary@sha256:2af97bd7e12f7b9d9caae777c543a0344999c271966b8e2d734237c182b65db9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 KB (123926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04007ade78aba22dac26703f1f18f9c9b7913ab2b431378ea18934acf73683a0`

```dockerfile
```

-	Layers:
	-	`sha256:fc18a829a9b69c165dae13a3870750fc4bdd1716b729cd4756fe4c7690896116`  
		Last Modified: Mon, 31 Jul 2023 18:28:10 GMT  
		Size: 105.3 KB (105264 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:af8b8112676af72a462cbef8f522f07c2a4767f3dea70653f040d03b95707a33`  
		Last Modified: Mon, 31 Jul 2023 18:28:10 GMT  
		Size: 18.7 KB (18662 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:5d83b8a507aca8cb212c7c708ebf0d2238c7b73d5bd86d4d1e6cfbc232cc2a0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7391652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36cf70ca02cf1a3293a8c159d14038fb1ccaf30a0cbfe18ae9a880765377e7b3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:9b22a3b9a2009266eccfbbf15fbc348f6c854a6c496df29e5c4f0a832b796c67 in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4444/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[7899/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-signer ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-signer --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./signer-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:ca79a18e143c0859a7d07fda202e645a6564d97bbda6a486c576b234535bda07`  
		Last Modified: Wed, 14 Jun 2023 22:34:09 GMT  
		Size: 2.8 MB (2810568 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17854043c5f29df129c2d07ef8b2bbbfb7f0395350d17b96f343ac46cc8af4ce`  
		Last Modified: Mon, 31 Jul 2023 21:55:12 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec1b469efcbc9e798d0dfa53284a09f81c6902fb1cc419ef542947639f5e39f6`  
		Last Modified: Mon, 31 Jul 2023 21:55:12 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8cfef48348f5651562dba8e722ab25881576c82d6d20629f57761ba200d891e9`  
		Last Modified: Mon, 31 Jul 2023 21:55:12 GMT  
		Size: 4.6 MB (4579015 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d43d56bef3fb444f6226d1299810149e70f3654d4c25b774ae162991f664e572`  
		Last Modified: Mon, 31 Jul 2023 21:55:13 GMT  
		Size: 355.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:766d195d340afb9b359203d7eee1873893324710712db412063ba01f40d4a278`  
		Last Modified: Mon, 31 Jul 2023 21:55:13 GMT  
		Size: 376.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:signer` - unknown; unknown

```console
$ docker pull notary@sha256:8feb4a0d6602651b1d94a9f957c92abafacba26645a41e2194af6ec80b0bcd71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 KB (19213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc041a6a305b79c438628b447ceefeb0d7df30c185d9f6026a38fdd678f83b45`

```dockerfile
```

-	Layers:
	-	`sha256:349d6c32d2c9156fcd47167e03b2ada6601c77b0102561bf94ed48953a80c9d8`  
		Last Modified: Mon, 31 Jul 2023 21:55:12 GMT  
		Size: 19.2 KB (19213 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:e93b927b443bf3e7d028b8d8b30520d1780fe07738f75ff8e18325c7c55cc0b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7101320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbd9d25b356e9364be835143fe56a32d17254b1b760d460b0767512086e11cd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4444/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[7899/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-signer ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-signer --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./signer-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:7c24f5411ee5e3f0b7e0a90b8f41269a12c46679cea19b390613be835c8c6de7`  
		Last Modified: Mon, 31 Jul 2023 22:27:52 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd8219ac3ddf5e0119ccb0bd6914ece183f87c511ee4c2c25315f90b3235b6eb`  
		Last Modified: Mon, 31 Jul 2023 22:27:52 GMT  
		Size: 4.3 MB (4296992 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:030eaf2823dd4d54d7a80fbdf251994faddcdd6ef6d47cc28f6f500144883b7d`  
		Last Modified: Mon, 31 Jul 2023 22:27:52 GMT  
		Size: 351.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a3fbf36a7068a8976d289fdb444024320b88462fa08f17c2ff1c4c628a9b33e`  
		Last Modified: Mon, 31 Jul 2023 22:27:52 GMT  
		Size: 375.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:signer` - unknown; unknown

```console
$ docker pull notary@sha256:a03b4649b02b6ff12e52dae62aa48cf18d45f5be752edfbb6248b3554b0caa82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 KB (123592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc7330281978c94648403b16ba13e0fb839dd22ce5e7eb8f591bd512dd613697`

```dockerfile
```

-	Layers:
	-	`sha256:c643721736376e2fe7f5f6e29845882a04a3fb71b196c76719e3aa323ae0c306`  
		Last Modified: Mon, 31 Jul 2023 22:27:52 GMT  
		Size: 104.9 KB (104890 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:cefa77db89a75f9c7a6ba6f9afdff5085a2b5f14eb9a13898646ac4e9863a7e5`  
		Last Modified: Mon, 31 Jul 2023 22:27:52 GMT  
		Size: 18.7 KB (18702 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:8cecc02bf92609cda71cd2f8acdd66b84110e03ddd01908d7acedb7814e20db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7200480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:382f6875b25d4e4bdcbe6f2cff5944dc1798400ea69f9b0b5af6228d18117195`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:16daa03175f0a8d874128d0c563e183e127bce1094ec72183deec297c28e021d in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4444/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[7899/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-signer ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-signer --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./signer-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:f2632e9f75f65dddb5b0520ecfca9796acf5318a6ed61e1c9068a3cf7614901c`  
		Last Modified: Mon, 31 Jul 2023 22:21:54 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e7bb426845f42b6da8f6bf06aa4b747975c287d77032862013f6c961e9276610`  
		Last Modified: Mon, 31 Jul 2023 22:21:54 GMT  
		Size: 4.6 MB (4606693 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:66e0449a27c77fa5c51017fa3477fcfc44a72938bc262ce1d7c3bfc800bf521b`  
		Last Modified: Mon, 31 Jul 2023 22:21:54 GMT  
		Size: 351.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d2df8ddf078c89e914057fcadd76163a2875cf4c22b1caeb4b5e8534f181ffd`  
		Last Modified: Mon, 31 Jul 2023 22:21:54 GMT  
		Size: 372.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:signer` - unknown; unknown

```console
$ docker pull notary@sha256:d21ebabaef229c4a90960dca2428bbb65092b8312b4d4b25cdcb5d2e233b8acb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 KB (123456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e270a05ff3f4224af9aa39628b1adef39ba5be7b7c977d03e858e98802ec2377`

```dockerfile
```

-	Layers:
	-	`sha256:71b5a71980dc9079d24dea4f388d2505262990f913bedd07027a5385a14ea4d9`  
		Last Modified: Mon, 31 Jul 2023 22:21:54 GMT  
		Size: 104.8 KB (104801 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:411f05598c4f323b51d4ba8d1aa376ec10c56ad9799fcb736d37673f9634e881`  
		Last Modified: Mon, 31 Jul 2023 22:21:54 GMT  
		Size: 18.7 KB (18655 bytes)  
		MIME: application/vnd.in-toto+json

## `notary:signer-0.7.0`

```console
$ docker pull notary@sha256:adbeb780e7d6e0cf9b40dc14ffef7129e8d5f67d812058cbc787c9cd7bb87723
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

### `notary:signer-0.7.0` - linux; amd64

```console
$ docker pull notary@sha256:e8599ff16babc2df1eacd517037bcb99b13e9c604cb949065c2fec9f5195bd64
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0b763659f7f9787164d6b87db1c3e8cacfaba9e919e2854f62c257f08e211c9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4444/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[7899/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-signer ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-signer --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./signer-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:29cf034d6e8ff3398b8061c5e0c5022fc1a8a315bb09d50f005413e9005313de`  
		Last Modified: Thu, 27 Jul 2023 01:06:57 GMT  
		Size: 117.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aedd335e680d05675f7d6064192254774d5aa83a5da38431ab7d84d0f9050094`  
		Last Modified: Thu, 27 Jul 2023 01:06:57 GMT  
		Size: 4.8 MB (4763094 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f6911346eea87c92024187efa5cf53c2e1cecf79d38f2e4705e08b7e7dce22d1`  
		Last Modified: Thu, 27 Jul 2023 01:06:57 GMT  
		Size: 349.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f7d069ef182b851234447ad822fb582930ed40fd0db8d07c044a2942f63ca24`  
		Last Modified: Thu, 27 Jul 2023 01:06:57 GMT  
		Size: 371.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:signer-0.7.0` - unknown; unknown

```console
$ docker pull notary@sha256:310081e9689c2223edb0b642551a64f03da1902100ba1242668fbaa1e5d581dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 KB (123918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7966101f0ea25b6e2e64b6f75e0c7388fb3d344a6b8dc6556e3b392469e61674`

```dockerfile
```

-	Layers:
	-	`sha256:122f346b38d2041fbec98d0a42fe70837934b8c5f86d92e31e7e0a57495df627`  
		Last Modified: Thu, 27 Jul 2023 01:06:57 GMT  
		Size: 105.3 KB (105262 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:be0a83490630d2b8bd9f10602bbd4bbdaebacbacb688d3a21e75a67a659b15b3`  
		Last Modified: Thu, 27 Jul 2023 18:31:05 GMT  
		Size: 18.7 KB (18656 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:signer-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:85ca8c07234ed12692fcfc0b0544fc0c72281d717d0d37ac5460d6f4fd4f12db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02ee362e35160cc03d43698f8943ba3ecfc2b552f31fe402a5cb738236d13e79`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:41a85835978e4acba9d92833f0d5e20084da50779e52d8832d576b003a7aa1bb in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4444/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[7899/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-signer ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-signer --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./signer-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:053f9b31dd2e619ba14dc3733515fcd65e92851f612b94453db88ea1d27ab0ea`  
		Last Modified: Wed, 14 Jun 2023 18:50:10 GMT  
		Size: 2.6 MB (2615570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc088f39d60a97a6a5a0805fb7780188b0b1f2360675f7aa332c0cc037f16998`  
		Last Modified: Mon, 31 Jul 2023 22:25:15 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc12745e10c1a181ced7dab8ff555cf4ed7fa4f7f7a3fa73fef5e6b7fd349808`  
		Last Modified: Mon, 31 Jul 2023 22:25:37 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66a62b42df3386acf28da6bbaf7404ff49eff9100c8afae13bbdde735e9f4b9`  
		Last Modified: Mon, 31 Jul 2023 22:25:38 GMT  
		Size: 4.5 MB (4526080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961af7eecfc17e0cb487ba2fc979334b176dc3022fa1a61f8169c85be2f078b8`  
		Last Modified: Mon, 31 Jul 2023 22:25:37 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f81fc243c1dd1db656074f15e79b694e5368dd9103f4e9221342d16c4bf0f15`  
		Last Modified: Mon, 31 Jul 2023 22:25:37 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:4dce322bc04ae80c70e649dd881da12954b9fa339dcadf45fada0ad0ebb273a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7103033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc9495eaca4d98b84e08d87c28eeab932e019aacb89030a3c1b6f3715ae03eb9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4444/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[7899/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-signer ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-signer --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./signer-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd268b404cb321ea63f6e8843d1e48cfb00da239533b0fa2d06c9b4d3f73b541`  
		Last Modified: Mon, 31 Jul 2023 16:30:44 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e8bb61657f23c0e41753fa77b1044cb7d8d062503b3f35a5d071c486832a3d5`  
		Last Modified: Mon, 31 Jul 2023 18:28:10 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4958b2100ed765baf3ffc8dbb3b559ee13c416a8466f10487e984352642d8c94`  
		Last Modified: Mon, 31 Jul 2023 18:28:11 GMT  
		Size: 4.4 MB (4393067 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b31e14b8df4b8dfc19f6fcf664b42d3950c91760468f0d21accaf884d3baaebb`  
		Last Modified: Mon, 31 Jul 2023 18:28:10 GMT  
		Size: 350.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d1ba07a8a4d10c9ad1b92401961655f36ad4dd213fbae0e76c6b2c1d85975977`  
		Last Modified: Mon, 31 Jul 2023 18:28:10 GMT  
		Size: 372.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:signer-0.7.0` - unknown; unknown

```console
$ docker pull notary@sha256:2af97bd7e12f7b9d9caae777c543a0344999c271966b8e2d734237c182b65db9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.9 KB (123926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04007ade78aba22dac26703f1f18f9c9b7913ab2b431378ea18934acf73683a0`

```dockerfile
```

-	Layers:
	-	`sha256:fc18a829a9b69c165dae13a3870750fc4bdd1716b729cd4756fe4c7690896116`  
		Last Modified: Mon, 31 Jul 2023 18:28:10 GMT  
		Size: 105.3 KB (105264 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:af8b8112676af72a462cbef8f522f07c2a4767f3dea70653f040d03b95707a33`  
		Last Modified: Mon, 31 Jul 2023 18:28:10 GMT  
		Size: 18.7 KB (18662 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:signer-0.7.0` - linux; 386

```console
$ docker pull notary@sha256:5d83b8a507aca8cb212c7c708ebf0d2238c7b73d5bd86d4d1e6cfbc232cc2a0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7391652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36cf70ca02cf1a3293a8c159d14038fb1ccaf30a0cbfe18ae9a880765377e7b3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:9b22a3b9a2009266eccfbbf15fbc348f6c854a6c496df29e5c4f0a832b796c67 in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4444/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[7899/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-signer ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-signer --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./signer-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:ca79a18e143c0859a7d07fda202e645a6564d97bbda6a486c576b234535bda07`  
		Last Modified: Wed, 14 Jun 2023 22:34:09 GMT  
		Size: 2.8 MB (2810568 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17854043c5f29df129c2d07ef8b2bbbfb7f0395350d17b96f343ac46cc8af4ce`  
		Last Modified: Mon, 31 Jul 2023 21:55:12 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec1b469efcbc9e798d0dfa53284a09f81c6902fb1cc419ef542947639f5e39f6`  
		Last Modified: Mon, 31 Jul 2023 21:55:12 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8cfef48348f5651562dba8e722ab25881576c82d6d20629f57761ba200d891e9`  
		Last Modified: Mon, 31 Jul 2023 21:55:12 GMT  
		Size: 4.6 MB (4579015 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d43d56bef3fb444f6226d1299810149e70f3654d4c25b774ae162991f664e572`  
		Last Modified: Mon, 31 Jul 2023 21:55:13 GMT  
		Size: 355.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:766d195d340afb9b359203d7eee1873893324710712db412063ba01f40d4a278`  
		Last Modified: Mon, 31 Jul 2023 21:55:13 GMT  
		Size: 376.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:signer-0.7.0` - unknown; unknown

```console
$ docker pull notary@sha256:8feb4a0d6602651b1d94a9f957c92abafacba26645a41e2194af6ec80b0bcd71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.2 KB (19213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc041a6a305b79c438628b447ceefeb0d7df30c185d9f6026a38fdd678f83b45`

```dockerfile
```

-	Layers:
	-	`sha256:349d6c32d2c9156fcd47167e03b2ada6601c77b0102561bf94ed48953a80c9d8`  
		Last Modified: Mon, 31 Jul 2023 21:55:12 GMT  
		Size: 19.2 KB (19213 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:signer-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:e93b927b443bf3e7d028b8d8b30520d1780fe07738f75ff8e18325c7c55cc0b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7101320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbd9d25b356e9364be835143fe56a32d17254b1b760d460b0767512086e11cd`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4444/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[7899/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-signer ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-signer --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./signer-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:7c24f5411ee5e3f0b7e0a90b8f41269a12c46679cea19b390613be835c8c6de7`  
		Last Modified: Mon, 31 Jul 2023 22:27:52 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd8219ac3ddf5e0119ccb0bd6914ece183f87c511ee4c2c25315f90b3235b6eb`  
		Last Modified: Mon, 31 Jul 2023 22:27:52 GMT  
		Size: 4.3 MB (4296992 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:030eaf2823dd4d54d7a80fbdf251994faddcdd6ef6d47cc28f6f500144883b7d`  
		Last Modified: Mon, 31 Jul 2023 22:27:52 GMT  
		Size: 351.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a3fbf36a7068a8976d289fdb444024320b88462fa08f17c2ff1c4c628a9b33e`  
		Last Modified: Mon, 31 Jul 2023 22:27:52 GMT  
		Size: 375.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:signer-0.7.0` - unknown; unknown

```console
$ docker pull notary@sha256:a03b4649b02b6ff12e52dae62aa48cf18d45f5be752edfbb6248b3554b0caa82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.6 KB (123592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc7330281978c94648403b16ba13e0fb839dd22ce5e7eb8f591bd512dd613697`

```dockerfile
```

-	Layers:
	-	`sha256:c643721736376e2fe7f5f6e29845882a04a3fb71b196c76719e3aa323ae0c306`  
		Last Modified: Mon, 31 Jul 2023 22:27:52 GMT  
		Size: 104.9 KB (104890 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:cefa77db89a75f9c7a6ba6f9afdff5085a2b5f14eb9a13898646ac4e9863a7e5`  
		Last Modified: Mon, 31 Jul 2023 22:27:52 GMT  
		Size: 18.7 KB (18702 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:signer-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:8cecc02bf92609cda71cd2f8acdd66b84110e03ddd01908d7acedb7814e20db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7200480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:382f6875b25d4e4bdcbe6f2cff5944dc1798400ea69f9b0b5af6228d18117195`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 24 Oct 2022 22:10:44 GMT
ADD file:16daa03175f0a8d874128d0c563e183e127bce1094ec72183deec297c28e021d in / 
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["/bin/sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[4444/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
EXPOSE map[7899/tcp:{}]
# Mon, 24 Oct 2022 22:10:44 GMT
ENV INSTALLDIR=/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
WORKDIR /notary/signer
# Mon, 24 Oct 2022 22:10:44 GMT
COPY /notary-signer ./ # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
RUN ./notary-signer --version # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./signer-config.json . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 24 Oct 2022 22:10:44 GMT
USER notary
# Mon, 24 Oct 2022 22:10:44 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 24 Oct 2022 22:10:44 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:f2632e9f75f65dddb5b0520ecfca9796acf5318a6ed61e1c9068a3cf7614901c`  
		Last Modified: Mon, 31 Jul 2023 22:21:54 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e7bb426845f42b6da8f6bf06aa4b747975c287d77032862013f6c961e9276610`  
		Last Modified: Mon, 31 Jul 2023 22:21:54 GMT  
		Size: 4.6 MB (4606693 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:66e0449a27c77fa5c51017fa3477fcfc44a72938bc262ce1d7c3bfc800bf521b`  
		Last Modified: Mon, 31 Jul 2023 22:21:54 GMT  
		Size: 351.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d2df8ddf078c89e914057fcadd76163a2875cf4c22b1caeb4b5e8534f181ffd`  
		Last Modified: Mon, 31 Jul 2023 22:21:54 GMT  
		Size: 372.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:signer-0.7.0` - unknown; unknown

```console
$ docker pull notary@sha256:d21ebabaef229c4a90960dca2428bbb65092b8312b4d4b25cdcb5d2e233b8acb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 KB (123456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e270a05ff3f4224af9aa39628b1adef39ba5be7b7c977d03e858e98802ec2377`

```dockerfile
```

-	Layers:
	-	`sha256:71b5a71980dc9079d24dea4f388d2505262990f913bedd07027a5385a14ea4d9`  
		Last Modified: Mon, 31 Jul 2023 22:21:54 GMT  
		Size: 104.8 KB (104801 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:411f05598c4f323b51d4ba8d1aa376ec10c56ad9799fcb736d37673f9634e881`  
		Last Modified: Mon, 31 Jul 2023 22:21:54 GMT  
		Size: 18.7 KB (18655 bytes)  
		MIME: application/vnd.in-toto+json
