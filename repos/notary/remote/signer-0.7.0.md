## `notary:signer-0.7.0`

```console
$ docker pull notary@sha256:6d9dc5d2057782ee6e3c523b7ffbd76f4f21b9a6499621a75475284b8a3ebccc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:signer-0.7.0` - linux; amd64

```console
$ docker pull notary@sha256:95efcd364bfacd0155dd4ad13110df92a2930ccf449ca9740c3bb5609135105e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ebe11f5c1d03d3de87dc3867c9bc23ac6ab56d92d6effa718c92ea518d8a5e8`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
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
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006de58a565eab12a85c007364709b9c3158a5cbe003d17c9c062ee51475613b`  
		Last Modified: Thu, 15 Jun 2023 05:47:42 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655a3983fcf06ac840361d61904864717dc82d5e2ddac9b3b0412b538509c5d9`  
		Last Modified: Thu, 15 Jun 2023 05:47:49 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fafa54d4ebebd6ad8a270c675ecfb39f5da9c9dfc10845b3760b2f6219ef96`  
		Last Modified: Thu, 15 Jun 2023 05:47:50 GMT  
		Size: 4.8 MB (4763101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f43b8480043f86cb5c511aae354b5d2de8634918ea4e9a188327b24d0dd9d6d`  
		Last Modified: Thu, 15 Jun 2023 05:47:49 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa93aff66bddcba481db60e97574fcede526cda8384914fbce55b65aca87b49`  
		Last Modified: Thu, 15 Jun 2023 05:47:49 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d485da9b0027fb193ffca24699f6e5223732640ea2ee48e14d411bc2e708aff1`  
		Last Modified: Thu, 15 Jun 2023 05:47:49 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:90b69ffc1941f2784fb289d01f1d0bae56519af7b96e1c45f9da363dc03412cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d29a2cf1aa464aac3c6883b5b9be6640617ade3eb758092fced0f819f0ae793d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:28 GMT
