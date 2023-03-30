<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `notary`

-	[`notary:server`](#notaryserver)
-	[`notary:server-0.7.0`](#notaryserver-070)
-	[`notary:signer`](#notarysigner)
-	[`notary:signer-0.7.0`](#notarysigner-070)

## `notary:server`

```console
$ docker pull notary@sha256:03a86e13badaaec26386d01a38d960b6f875c082e176b47221df4e63df789be3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:server` - linux; amd64

```console
$ docker pull notary@sha256:e00f893e919c50d78e4c720ed8a0cf070f02d6931ad9d9bf30ebe703fc4e0a35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7957091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e35c213eee97af501be09503bbd3a9cb022a389cd684070d5c7d22aacd2f10da`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:40:38 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
EXPOSE map[4443/tcp:{}]
# Wed, 29 Mar 2023 20:40:38 GMT
ENV INSTALLDIR=/notary/server
# Wed, 29 Mar 2023 20:40:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 29 Mar 2023 20:40:38 GMT
WORKDIR /notary/server
# Wed, 29 Mar 2023 20:40:38 GMT
COPY /notary-server ./ # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
RUN ./notary-server --version # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
COPY ./server-config.json . # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
USER notary
# Wed, 29 Mar 2023 20:40:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 20:40:38 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0647f7d50bd9007a9af72eec9925f5e3e4e0c35d1796c4a0970fca9f7c127a2a`  
		Last Modified: Wed, 29 Mar 2023 19:31:54 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cbb624cd06df602b5b41078cd8459f5f9cfbae1af96449820dfebaebf8e32c`  
		Last Modified: Wed, 29 Mar 2023 19:31:52 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e55a781c00a3b5a43bf525364dfa7c7aa40d36e57e62e14753530ac0a7610b`  
		Last Modified: Thu, 30 Mar 2023 03:57:32 GMT  
		Size: 5.1 MB (5147066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdbf60b6eca78e37bbf14e9346808e473f81b29ffb644b2608a8c9d99f392a8`  
		Last Modified: Thu, 30 Mar 2023 03:57:31 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb4e5fb38c054df8b76a3e82cf4aa269255ac01a6771f7c3b71b08eecaa30c3`  
		Last Modified: Thu, 30 Mar 2023 03:57:31 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8bc383fe0079b8f879147b22600adb4f228e7d63ccf71fa39cfc6d753ac991`  
		Last Modified: Thu, 30 Mar 2023 03:57:31 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:23d915b8fc86ba84a47569759c085a1fce986718b48ed6c3798edc7f92865eb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7510961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c51aedff3c3e5ac57a0ff65372e9ae7a6ea98548e62e4c9354c6ffe2bf1c8f6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Mon, 27 Mar 2023 22:54:37 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 27 Mar 2023 22:54:37 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 27 Mar 2023 22:54:37 GMT
ENV INSTALLDIR=/notary/server
# Mon, 27 Mar 2023 22:54:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 27 Mar 2023 22:54:37 GMT
WORKDIR /notary/server
# Mon, 27 Mar 2023 22:54:37 GMT
COPY /notary-server ./ # buildkit
# Mon, 27 Mar 2023 22:54:37 GMT
RUN ./notary-server --version # buildkit
# Mon, 27 Mar 2023 22:54:37 GMT
COPY ./server-config.json . # buildkit
# Mon, 27 Mar 2023 22:54:37 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 27 Mar 2023 22:54:37 GMT
USER notary
# Mon, 27 Mar 2023 22:54:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 27 Mar 2023 22:54:37 GMT
CMD ["notary-server" "--version"]
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
	-	`sha256:214377c027ebc3bfa8cf5d9c6adfe42cde43421c65fc600f490de087016f240c`  
		Last Modified: Wed, 08 Mar 2023 00:17:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3bb2a4e62a65feb82fba8588770b570f54113f46f523b08f7818828fa53331`  
		Last Modified: Tue, 28 Mar 2023 00:20:59 GMT  
		Size: 4.9 MB (4891950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cff8843aea5a062ff464e1104d4cb83972aaa0839fc7d62c2a9775ed52d1fbf`  
		Last Modified: Tue, 28 Mar 2023 00:20:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263be01dcc7d5866ad1c9c9ed1ef5740967e63099e03f6b85a3e1f72749d9e6`  
		Last Modified: Tue, 28 Mar 2023 00:20:58 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd4b4ae5f17d4495c678e86f290ed0dad3c41e9926c582bb4526c43c39e67fd`  
		Last Modified: Tue, 28 Mar 2023 00:20:58 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:dfb6e80f4cfbec424a93b0fd94c008dd0fb5cef8e8a24204491503f2f5808f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7444385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9faeb2409f2653b510503d6973459adf3e8052841162926baa5bd2868f19607`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:03:56 GMT
RUN adduser -D -H -g "" notary # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
EXPOSE map[4443/tcp:{}]
# Thu, 30 Mar 2023 04:03:56 GMT
ENV INSTALLDIR=/notary/server
# Thu, 30 Mar 2023 04:03:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 30 Mar 2023 04:03:56 GMT
WORKDIR /notary/server
# Thu, 30 Mar 2023 04:03:56 GMT
COPY /notary-server ./ # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
RUN ./notary-server --version # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
COPY ./server-config.json . # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
USER notary
# Thu, 30 Mar 2023 04:03:56 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 30 Mar 2023 04:03:56 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b02441c89b609b85e27619f8e09f858e27fdac246a198c3e19163753fcb092`  
		Last Modified: Wed, 29 Mar 2023 21:25:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be341198c2c1024a88bf425d3d85938636d2f2245ff653215d9656b0c95a9867`  
		Last Modified: Wed, 29 Mar 2023 21:25:28 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943482d51612428f68b4a3180189ab6c7611bbf42f944750a1f748e07ddff05d`  
		Last Modified: Thu, 30 Mar 2023 07:47:39 GMT  
		Size: 4.7 MB (4732811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c07e8dc6d63e3bcb31762dcd23a69ed5bdb0e214e6e3ff12f7a0c52b8741e1`  
		Last Modified: Thu, 30 Mar 2023 07:47:39 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143f6a888af51b459fda6eeeba4e638eb4823501d9aefc5dfaba59a0f75897b0`  
		Last Modified: Thu, 30 Mar 2023 07:47:38 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5bf110c31bbd45a564e0d069c3cefd3a8fb8cd2250273d15a2ae2005d4309a`  
		Last Modified: Thu, 30 Mar 2023 07:47:38 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; 386

```console
$ docker pull notary@sha256:3bbc97281bffc2fd362257fd87ba108bc61912f8b963047bd81770d9f9340a11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7761916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c272e6034e8c04514730a63792c6d7d6add1e4aa56b057cead31d50a6f106fa`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:08:35 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
EXPOSE map[4443/tcp:{}]
# Wed, 29 Mar 2023 18:08:35 GMT
ENV INSTALLDIR=/notary/server
# Wed, 29 Mar 2023 18:08:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 29 Mar 2023 18:08:35 GMT
WORKDIR /notary/server
# Wed, 29 Mar 2023 18:08:35 GMT
COPY /notary-server ./ # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
RUN ./notary-server --version # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
COPY ./server-config.json . # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
USER notary
# Wed, 29 Mar 2023 18:08:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 18:08:35 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:dea45757091f21722aec41fb20845e57a04f4bb8c199531491f1dc070480a574`  
		Last Modified: Wed, 29 Mar 2023 17:39:11 GMT  
		Size: 2.8 MB (2810814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe6407f813eee3328c3e3f4bbd5ee13b51acde95006059cfb731f7988943bc`  
		Last Modified: Wed, 29 Mar 2023 20:02:06 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d063664bd25326f6e9c648afcdb1d8586b5b6498dfe6770038000947c8f935`  
		Last Modified: Wed, 29 Mar 2023 20:02:04 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad33646a6a6184efef697df6bf3433747f0e4ce2e91064f893d6b71ec5c05f47`  
		Last Modified: Wed, 29 Mar 2023 20:02:05 GMT  
		Size: 4.9 MB (4948877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442ce6abf2fcd69d86efd2d762564c115c8ab639114b0ef47a01f50eb95bd6d0`  
		Last Modified: Wed, 29 Mar 2023 20:02:04 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132aaa5c1be8694f33c9b0f457252a91da484ebfab818f920dca166449c3806a`  
		Last Modified: Wed, 29 Mar 2023 20:02:04 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227623bd304a4e813c69bfadb810b933ff3327addba2ce02b3cb98f0b89308cc`  
		Last Modified: Wed, 29 Mar 2023 20:02:04 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; ppc64le

```console
$ docker pull notary@sha256:51a7ee9eafa2e160dac273f2db4c914624ffae66275ac9b80fc87f82d4c8a28a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7444386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c947aa8ad516e6ecb35a2fc956f2038f6fd4233cc63b029734250b0ed0e2c6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:16:34 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
EXPOSE map[4443/tcp:{}]
# Wed, 29 Mar 2023 18:16:34 GMT
ENV INSTALLDIR=/notary/server
# Wed, 29 Mar 2023 18:16:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 29 Mar 2023 18:16:34 GMT
WORKDIR /notary/server
# Wed, 29 Mar 2023 18:16:34 GMT
COPY /notary-server ./ # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
RUN ./notary-server --version # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
COPY ./server-config.json . # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
USER notary
# Wed, 29 Mar 2023 18:16:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eea900e54ccdc885e48cf524add82df276a804af096abc866a2cb00078bf29c`  
		Last Modified: Wed, 29 Mar 2023 22:35:43 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7dfa1fb665cef120a2e530d1a24146e1b9c7bbb8b713371641a879d2fa14d0c`  
		Last Modified: Wed, 29 Mar 2023 22:35:40 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc4048df030f353cab40d3b794d5dfa8a380f2648ad74402e978e8c7b5611a2`  
		Last Modified: Wed, 29 Mar 2023 22:35:41 GMT  
		Size: 4.6 MB (4637488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76b2c8e04eff6302a3088e869192190ad203a38a9602c3fd15cfbf2edcaaaa3`  
		Last Modified: Wed, 29 Mar 2023 22:35:40 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1ca5ff9725a1fe1dbffd0305119219d284c11f1c11d4e97e6671c3916341c3`  
		Last Modified: Wed, 29 Mar 2023 22:35:40 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49d6884306b875ce02f44216a742ec18ed3847ca8cea5adc7a4e530cb660727`  
		Last Modified: Wed, 29 Mar 2023 22:35:40 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:e95b37351b1805183c24312f4db36bfba0c7a18d68882eb007621185bf4e0814
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05fdb3a7a4ecb043fa8a84d1af9aa198f509f8ce273a93d9adc879f2109418ec`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 23:05:50 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
EXPOSE map[4443/tcp:{}]
# Wed, 29 Mar 2023 23:05:50 GMT
ENV INSTALLDIR=/notary/server
# Wed, 29 Mar 2023 23:05:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 29 Mar 2023 23:05:50 GMT
WORKDIR /notary/server
# Wed, 29 Mar 2023 23:05:50 GMT
COPY /notary-server ./ # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
RUN ./notary-server --version # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
COPY ./server-config.json . # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
USER notary
# Wed, 29 Mar 2023 23:05:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 23:05:50 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2496bacdc3e38b8319b094c7cd682983189e795236b61f362a29c0e8e94ceb5`  
		Last Modified: Wed, 29 Mar 2023 19:02:13 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df35cdffecfe59047614da00e02372516c2bc15ab6db89203a960b5357c45501`  
		Last Modified: Wed, 29 Mar 2023 19:02:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b31df267de3e8d8276ac5440942fb41de3c4981def07f2d4235053cd95522c5`  
		Last Modified: Thu, 30 Mar 2023 04:59:57 GMT  
		Size: 5.0 MB (4974125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4716e9e534e9b87fe2c5a112a0e4d9d4b0aa75ba4568e3965820d1e34e165bf`  
		Last Modified: Thu, 30 Mar 2023 04:59:57 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a875755506f19fc0e9309d9a462d37ce27b8cadce1d2e6d00a09db6ebd2472f0`  
		Last Modified: Thu, 30 Mar 2023 04:59:57 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811fe7925b88a2716abe111f488969b693c0bd77895133b27a6df74885b5a734`  
		Last Modified: Thu, 30 Mar 2023 04:59:57 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:server-0.7.0`

```console
$ docker pull notary@sha256:03a86e13badaaec26386d01a38d960b6f875c082e176b47221df4e63df789be3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:server-0.7.0` - linux; amd64

```console
$ docker pull notary@sha256:e00f893e919c50d78e4c720ed8a0cf070f02d6931ad9d9bf30ebe703fc4e0a35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7957091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e35c213eee97af501be09503bbd3a9cb022a389cd684070d5c7d22aacd2f10da`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:40:38 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
EXPOSE map[4443/tcp:{}]
# Wed, 29 Mar 2023 20:40:38 GMT
ENV INSTALLDIR=/notary/server
# Wed, 29 Mar 2023 20:40:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 29 Mar 2023 20:40:38 GMT
WORKDIR /notary/server
# Wed, 29 Mar 2023 20:40:38 GMT
COPY /notary-server ./ # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
RUN ./notary-server --version # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
COPY ./server-config.json . # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
USER notary
# Wed, 29 Mar 2023 20:40:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 20:40:38 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0647f7d50bd9007a9af72eec9925f5e3e4e0c35d1796c4a0970fca9f7c127a2a`  
		Last Modified: Wed, 29 Mar 2023 19:31:54 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cbb624cd06df602b5b41078cd8459f5f9cfbae1af96449820dfebaebf8e32c`  
		Last Modified: Wed, 29 Mar 2023 19:31:52 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e55a781c00a3b5a43bf525364dfa7c7aa40d36e57e62e14753530ac0a7610b`  
		Last Modified: Thu, 30 Mar 2023 03:57:32 GMT  
		Size: 5.1 MB (5147066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdbf60b6eca78e37bbf14e9346808e473f81b29ffb644b2608a8c9d99f392a8`  
		Last Modified: Thu, 30 Mar 2023 03:57:31 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb4e5fb38c054df8b76a3e82cf4aa269255ac01a6771f7c3b71b08eecaa30c3`  
		Last Modified: Thu, 30 Mar 2023 03:57:31 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8bc383fe0079b8f879147b22600adb4f228e7d63ccf71fa39cfc6d753ac991`  
		Last Modified: Thu, 30 Mar 2023 03:57:31 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:23d915b8fc86ba84a47569759c085a1fce986718b48ed6c3798edc7f92865eb8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7510961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c51aedff3c3e5ac57a0ff65372e9ae7a6ea98548e62e4c9354c6ffe2bf1c8f6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Mon, 27 Mar 2023 22:54:37 GMT
RUN adduser -D -H -g "" notary # buildkit
# Mon, 27 Mar 2023 22:54:37 GMT
EXPOSE map[4443/tcp:{}]
# Mon, 27 Mar 2023 22:54:37 GMT
ENV INSTALLDIR=/notary/server
# Mon, 27 Mar 2023 22:54:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Mon, 27 Mar 2023 22:54:37 GMT
WORKDIR /notary/server
# Mon, 27 Mar 2023 22:54:37 GMT
COPY /notary-server ./ # buildkit
# Mon, 27 Mar 2023 22:54:37 GMT
RUN ./notary-server --version # buildkit
# Mon, 27 Mar 2023 22:54:37 GMT
COPY ./server-config.json . # buildkit
# Mon, 27 Mar 2023 22:54:37 GMT
COPY ./entrypoint.sh . # buildkit
# Mon, 27 Mar 2023 22:54:37 GMT
USER notary
# Mon, 27 Mar 2023 22:54:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 27 Mar 2023 22:54:37 GMT
CMD ["notary-server" "--version"]
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
	-	`sha256:214377c027ebc3bfa8cf5d9c6adfe42cde43421c65fc600f490de087016f240c`  
		Last Modified: Wed, 08 Mar 2023 00:17:00 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3bb2a4e62a65feb82fba8588770b570f54113f46f523b08f7818828fa53331`  
		Last Modified: Tue, 28 Mar 2023 00:20:59 GMT  
		Size: 4.9 MB (4891950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cff8843aea5a062ff464e1104d4cb83972aaa0839fc7d62c2a9775ed52d1fbf`  
		Last Modified: Tue, 28 Mar 2023 00:20:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d263be01dcc7d5866ad1c9c9ed1ef5740967e63099e03f6b85a3e1f72749d9e6`  
		Last Modified: Tue, 28 Mar 2023 00:20:58 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd4b4ae5f17d4495c678e86f290ed0dad3c41e9926c582bb4526c43c39e67fd`  
		Last Modified: Tue, 28 Mar 2023 00:20:58 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:dfb6e80f4cfbec424a93b0fd94c008dd0fb5cef8e8a24204491503f2f5808f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7444385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9faeb2409f2653b510503d6973459adf3e8052841162926baa5bd2868f19607`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:03:56 GMT
RUN adduser -D -H -g "" notary # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
EXPOSE map[4443/tcp:{}]
# Thu, 30 Mar 2023 04:03:56 GMT
ENV INSTALLDIR=/notary/server
# Thu, 30 Mar 2023 04:03:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Thu, 30 Mar 2023 04:03:56 GMT
WORKDIR /notary/server
# Thu, 30 Mar 2023 04:03:56 GMT
COPY /notary-server ./ # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
RUN ./notary-server --version # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
COPY ./server-config.json . # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
USER notary
# Thu, 30 Mar 2023 04:03:56 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 30 Mar 2023 04:03:56 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b02441c89b609b85e27619f8e09f858e27fdac246a198c3e19163753fcb092`  
		Last Modified: Wed, 29 Mar 2023 21:25:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be341198c2c1024a88bf425d3d85938636d2f2245ff653215d9656b0c95a9867`  
		Last Modified: Wed, 29 Mar 2023 21:25:28 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943482d51612428f68b4a3180189ab6c7611bbf42f944750a1f748e07ddff05d`  
		Last Modified: Thu, 30 Mar 2023 07:47:39 GMT  
		Size: 4.7 MB (4732811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c07e8dc6d63e3bcb31762dcd23a69ed5bdb0e214e6e3ff12f7a0c52b8741e1`  
		Last Modified: Thu, 30 Mar 2023 07:47:39 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143f6a888af51b459fda6eeeba4e638eb4823501d9aefc5dfaba59a0f75897b0`  
		Last Modified: Thu, 30 Mar 2023 07:47:38 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5bf110c31bbd45a564e0d069c3cefd3a8fb8cd2250273d15a2ae2005d4309a`  
		Last Modified: Thu, 30 Mar 2023 07:47:38 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; 386

```console
$ docker pull notary@sha256:3bbc97281bffc2fd362257fd87ba108bc61912f8b963047bd81770d9f9340a11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7761916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c272e6034e8c04514730a63792c6d7d6add1e4aa56b057cead31d50a6f106fa`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:08:35 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
EXPOSE map[4443/tcp:{}]
# Wed, 29 Mar 2023 18:08:35 GMT
ENV INSTALLDIR=/notary/server
# Wed, 29 Mar 2023 18:08:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 29 Mar 2023 18:08:35 GMT
WORKDIR /notary/server
# Wed, 29 Mar 2023 18:08:35 GMT
COPY /notary-server ./ # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
RUN ./notary-server --version # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
COPY ./server-config.json . # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
USER notary
# Wed, 29 Mar 2023 18:08:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 18:08:35 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:dea45757091f21722aec41fb20845e57a04f4bb8c199531491f1dc070480a574`  
		Last Modified: Wed, 29 Mar 2023 17:39:11 GMT  
		Size: 2.8 MB (2810814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe6407f813eee3328c3e3f4bbd5ee13b51acde95006059cfb731f7988943bc`  
		Last Modified: Wed, 29 Mar 2023 20:02:06 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d063664bd25326f6e9c648afcdb1d8586b5b6498dfe6770038000947c8f935`  
		Last Modified: Wed, 29 Mar 2023 20:02:04 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad33646a6a6184efef697df6bf3433747f0e4ce2e91064f893d6b71ec5c05f47`  
		Last Modified: Wed, 29 Mar 2023 20:02:05 GMT  
		Size: 4.9 MB (4948877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442ce6abf2fcd69d86efd2d762564c115c8ab639114b0ef47a01f50eb95bd6d0`  
		Last Modified: Wed, 29 Mar 2023 20:02:04 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132aaa5c1be8694f33c9b0f457252a91da484ebfab818f920dca166449c3806a`  
		Last Modified: Wed, 29 Mar 2023 20:02:04 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227623bd304a4e813c69bfadb810b933ff3327addba2ce02b3cb98f0b89308cc`  
		Last Modified: Wed, 29 Mar 2023 20:02:04 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:51a7ee9eafa2e160dac273f2db4c914624ffae66275ac9b80fc87f82d4c8a28a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7444386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8c947aa8ad516e6ecb35a2fc956f2038f6fd4233cc63b029734250b0ed0e2c6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:16:34 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
EXPOSE map[4443/tcp:{}]
# Wed, 29 Mar 2023 18:16:34 GMT
ENV INSTALLDIR=/notary/server
# Wed, 29 Mar 2023 18:16:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 29 Mar 2023 18:16:34 GMT
WORKDIR /notary/server
# Wed, 29 Mar 2023 18:16:34 GMT
COPY /notary-server ./ # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
RUN ./notary-server --version # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
COPY ./server-config.json . # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
USER notary
# Wed, 29 Mar 2023 18:16:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eea900e54ccdc885e48cf524add82df276a804af096abc866a2cb00078bf29c`  
		Last Modified: Wed, 29 Mar 2023 22:35:43 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7dfa1fb665cef120a2e530d1a24146e1b9c7bbb8b713371641a879d2fa14d0c`  
		Last Modified: Wed, 29 Mar 2023 22:35:40 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc4048df030f353cab40d3b794d5dfa8a380f2648ad74402e978e8c7b5611a2`  
		Last Modified: Wed, 29 Mar 2023 22:35:41 GMT  
		Size: 4.6 MB (4637488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76b2c8e04eff6302a3088e869192190ad203a38a9602c3fd15cfbf2edcaaaa3`  
		Last Modified: Wed, 29 Mar 2023 22:35:40 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1ca5ff9725a1fe1dbffd0305119219d284c11f1c11d4e97e6671c3916341c3`  
		Last Modified: Wed, 29 Mar 2023 22:35:40 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49d6884306b875ce02f44216a742ec18ed3847ca8cea5adc7a4e530cb660727`  
		Last Modified: Wed, 29 Mar 2023 22:35:40 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:e95b37351b1805183c24312f4db36bfba0c7a18d68882eb007621185bf4e0814
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7569744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05fdb3a7a4ecb043fa8a84d1af9aa198f509f8ce273a93d9adc879f2109418ec`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 23:05:50 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
EXPOSE map[4443/tcp:{}]
# Wed, 29 Mar 2023 23:05:50 GMT
ENV INSTALLDIR=/notary/server
# Wed, 29 Mar 2023 23:05:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Wed, 29 Mar 2023 23:05:50 GMT
WORKDIR /notary/server
# Wed, 29 Mar 2023 23:05:50 GMT
COPY /notary-server ./ # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
RUN ./notary-server --version # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
COPY ./server-config.json . # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
USER notary
# Wed, 29 Mar 2023 23:05:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 23:05:50 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2496bacdc3e38b8319b094c7cd682983189e795236b61f362a29c0e8e94ceb5`  
		Last Modified: Wed, 29 Mar 2023 19:02:13 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df35cdffecfe59047614da00e02372516c2bc15ab6db89203a960b5357c45501`  
		Last Modified: Wed, 29 Mar 2023 19:02:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b31df267de3e8d8276ac5440942fb41de3c4981def07f2d4235053cd95522c5`  
		Last Modified: Thu, 30 Mar 2023 04:59:57 GMT  
		Size: 5.0 MB (4974125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4716e9e534e9b87fe2c5a112a0e4d9d4b0aa75ba4568e3965820d1e34e165bf`  
		Last Modified: Thu, 30 Mar 2023 04:59:57 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a875755506f19fc0e9309d9a462d37ce27b8cadce1d2e6d00a09db6ebd2472f0`  
		Last Modified: Thu, 30 Mar 2023 04:59:57 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811fe7925b88a2716abe111f488969b693c0bd77895133b27a6df74885b5a734`  
		Last Modified: Thu, 30 Mar 2023 04:59:57 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer`

```console
$ docker pull notary@sha256:b32ee19aa9ea15cfdaabe89a96ea9415c72d10c29b923ca2bc18598d35dedd0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:signer` - linux; amd64

```console
$ docker pull notary@sha256:0f2bf9479cb96b68dcdaec6d8d80b60d87c2634607602a67ae6280b3d14f452a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7571285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a44bd89ec153013898fbef4675fc6fecd63ebcb330805921f15a61cb9ce69ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:40:38 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 20:40:38 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 20:40:38 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 20:40:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 20:40:38 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 20:40:38 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
USER notary
# Wed, 29 Mar 2023 20:40:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 20:40:38 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0647f7d50bd9007a9af72eec9925f5e3e4e0c35d1796c4a0970fca9f7c127a2a`  
		Last Modified: Wed, 29 Mar 2023 19:31:54 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0616adcfb81a6d2087ac3d3915f5ffdfe33d1df0716cfc8fc50c4060d9cfbfa`  
		Last Modified: Wed, 29 Mar 2023 19:32:02 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8aabcde76944ad29949574fa85bd40ff75967331889c667388270bb3d9aa7db`  
		Last Modified: Thu, 30 Mar 2023 03:57:40 GMT  
		Size: 4.8 MB (4761335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cf7cd6b50ab33c61022be140d86c687c274e70a626c611ca2d491ec8adf162`  
		Last Modified: Thu, 30 Mar 2023 03:57:39 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b872af879f30f6fb0cbdbaecdff20ceb7ea87a569d66d6d72700892327f4817d`  
		Last Modified: Thu, 30 Mar 2023 03:57:39 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd1f5bcd19ae46f0fe7dbae2711efc2bc4170f6d348768af3ff9275a23aa698`  
		Last Modified: Thu, 30 Mar 2023 03:57:39 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:5f20466282b1eb92b0eb6ae0df6aab7ea93613232d282c616cf469558bb40953
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b48a8bb26415f49556a4c06f3798fa3279cd07e3390e756ed56e72d4ce6cde2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:20:00 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 19:20:00 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 19:20:00 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 19:20:00 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 19:20:00 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 19:20:00 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 19:20:00 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 19:20:00 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 19:20:00 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 19:20:00 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 19:20:00 GMT
USER notary
# Wed, 29 Mar 2023 19:20:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 19:20:00 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:c4ddbcc13e08e4ef30f810d8afad41fd6994bd8af7d37746d0ea33d8813968fc`  
		Last Modified: Wed, 29 Mar 2023 18:02:04 GMT  
		Size: 2.6 MB (2616846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68b2bcff70e852a0b418fc8919bf42378c7436f1c4e527b11979889457abb98`  
		Last Modified: Thu, 30 Mar 2023 01:14:16 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca002e85881ded17eced5eebddd6b3e45cd1bef4bf21c008a88fe58a3cc15b2`  
		Last Modified: Thu, 30 Mar 2023 01:14:14 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02bc7ddf7520d194771f171e013d7735ceae067a17a105b5099168ad560e0ef`  
		Last Modified: Thu, 30 Mar 2023 01:14:15 GMT  
		Size: 4.5 MB (4524238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6430b5cd7d65f862df1997af2bda514131f9ee796371bb8c32c0a6e6c0f65214`  
		Last Modified: Thu, 30 Mar 2023 01:14:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4615bccd0c7997c6e04cb220d6c1b7ac0ecae21c2790c9d4c30dccd16a7607af`  
		Last Modified: Thu, 30 Mar 2023 01:14:14 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c90e73a8270f6b4cf90b3539b488ba56531d7dcdc3f4a6a2aae599cbd63993`  
		Last Modified: Thu, 30 Mar 2023 01:14:14 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:9c970915d52478a188dfc247a8f12792e6085b92a5e30dfcbae1802c118e6a49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7101589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80691f4f9ede851fb8c362eeb20c7876b995405efd768cdbd18c046a9a339dff`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:03:56 GMT
RUN adduser -D -H -g "" notary # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
EXPOSE map[4444/tcp:{}]
# Thu, 30 Mar 2023 04:03:56 GMT
EXPOSE map[7899/tcp:{}]
# Thu, 30 Mar 2023 04:03:56 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 30 Mar 2023 04:03:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 30 Mar 2023 04:03:56 GMT
WORKDIR /notary/signer
# Thu, 30 Mar 2023 04:03:56 GMT
COPY /notary-signer ./ # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
RUN ./notary-signer --version # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
COPY ./signer-config.json . # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
USER notary
# Thu, 30 Mar 2023 04:03:56 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 30 Mar 2023 04:03:56 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b02441c89b609b85e27619f8e09f858e27fdac246a198c3e19163753fcb092`  
		Last Modified: Wed, 29 Mar 2023 21:25:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dd30044d17dd0900f33ee4cd64e106aa2d710607e560c51ad8bc6fd3172e8e`  
		Last Modified: Wed, 29 Mar 2023 21:25:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ef1b8fe35ed915c089fc44fbf2c8571200bc911793a779ac05f81d8ac06e77`  
		Last Modified: Thu, 30 Mar 2023 07:47:47 GMT  
		Size: 4.4 MB (4390084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562d6ddf1199ce724325b4ca8443047244166b5c25ce61a3cd6cdd1796a20e7`  
		Last Modified: Thu, 30 Mar 2023 07:47:46 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9c3fbb1d63c193db2abe041dfa66b797274e44935438008359e216222e5e22`  
		Last Modified: Thu, 30 Mar 2023 07:47:46 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ecc8ddf6e36fe1f9188496e2a317b40ef4bba1e52f235295693808ae4d1b6d`  
		Last Modified: Thu, 30 Mar 2023 07:47:46 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:4abeddf0514a353212971d22dac3dcd0f362eb5673c5dee566a64a66dd0112f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7388858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86e928c18ae2b7afcf2dea0e43582ea72f94f386a85415c22902a8b67b189c34`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:08:35 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 18:08:35 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 18:08:35 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 18:08:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 18:08:35 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 18:08:35 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
USER notary
# Wed, 29 Mar 2023 18:08:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 18:08:35 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:dea45757091f21722aec41fb20845e57a04f4bb8c199531491f1dc070480a574`  
		Last Modified: Wed, 29 Mar 2023 17:39:11 GMT  
		Size: 2.8 MB (2810814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe6407f813eee3328c3e3f4bbd5ee13b51acde95006059cfb731f7988943bc`  
		Last Modified: Wed, 29 Mar 2023 20:02:06 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb27e6c7f9cb4bd86bcf086d62affd7ae9ff7ddd66d35b1e968864cbd01871e`  
		Last Modified: Wed, 29 Mar 2023 20:02:14 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22b0bd116bf381f3b9b420f35e74669226ff0912664b3b7952bba9201986614`  
		Last Modified: Wed, 29 Mar 2023 20:02:15 GMT  
		Size: 4.6 MB (4575891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea7b49dc7a7633c397ab80131dd1867ed00c1370efa343eda4422598ee41df9`  
		Last Modified: Wed, 29 Mar 2023 20:02:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35c4944b89fc1336c998b8f12403111ec969b6da3225128d43e94385d8af41b`  
		Last Modified: Wed, 29 Mar 2023 20:02:14 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba9413a1ce459d7b222d8aa6ca7717f479471558ba35680a895fa2e0f51c372`  
		Last Modified: Wed, 29 Mar 2023 20:02:14 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:f8ea061a49b8604d5b6c364df95cf8e4fd8a0078502dacbdbd24a1e63b0f69fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7102937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75674e93d41facd2a781b6cab18d39bc1ca79545595c67472e958d1b0d7e2c10`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:16:34 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 18:16:34 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 18:16:34 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 18:16:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 18:16:34 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 18:16:34 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
USER notary
# Wed, 29 Mar 2023 18:16:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eea900e54ccdc885e48cf524add82df276a804af096abc866a2cb00078bf29c`  
		Last Modified: Wed, 29 Mar 2023 22:35:43 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66e653fcd0757f3ba42b926dcd02930e19de92db844de27b1fd55e1cba8b81c`  
		Last Modified: Wed, 29 Mar 2023 22:35:51 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94acfc7ce28ccc4dd68c28b39af94300962f5982ad1fb370f461cc1c2ce635ea`  
		Last Modified: Wed, 29 Mar 2023 22:35:52 GMT  
		Size: 4.3 MB (4296107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52bf7f8a58c4ca88435c06fc676952d37760b7cbc995df55f3c1ccaa3025778`  
		Last Modified: Wed, 29 Mar 2023 22:35:51 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d47683e16da216655074126adba4d7c5b0eb58015a0292d10c3cdf46fdc1544`  
		Last Modified: Wed, 29 Mar 2023 22:35:51 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59322b661afb3f89a98e046f5fc6b0f7898bdfc2353cb5f6d4c5a7471036f390`  
		Last Modified: Wed, 29 Mar 2023 22:35:51 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:28d65546cc44a6dfc83a0e965fad7242b77ff31606c34122fd9265743ed751de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7200811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8fc7db32d4edb6c9a40d4fa559490156325344b89d7b825906fd577e16c990`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 23:05:50 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 23:05:50 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 23:05:50 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 23:05:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 23:05:50 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 23:05:50 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
USER notary
# Wed, 29 Mar 2023 23:05:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 23:05:50 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2496bacdc3e38b8319b094c7cd682983189e795236b61f362a29c0e8e94ceb5`  
		Last Modified: Wed, 29 Mar 2023 19:02:13 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896ac2c8f346280fd047876860be1d522eae075adf2d30efb94fdc4359a6a466`  
		Last Modified: Wed, 29 Mar 2023 19:02:18 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b66ebc5bf43547a0b3d18343a506b2fe82ff53f2f13f07ad02fb4a5ebe03bb`  
		Last Modified: Thu, 30 Mar 2023 05:00:04 GMT  
		Size: 4.6 MB (4605266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daf0f3398223518d55aae06f1ddd2509deab4fd21967079f6b5045ec8fbcc62`  
		Last Modified: Thu, 30 Mar 2023 05:00:03 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1986357c23063241c28fc4601b777e64b9afee96a2b157d910977c62964636`  
		Last Modified: Thu, 30 Mar 2023 05:00:03 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e01526cc6d8dc2c2d59834a29982b132720ac4f5ada52ea826bd120ef95dcb0`  
		Last Modified: Thu, 30 Mar 2023 05:00:03 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer-0.7.0`

```console
$ docker pull notary@sha256:b32ee19aa9ea15cfdaabe89a96ea9415c72d10c29b923ca2bc18598d35dedd0e
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
$ docker pull notary@sha256:0f2bf9479cb96b68dcdaec6d8d80b60d87c2634607602a67ae6280b3d14f452a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7571285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a44bd89ec153013898fbef4675fc6fecd63ebcb330805921f15a61cb9ce69ab`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:40:38 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 20:40:38 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 20:40:38 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 20:40:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 20:40:38 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 20:40:38 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 20:40:38 GMT
USER notary
# Wed, 29 Mar 2023 20:40:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 20:40:38 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0647f7d50bd9007a9af72eec9925f5e3e4e0c35d1796c4a0970fca9f7c127a2a`  
		Last Modified: Wed, 29 Mar 2023 19:31:54 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0616adcfb81a6d2087ac3d3915f5ffdfe33d1df0716cfc8fc50c4060d9cfbfa`  
		Last Modified: Wed, 29 Mar 2023 19:32:02 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8aabcde76944ad29949574fa85bd40ff75967331889c667388270bb3d9aa7db`  
		Last Modified: Thu, 30 Mar 2023 03:57:40 GMT  
		Size: 4.8 MB (4761335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cf7cd6b50ab33c61022be140d86c687c274e70a626c611ca2d491ec8adf162`  
		Last Modified: Thu, 30 Mar 2023 03:57:39 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b872af879f30f6fb0cbdbaecdff20ceb7ea87a569d66d6d72700892327f4817d`  
		Last Modified: Thu, 30 Mar 2023 03:57:39 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd1f5bcd19ae46f0fe7dbae2711efc2bc4170f6d348768af3ff9275a23aa698`  
		Last Modified: Thu, 30 Mar 2023 03:57:39 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:5f20466282b1eb92b0eb6ae0df6aab7ea93613232d282c616cf469558bb40953
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7143249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b48a8bb26415f49556a4c06f3798fa3279cd07e3390e756ed56e72d4ce6cde2`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:20:00 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 19:20:00 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 19:20:00 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 19:20:00 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 19:20:00 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 19:20:00 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 19:20:00 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 19:20:00 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 19:20:00 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 19:20:00 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 19:20:00 GMT
USER notary
# Wed, 29 Mar 2023 19:20:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 19:20:00 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:c4ddbcc13e08e4ef30f810d8afad41fd6994bd8af7d37746d0ea33d8813968fc`  
		Last Modified: Wed, 29 Mar 2023 18:02:04 GMT  
		Size: 2.6 MB (2616846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68b2bcff70e852a0b418fc8919bf42378c7436f1c4e527b11979889457abb98`  
		Last Modified: Thu, 30 Mar 2023 01:14:16 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca002e85881ded17eced5eebddd6b3e45cd1bef4bf21c008a88fe58a3cc15b2`  
		Last Modified: Thu, 30 Mar 2023 01:14:14 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02bc7ddf7520d194771f171e013d7735ceae067a17a105b5099168ad560e0ef`  
		Last Modified: Thu, 30 Mar 2023 01:14:15 GMT  
		Size: 4.5 MB (4524238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6430b5cd7d65f862df1997af2bda514131f9ee796371bb8c32c0a6e6c0f65214`  
		Last Modified: Thu, 30 Mar 2023 01:14:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4615bccd0c7997c6e04cb220d6c1b7ac0ecae21c2790c9d4c30dccd16a7607af`  
		Last Modified: Thu, 30 Mar 2023 01:14:14 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c90e73a8270f6b4cf90b3539b488ba56531d7dcdc3f4a6a2aae599cbd63993`  
		Last Modified: Thu, 30 Mar 2023 01:14:14 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:9c970915d52478a188dfc247a8f12792e6085b92a5e30dfcbae1802c118e6a49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7101589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80691f4f9ede851fb8c362eeb20c7876b995405efd768cdbd18c046a9a339dff`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:03:56 GMT
RUN adduser -D -H -g "" notary # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
EXPOSE map[4444/tcp:{}]
# Thu, 30 Mar 2023 04:03:56 GMT
EXPOSE map[7899/tcp:{}]
# Thu, 30 Mar 2023 04:03:56 GMT
ENV INSTALLDIR=/notary/signer
# Thu, 30 Mar 2023 04:03:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Thu, 30 Mar 2023 04:03:56 GMT
WORKDIR /notary/signer
# Thu, 30 Mar 2023 04:03:56 GMT
COPY /notary-signer ./ # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
RUN ./notary-signer --version # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
COPY ./signer-config.json . # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
COPY ./entrypoint.sh . # buildkit
# Thu, 30 Mar 2023 04:03:56 GMT
USER notary
# Thu, 30 Mar 2023 04:03:56 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 30 Mar 2023 04:03:56 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b02441c89b609b85e27619f8e09f858e27fdac246a198c3e19163753fcb092`  
		Last Modified: Wed, 29 Mar 2023 21:25:30 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dd30044d17dd0900f33ee4cd64e106aa2d710607e560c51ad8bc6fd3172e8e`  
		Last Modified: Wed, 29 Mar 2023 21:25:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ef1b8fe35ed915c089fc44fbf2c8571200bc911793a779ac05f81d8ac06e77`  
		Last Modified: Thu, 30 Mar 2023 07:47:47 GMT  
		Size: 4.4 MB (4390084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4562d6ddf1199ce724325b4ca8443047244166b5c25ce61a3cd6cdd1796a20e7`  
		Last Modified: Thu, 30 Mar 2023 07:47:46 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9c3fbb1d63c193db2abe041dfa66b797274e44935438008359e216222e5e22`  
		Last Modified: Thu, 30 Mar 2023 07:47:46 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ecc8ddf6e36fe1f9188496e2a317b40ef4bba1e52f235295693808ae4d1b6d`  
		Last Modified: Thu, 30 Mar 2023 07:47:46 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; 386

```console
$ docker pull notary@sha256:4abeddf0514a353212971d22dac3dcd0f362eb5673c5dee566a64a66dd0112f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7388858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86e928c18ae2b7afcf2dea0e43582ea72f94f386a85415c22902a8b67b189c34`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:08:35 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 18:08:35 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 18:08:35 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 18:08:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 18:08:35 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 18:08:35 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 18:08:35 GMT
USER notary
# Wed, 29 Mar 2023 18:08:35 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 18:08:35 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:dea45757091f21722aec41fb20845e57a04f4bb8c199531491f1dc070480a574`  
		Last Modified: Wed, 29 Mar 2023 17:39:11 GMT  
		Size: 2.8 MB (2810814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe6407f813eee3328c3e3f4bbd5ee13b51acde95006059cfb731f7988943bc`  
		Last Modified: Wed, 29 Mar 2023 20:02:06 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb27e6c7f9cb4bd86bcf086d62affd7ae9ff7ddd66d35b1e968864cbd01871e`  
		Last Modified: Wed, 29 Mar 2023 20:02:14 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22b0bd116bf381f3b9b420f35e74669226ff0912664b3b7952bba9201986614`  
		Last Modified: Wed, 29 Mar 2023 20:02:15 GMT  
		Size: 4.6 MB (4575891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea7b49dc7a7633c397ab80131dd1867ed00c1370efa343eda4422598ee41df9`  
		Last Modified: Wed, 29 Mar 2023 20:02:14 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35c4944b89fc1336c998b8f12403111ec969b6da3225128d43e94385d8af41b`  
		Last Modified: Wed, 29 Mar 2023 20:02:14 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba9413a1ce459d7b222d8aa6ca7717f479471558ba35680a895fa2e0f51c372`  
		Last Modified: Wed, 29 Mar 2023 20:02:14 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:f8ea061a49b8604d5b6c364df95cf8e4fd8a0078502dacbdbd24a1e63b0f69fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7102937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75674e93d41facd2a781b6cab18d39bc1ca79545595c67472e958d1b0d7e2c10`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:16:34 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 18:16:34 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 18:16:34 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 18:16:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 18:16:34 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 18:16:34 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 18:16:34 GMT
USER notary
# Wed, 29 Mar 2023 18:16:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eea900e54ccdc885e48cf524add82df276a804af096abc866a2cb00078bf29c`  
		Last Modified: Wed, 29 Mar 2023 22:35:43 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66e653fcd0757f3ba42b926dcd02930e19de92db844de27b1fd55e1cba8b81c`  
		Last Modified: Wed, 29 Mar 2023 22:35:51 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94acfc7ce28ccc4dd68c28b39af94300962f5982ad1fb370f461cc1c2ce635ea`  
		Last Modified: Wed, 29 Mar 2023 22:35:52 GMT  
		Size: 4.3 MB (4296107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52bf7f8a58c4ca88435c06fc676952d37760b7cbc995df55f3c1ccaa3025778`  
		Last Modified: Wed, 29 Mar 2023 22:35:51 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d47683e16da216655074126adba4d7c5b0eb58015a0292d10c3cdf46fdc1544`  
		Last Modified: Wed, 29 Mar 2023 22:35:51 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59322b661afb3f89a98e046f5fc6b0f7898bdfc2353cb5f6d4c5a7471036f390`  
		Last Modified: Wed, 29 Mar 2023 22:35:51 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:28d65546cc44a6dfc83a0e965fad7242b77ff31606c34122fd9265743ed751de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7200811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8fc7db32d4edb6c9a40d4fa559490156325344b89d7b825906fd577e16c990`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 23:05:50 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 23:05:50 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 23:05:50 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 23:05:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 23:05:50 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 23:05:50 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 23:05:50 GMT
USER notary
# Wed, 29 Mar 2023 23:05:50 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 23:05:50 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2496bacdc3e38b8319b094c7cd682983189e795236b61f362a29c0e8e94ceb5`  
		Last Modified: Wed, 29 Mar 2023 19:02:13 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896ac2c8f346280fd047876860be1d522eae075adf2d30efb94fdc4359a6a466`  
		Last Modified: Wed, 29 Mar 2023 19:02:18 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b66ebc5bf43547a0b3d18343a506b2fe82ff53f2f13f07ad02fb4a5ebe03bb`  
		Last Modified: Thu, 30 Mar 2023 05:00:04 GMT  
		Size: 4.6 MB (4605266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daf0f3398223518d55aae06f1ddd2509deab4fd21967079f6b5045ec8fbcc62`  
		Last Modified: Thu, 30 Mar 2023 05:00:03 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1986357c23063241c28fc4601b777e64b9afee96a2b157d910977c62964636`  
		Last Modified: Thu, 30 Mar 2023 05:00:03 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e01526cc6d8dc2c2d59834a29982b132720ac4f5ada52ea826bd120ef95dcb0`  
		Last Modified: Thu, 30 Mar 2023 05:00:03 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
