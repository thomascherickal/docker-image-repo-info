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