ADD file:41a85835978e4acba9d92833f0d5e20084da50779e52d8832d576b003a7aa1bb in / 
# Wed, 14 Jun 2023 18:49:29 GMT
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
	-	`sha256:3a8b1ea8ec24955304373c42ddad13462ec8177200b715cdae1220f4372b27ae`  
		Last Modified: Thu, 15 Jun 2023 00:03:34 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b33cd03e7c050247a53bb85a5e824fbd3a6f60a9e46f48ec351284ca00c03ba`  
		Last Modified: Thu, 15 Jun 2023 00:03:41 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6de8c0f2553b1605a20b1437a913dc49acc099537d27716ed4d43c4a6d5e27`  
		Last Modified: Thu, 15 Jun 2023 00:03:42 GMT  
		Size: 4.5 MB (4526084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d6061b8841cef9458c9a7cd08da53f77f8d324ce0c4211e9f2678f336e24b8`  
		Last Modified: Thu, 15 Jun 2023 00:03:41 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e79186352f46e97beade2cbd4c13c87ca1f3728166b546c1e329156ca7c63e1`  
		Last Modified: Thu, 15 Jun 2023 00:03:41 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2552d856cbe04e784c17c1cd727703ee4026471bc096db7673bc27dc6b98861`  
		Last Modified: Thu, 15 Jun 2023 00:03:41 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:cdfbafdf7af365183ad5d8557e31ef41ae4664c836cb4ed4265f571d33a0cdbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7103121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5ca3462d1385a6811a6e282e95b9f8501e95be3f3549839f3dbcf6db17276a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
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
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a70fe37c8d33b219ba725d1903a536b2d54bd47305e1c9d9a969b379ece36`  
		Last Modified: Thu, 15 Jun 2023 03:04:58 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b3a6a315e1165176c346930f35d9db3af0888e15d5c29cf684c613b9564c17`  
		Last Modified: Thu, 15 Jun 2023 03:05:07 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3e485eff1aa2e6b6f21c727023342ca7a2ba1aae943a356fe253667b888366`  
		Last Modified: Thu, 15 Jun 2023 03:05:08 GMT  
		Size: 4.4 MB (4393070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e14761d071f0bcf50e535d0846b939840705ad58664107d393c36f42432dec6`  
		Last Modified: Thu, 15 Jun 2023 03:05:07 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf9c028f26fb72268189bede7ad70af1372b0c98a97010ef5b09c06686ca538`  
		Last Modified: Thu, 15 Jun 2023 03:05:07 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d895fe244d16b20c48cac708c0415dfe473862a280cfb1b110bbf36ba848804`  
		Last Modified: Thu, 15 Jun 2023 03:05:07 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; 386

```console
$ docker pull notary@sha256:3908bd7d74032da2e951fae39374837d4c9001a9eeb36f65a4f38de321f67650
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7391736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:969ec6f8dce8da8f77866cdc09f961851ec88146f2df785c649a47c6aacc2b5b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:30 GMT
ADD file:9b22a3b9a2009266eccfbbf15fbc348f6c854a6c496df29e5c4f0a832b796c67 in / 
# Wed, 14 Jun 2023 22:33:30 GMT
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
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a41c79ffa0a1ed1ad6af485640f3cedcf7b3926deb902b5424bee397e0fac9`  
		Last Modified: Thu, 15 Jun 2023 03:36:32 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019d3941ffbaab7a8ec9ea3a777e2cebb13552668a940019ab1292ae76bbc56d`  
		Last Modified: Thu, 15 Jun 2023 03:36:40 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23af9417015f9c3fcc45be64e96faadd47ad4062e5c87a3dcd88fb33ff85b11`  
		Last Modified: Thu, 15 Jun 2023 03:36:41 GMT  
		Size: 4.6 MB (4579009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ceec2cbcaee458f643a2d52becdfcf8b3501034a0f89f7bf3686e3ae3ab25d4`  
		Last Modified: Thu, 15 Jun 2023 03:36:40 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1338ad8d68929871f4271e3a40e7ae0caf52cdabefe1320eb3485238f92507e`  
		Last Modified: Thu, 15 Jun 2023 03:36:40 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a15cd05a039e0501ac982e3495d7fa7c0e59d373779483e7aabc979fd5eb071`  
		Last Modified: Thu, 15 Jun 2023 03:36:40 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:da947a1870c513cce66f04289b514c550059f298fb12f9daaa0bc754bc339b14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7101407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c6b9858ad1c7c60f820fcc6a03c859434ae14e41d27b1c995748a5d4d438b80`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Thu, 15 Jun 2023 00:40:03 GMT
ADD file:687ce61613e63c93be9debda827167f433a51769ad625312ea1250ee87b62f30 in / 
# Thu, 15 Jun 2023 00:40:03 GMT
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
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae01cf59efaf0a10f9728f0d6f10af743f74c6440f154139a12f2d2449f7fce`  
		Last Modified: Thu, 15 Jun 2023 05:17:42 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3b8a820a53d1d79b059a6700a15b805a541e4558e0d023f4d1ad10de1b5c2f`  
		Last Modified: Thu, 15 Jun 2023 05:17:50 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8560dfe3eafd85154860dd418646bf0e62560a30641f78e8a23b7058f30dae`  
		Last Modified: Thu, 15 Jun 2023 05:17:52 GMT  
		Size: 4.3 MB (4296984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85e942faea91f0a0cffc55c8455b4a00903a3b4ec430f2b9792b27f4317bbde`  
		Last Modified: Thu, 15 Jun 2023 05:17:51 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0cc833f52914db1085fdfb5f95fd3b781c087deec6f016bd20137e16bd4990`  
		Last Modified: Thu, 15 Jun 2023 05:17:50 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04a6a6f63fee0a49213b9d8d6883fcb277108202c9b491163c6ba5d93fcb802`  
		Last Modified: Thu, 15 Jun 2023 05:17:50 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:df0c012735312c7c6bdab1807de23d900b5d317dac1bfb3ba2a517b3d528faed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7202239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e947d59f41f660c63827a3cde0e826473645f6fedbee7fdbc11cca247542e6d9`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:45:37 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:45:37 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 02 May 2023 18:45:37 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 02 May 2023 18:45:37 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 02 May 2023 18:45:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 02 May 2023 18:45:37 GMT
WORKDIR /notary/signer
# Tue, 02 May 2023 18:45:37 GMT
COPY /notary-signer ./ # buildkit
# Tue, 02 May 2023 18:45:37 GMT
RUN ./notary-signer --version # buildkit
# Tue, 02 May 2023 18:45:37 GMT
COPY ./signer-config.json . # buildkit
# Tue, 02 May 2023 18:45:37 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:45:37 GMT
USER notary
# Tue, 02 May 2023 18:45:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:45:37 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d718f433f226a10233b1c2fd202d613455bab7210ecab0e649f578786e27cc7`  
		Last Modified: Tue, 02 May 2023 19:14:49 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b0e7bac61f3956b146049f39a99820a3bb37186cd5687fe8d4c4d16260b05f`  
		Last Modified: Tue, 02 May 2023 19:14:53 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4d94993f25b2dc1fc676cb84a5de77085d32f5fed07181cc681b81ebb04397`  
		Last Modified: Tue, 02 May 2023 19:14:54 GMT  
		Size: 4.6 MB (4606697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2026d1beb12855074e085e40a1904ab8b616443b9a66680c53361ed62d95ff0c`  
		Last Modified: Tue, 02 May 2023 19:14:53 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a541084e182dcba399dcf9cca0ddb67fb7f71ba8b300d52c5f7f7968a907057b`  
		Last Modified: Tue, 02 May 2023 19:14:53 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff7369e69e70dd9b3c20eb7c5985f6007d57a56599ec0468fb0c32c83d8ab6c`  
		Last Modified: Tue, 02 May 2023 19:14:53 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
