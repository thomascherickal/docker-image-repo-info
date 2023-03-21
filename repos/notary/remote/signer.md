## `notary:signer`

```console
$ docker pull notary@sha256:05c0d65fe189cfb50c494f3accdea6b5a6caf6c474f6cc4f3aef3342201685d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:signer` - linux; amd64

```console
$ docker pull notary@sha256:c251779f1417ae5a5ee417d2d30e686eabbbb8de059978fa36f37aad9946b69f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7571275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b0be1197a26a971e5761cf8ccd7b56756b8d45fcaccf0193ffd72e852d107f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 10:15:51 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 10:16:14 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 11 Feb 2023 10:16:14 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 11 Feb 2023 10:16:14 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 11 Feb 2023 10:16:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 11 Feb 2023 10:16:14 GMT
WORKDIR /notary/signer
# Wed, 08 Mar 2023 00:49:22 GMT
COPY /notary-signer ./ # buildkit
# Wed, 08 Mar 2023 00:49:23 GMT
RUN ./notary-signer --version # buildkit
# Wed, 08 Mar 2023 00:49:23 GMT
COPY ./signer-config.json . # buildkit
# Wed, 08 Mar 2023 00:49:23 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:49:23 GMT
USER notary
# Wed, 08 Mar 2023 00:49:23 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:49:23 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a8bf9348133d1e770b90e9991d3f65c555075470962fb5e1321cf7201947a6`  
		Last Modified: Sat, 11 Feb 2023 10:16:25 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0208e6d213823747dbf355ecd6e4879b414b1413e219476f0ffa3791d92aade7`  
		Last Modified: Sat, 11 Feb 2023 10:16:33 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d4813226483e6e0e68e4703b12d04bf207dd1e73af737985a819e977cf180b`  
		Last Modified: Wed, 08 Mar 2023 00:49:41 GMT  
		Size: 4.8 MB (4761343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fe5ef8141b6313f5d7afeb9c50c6567fe00bd4c6c5525f0b083735b3735dd6`  
		Last Modified: Wed, 08 Mar 2023 00:49:40 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18688d46ffe85cf58379eff4073d0f279e209261cb80dcc23b613698bacc134`  
		Last Modified: Wed, 08 Mar 2023 00:49:40 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e0a2298e2263fef9565a3cf84018cadde98b1f0ec959259993a6654fcc6579`  
		Last Modified: Wed, 08 Mar 2023 00:49:40 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:6216b68394c7b4e65f20eb11cad25ac367c0478004def016247f5d7597da696c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f92b4b68b3a717c29b9a43adbaa0bee16844e3aa91f027fd94fd9aa0b8037262`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 00:16:13 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 08 Mar 2023 00:16:43 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 08 Mar 2023 00:16:43 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 08 Mar 2023 00:16:43 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 08 Mar 2023 00:16:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 08 Mar 2023 00:16:43 GMT
WORKDIR /notary/signer
# Mon, 13 Mar 2023 22:40:43 GMT
COPY /notary-signer ./ # buildkit
# Mon, 13 Mar 2023 22:40:43 GMT
RUN ./notary-signer --version # buildkit
# Mon, 13 Mar 2023 22:40:43 GMT
COPY ./signer-config.json . # buildkit
# Mon, 13 Mar 2023 22:40:43 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 13 Mar 2023 22:40:43 GMT
USER notary
# Mon, 13 Mar 2023 22:40:43 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 13 Mar 2023 22:40:43 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b05793ac14c68387ad3a34fa8d5d4136f040e8b820b1eee3595d30529d87e46`  
		Last Modified: Wed, 08 Mar 2023 00:17:02 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8867bd3aa695c936397740852a2a23245f7a8147431da0dea7ea79cb52c3fb7`  
		Last Modified: Wed, 08 Mar 2023 00:17:12 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9d6f44471853d748615de79835f860dbaf6a96899425bfe41892a55b8bbc82`  
		Last Modified: Mon, 13 Mar 2023 22:41:10 GMT  
		Size: 4.5 MB (4524257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a29049d4e5f31919a6825670eff28003d1d6a5e8a1a0db07cb80c508d56339`  
		Last Modified: Mon, 13 Mar 2023 22:41:09 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0e82b1ac8c1d3b1d7406e09d51ada3c9d5eef0b16c90412117a62e19a79f64`  
		Last Modified: Mon, 13 Mar 2023 22:41:09 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97710136b3555e60fb404524d8523f81cc0860b525a91fa4bef04700c7b55915`  
		Last Modified: Mon, 13 Mar 2023 22:41:09 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:ed2230bebee769c527fad6a0573eedc33301a45bd3796e689d15264b0bfee8bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7101670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc4b332df6d7a1d49a93bf4106d687f0e5274b77b1fdf9fe622c2b33a3230c9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Tue, 07 Mar 2023 23:45:55 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 07 Mar 2023 23:45:55 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 07 Mar 2023 23:45:55 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 07 Mar 2023 23:45:55 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 07 Mar 2023 23:45:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 07 Mar 2023 23:45:55 GMT
WORKDIR /notary/signer
# Tue, 07 Mar 2023 23:45:55 GMT
COPY /notary-signer ./ # buildkit
# Tue, 07 Mar 2023 23:45:55 GMT
RUN ./notary-signer --version # buildkit
# Tue, 07 Mar 2023 23:45:55 GMT
COPY ./signer-config.json . # buildkit
# Tue, 07 Mar 2023 23:45:55 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 07 Mar 2023 23:45:55 GMT
USER notary
# Tue, 07 Mar 2023 23:45:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 07 Mar 2023 23:45:55 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:159a7eace2e2271aeda929af19e5b838b268c4259c13350da47f45165b4393aa`  
		Last Modified: Tue, 21 Mar 2023 16:27:46 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d99ee501c3a276a4b465c27645d99477296bb915fa6536394d2791fa3ebfdb00`  
		Last Modified: Tue, 21 Mar 2023 16:27:50 GMT  
		Size: 125.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:638fe6e19bc680b5308d4d35e4c51ea467b0817f02ce1988c350435ec6948488`  
		Last Modified: Tue, 21 Mar 2023 16:27:50 GMT  
		Size: 4.4 MB (4390074 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a24c73e638df52d19faf7a3d8c545fd2d5e9583e8d710a47f45f1e66cf77807`  
		Last Modified: Tue, 21 Mar 2023 16:27:50 GMT  
		Size: 356.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad4a37ddf1a28eb3d6f7d6a5bbc789e9106907a95b66ebdceebeb925a34a75f8`  
		Last Modified: Tue, 21 Mar 2023 16:27:50 GMT  
		Size: 381.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `notary:signer` - unknown; unknown

```console
$ docker pull notary@sha256:f5549ba8fab66713c4d04b1216c5ca3e2e8c79c9479b3ec6e40d891bcec1e52a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.5 KB (107549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00309e6becd79d95c483ef7806096f6deede765ad8ef27106ecc152545d6a2e3`

```dockerfile
```

-	Layers:
	-	`sha256:4b946b3be7c306cc41ba6e952f7db5782d5a55f63d6fb7c9edf0d5df666ed9b9`  
		Last Modified: Tue, 21 Mar 2023 16:27:50 GMT  
		Size: 89.2 KB (89250 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7bee9970ef051e209b25dc4b73f72744e4c31e7ba081d691204386851dfaeffc`  
		Last Modified: Tue, 21 Mar 2023 16:27:50 GMT  
		Size: 18.3 KB (18299 bytes)  
		MIME: application/vnd.in-toto+json

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:79b4c323f58cb5f6ea257c2af5204098abeea66bb6d3c60b46f4693e04741701
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7381566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ddf368d5d9c9179b534f7d9a67b82e27281f60554a17dc0820eabc3abfca32c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:57:54 GMT
RUN adduser -D -H -g "" notary
# Sat, 12 Nov 2022 04:58:12 GMT
EXPOSE 4444
# Sat, 12 Nov 2022 04:58:12 GMT
EXPOSE 7899
# Sat, 12 Nov 2022 04:58:13 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:58:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:58:15 GMT
WORKDIR /notary/signer
# Wed, 16 Nov 2022 20:11:26 GMT
COPY file:044b2b6099382d2e11ff09d47c7a63f7cf3796f05317a8a2bbfed5d98c843503 in ./ 
# Wed, 16 Nov 2022 20:11:26 GMT
RUN ./notary-signer --version
# Wed, 16 Nov 2022 20:11:28 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Wed, 16 Nov 2022 20:11:29 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Wed, 16 Nov 2022 20:11:29 GMT
USER notary
# Wed, 16 Nov 2022 20:11:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 16 Nov 2022 20:11:31 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:0c10ccf9426f4a034c81b9e1a0fa81fc5cd957d8a4e0ea545ee33f4cd59f227b`  
		Last Modified: Sat, 12 Nov 2022 03:39:07 GMT  
		Size: 2.8 MB (2808348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e2a37344f15c9c47f28fb76d0bbfae6f9adb65b4d686216a9a5881505ed0ec`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26472dc994c1e659b114a40b8becb18e4595de57079b3495843fe3ee077329d`  
		Last Modified: Sat, 12 Nov 2022 04:58:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77cc9f8b030709827b83734498c26e9c13fdcad73c1751041bf38760164b7c8`  
		Last Modified: Wed, 16 Nov 2022 20:11:58 GMT  
		Size: 4.6 MB (4571177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d739be5aa3edcc7ba9f282a037921fc7c54d03aa47497444165ee21ada1487a6`  
		Last Modified: Wed, 16 Nov 2022 20:11:57 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f6cc98121c6d6e23c455cc4891ee75f1d872207a89e3ff24c67d8eedf86dac`  
		Last Modified: Wed, 16 Nov 2022 20:11:58 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:606c37e1d97f4e68ec67ee57439cbcefd35416825bbee5a8438fea16cf305ab1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7102909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d66c8f75871355a84a407a350373d37201ae2aabe85cf2690b4d651da520a1c2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:31:58 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 09:32:48 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 11 Feb 2023 09:32:48 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 11 Feb 2023 09:32:48 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 11 Feb 2023 09:32:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 11 Feb 2023 09:32:48 GMT
WORKDIR /notary/signer
# Wed, 08 Mar 2023 00:51:17 GMT
COPY /notary-signer ./ # buildkit
# Wed, 08 Mar 2023 00:51:18 GMT
RUN ./notary-signer --version # buildkit
# Wed, 08 Mar 2023 00:51:18 GMT
COPY ./signer-config.json . # buildkit
# Wed, 08 Mar 2023 00:51:18 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:51:18 GMT
USER notary
# Wed, 08 Mar 2023 00:51:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:51:18 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674d271c42b70a8c82b552b2772787a6cac62d60cdc88c599bd983e06b4b1199`  
		Last Modified: Sat, 11 Feb 2023 09:33:10 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11d0b9967527e3e2fe9a387dd1b08ba83b7816d9e3863fb0f3e9c0a13f0225d`  
		Last Modified: Sat, 11 Feb 2023 09:33:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02a9326979cee7618aa2b342258e4cbc31c56b91a4e7e8e89eff264c67e95f6`  
		Last Modified: Wed, 08 Mar 2023 00:51:47 GMT  
		Size: 4.3 MB (4296112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808f46240e2aaa0c8f9fcfd65d773fc98ad9c37bd27eb1aeb70ce112edf1ea7b`  
		Last Modified: Wed, 08 Mar 2023 00:51:46 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfc68a2dc7ed5e20299b9ec5b2c868071a1ab4f3aaee290a0da97297b5d30e3`  
		Last Modified: Wed, 08 Mar 2023 00:51:46 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9b06a55652879187796edbb714b3d74db89083480a9347c81e1573381e9eef`  
		Last Modified: Wed, 08 Mar 2023 00:51:46 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:abfdfe9dbde3305247e776f74ae5d4099b7c5219de959bc45f17b176e6e98dd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7201015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d2c656f5776c347bac9afaa7f72464bdbb3b96dab6e81f650def3f08fe52c9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:38:26 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 11 Feb 2023 03:38:57 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 11 Feb 2023 03:38:57 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 11 Feb 2023 03:38:57 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 11 Feb 2023 03:38:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 11 Feb 2023 03:38:57 GMT
WORKDIR /notary/signer
# Wed, 08 Mar 2023 00:12:03 GMT
COPY /notary-signer ./ # buildkit
# Wed, 08 Mar 2023 00:12:03 GMT
RUN ./notary-signer --version # buildkit
# Wed, 08 Mar 2023 00:12:04 GMT
COPY ./signer-config.json . # buildkit
# Wed, 08 Mar 2023 00:12:04 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 08 Mar 2023 00:12:04 GMT
USER notary
# Wed, 08 Mar 2023 00:12:04 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 08 Mar 2023 00:12:04 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf825008c0747d1db1e6a08e31a5fa2a33c8e0f8a5fe8b2f86af75110c97e790`  
		Last Modified: Sat, 11 Feb 2023 03:39:15 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47b3001bbc3d992bc8bd18f0274d2c096ab38122bfe91ebb713a068610faf80`  
		Last Modified: Sat, 11 Feb 2023 03:39:21 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabbaa0ac8ed6dfd08e91e9308501b5f3fa7aa8d1daf1f4a29f94ed70b293e76`  
		Last Modified: Wed, 08 Mar 2023 00:12:25 GMT  
		Size: 4.6 MB (4605262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e6168f2066015c6e1d056de0590b9058c7af98779aff58a8fe380fd458a4ed`  
		Last Modified: Wed, 08 Mar 2023 00:12:25 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b309adaebe295395e40d60e06633c7bf6897b14e3b191a69619b8b19cbe4c03a`  
		Last Modified: Wed, 08 Mar 2023 00:12:25 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc5983824d5ba6398ee6e275f8ebbc82284ec48ed5f55ab1ebb58db0a9e6177`  
		Last Modified: Wed, 08 Mar 2023 00:12:25 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
