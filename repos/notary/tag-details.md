<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `notary`

-	[`notary:server`](#notaryserver)
-	[`notary:server-0.7.0`](#notaryserver-070)
-	[`notary:signer`](#notarysigner)
-	[`notary:signer-0.7.0`](#notarysigner-070)

## `notary:server`

```console
$ docker pull notary@sha256:581c6109ca091149245c98490372227e4f5a523b12440c1791252a44f8b1e7b3
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
$ docker pull notary@sha256:38033e73a87483aa995831a0ace0aa5fbc5faea7debaaf5a8049b4dcf1a32778
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7957732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e59645ea6776ba06b6a3a1d85ba272d3b8a6eeab645e01d62d6af7747cbd755b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:32:09 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 04 Apr 2023 18:32:09 GMT
ENV INSTALLDIR=/notary/server
# Tue, 04 Apr 2023 18:32:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 04 Apr 2023 18:32:09 GMT
WORKDIR /notary/server
# Tue, 04 Apr 2023 18:32:09 GMT
COPY /notary-server ./ # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
RUN ./notary-server --version # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
COPY ./server-config.json . # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
USER notary
# Tue, 04 Apr 2023 18:32:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:32:09 GMT
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
	-	`sha256:ae6033ff6c5306c860d176e4f63ee95200657bdf39dcac9aa5996a52c9cd2bce`  
		Last Modified: Tue, 04 Apr 2023 18:52:30 GMT  
		Size: 5.1 MB (5147706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cb2ce27c29e726a10db7f3602fff9eac81142d5cb5860961f0cfc25e4b17ed`  
		Last Modified: Tue, 04 Apr 2023 18:52:27 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b58d530011c6e6507355770a9fa7dccec9b417e55adff23aa8318bbe2419c8`  
		Last Modified: Tue, 04 Apr 2023 18:52:27 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a9201e2f6bd50eb77bd885b968b7f2cea0067972b0f8a22c0acd7cd7038140`  
		Last Modified: Tue, 04 Apr 2023 18:52:27 GMT  
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
$ docker pull notary@sha256:e694df0d62760b881cfcfdf4a98068265fd3642afc15d5c4897ae25ac46d5139
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7445278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:221135de97cdf2fdc284d293c93798e3c839dfa109544965655cfccdd42c8ff7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:31:29 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 04 Apr 2023 18:31:29 GMT
ENV INSTALLDIR=/notary/server
# Tue, 04 Apr 2023 18:31:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 04 Apr 2023 18:31:29 GMT
WORKDIR /notary/server
# Tue, 04 Apr 2023 18:31:29 GMT
COPY /notary-server ./ # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
RUN ./notary-server --version # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
COPY ./server-config.json . # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
USER notary
# Tue, 04 Apr 2023 18:31:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:31:29 GMT
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
	-	`sha256:4d5ccf3043141a3e6c39b3471be9e091c376d20c9b936984977a454a12cc8041`  
		Last Modified: Tue, 04 Apr 2023 18:51:03 GMT  
		Size: 4.7 MB (4733700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c7c215b81721208ca96fdbe5b1e708e0ffa5771a485ea301f55e9c43ee9d85`  
		Last Modified: Tue, 04 Apr 2023 18:51:02 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73678ec06be8c4ac10f7a68fb7ccc299c396b8800ad93e8628ad0b12239cd2e2`  
		Last Modified: Tue, 04 Apr 2023 18:51:02 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d5c7b604457ddb60c19aa06f5be53a3d1655f69d13329dedc9529049a579fe`  
		Last Modified: Tue, 04 Apr 2023 18:51:02 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; 386

```console
$ docker pull notary@sha256:1d95a7d4aefd2fdb61afd5ba0754e36945df32d1168565fd3dcdd22ebe910b91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7762889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39ce85b2a309ee388a19183ba7877bd5c16c2a78f08772b1499e4900b15ad3ad`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:38:09 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 04 Apr 2023 18:38:09 GMT
ENV INSTALLDIR=/notary/server
# Tue, 04 Apr 2023 18:38:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 04 Apr 2023 18:38:09 GMT
WORKDIR /notary/server
# Tue, 04 Apr 2023 18:38:09 GMT
COPY /notary-server ./ # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
RUN ./notary-server --version # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
COPY ./server-config.json . # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
USER notary
# Tue, 04 Apr 2023 18:38:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:38:09 GMT
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
	-	`sha256:a84b63ff713e3e110d439b56101a4e629b5a3cb4d013fa7b4c038ad4b4f6dd6b`  
		Last Modified: Tue, 04 Apr 2023 18:58:58 GMT  
		Size: 4.9 MB (4949845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479755b6f7b68df076a0131604e6628f5d46cd881499f8d888ac361a5ae44f4d`  
		Last Modified: Tue, 04 Apr 2023 18:58:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5eaff1e003f8017370ff5f8720c9e9b8ae830ceac6176a016e1f379d965e8d`  
		Last Modified: Tue, 04 Apr 2023 18:58:57 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fdc9eb5debe908895457bef757f802c43e900eb1b833dd89503a8cb3b5173e`  
		Last Modified: Tue, 04 Apr 2023 18:58:57 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; ppc64le

```console
$ docker pull notary@sha256:7c076eec186e8038fe69d54a66989e3a91c56f3a4b38f8770c67faab608cbd9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7445323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:493fb1d65fca182158bf5095a234c55aa5be5de759cadfde45559337025b3b82`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:38:42 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 04 Apr 2023 18:38:42 GMT
ENV INSTALLDIR=/notary/server
# Tue, 04 Apr 2023 18:38:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 04 Apr 2023 18:38:42 GMT
WORKDIR /notary/server
# Tue, 04 Apr 2023 18:38:42 GMT
COPY /notary-server ./ # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
RUN ./notary-server --version # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
COPY ./server-config.json . # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
USER notary
# Tue, 04 Apr 2023 18:38:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:38:42 GMT
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
	-	`sha256:ad4a590a465c27aa5a29bd297d1e68effa8acc419174358cdd0a8a6a84820dfa`  
		Last Modified: Tue, 04 Apr 2023 18:59:52 GMT  
		Size: 4.6 MB (4638418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5b8c26bdc75f5cd1e421d00063098d1fe5659e74739dfaa895453deb4cfe87`  
		Last Modified: Tue, 04 Apr 2023 18:59:51 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab45b68267c877393096be43ae3bb328e2070659d00516492d9c7159c75b952`  
		Last Modified: Tue, 04 Apr 2023 18:59:51 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f997fefe5793a23fad058d49b3da7ec402d10ed3bf37ee62d2a37f7e77ab1f0`  
		Last Modified: Tue, 04 Apr 2023 18:59:51 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:1ff9463ad5fca4543b72138ab861eb2674ecf8cad3e5fda7680134102c8a7b3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7571574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8728d93ff4f8d6b5e2bfb139a2c18ad0866f6d1693deba4967e7959a0ddf402`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:33:21 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 04 Apr 2023 18:33:21 GMT
ENV INSTALLDIR=/notary/server
# Tue, 04 Apr 2023 18:33:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 04 Apr 2023 18:33:21 GMT
WORKDIR /notary/server
# Tue, 04 Apr 2023 18:33:21 GMT
COPY /notary-server ./ # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
RUN ./notary-server --version # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
COPY ./server-config.json . # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
USER notary
# Tue, 04 Apr 2023 18:33:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:33:21 GMT
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
	-	`sha256:bef149a60bf86421301321480e056107d4635bca444c4588f5f9a59de57ae26d`  
		Last Modified: Tue, 04 Apr 2023 18:52:53 GMT  
		Size: 5.0 MB (4975954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a351f9f76c66a4782e7980ec804334bfda5ef29f54e6d8a19e8820afb8e7dc8f`  
		Last Modified: Tue, 04 Apr 2023 18:52:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2889b67f069c689b59a55d397bd670e6be326a822558227f79cd022a27a7f430`  
		Last Modified: Tue, 04 Apr 2023 18:52:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3a26d38711527b618620bd74986103d2c7087732b789714f8f4a062f567e99`  
		Last Modified: Tue, 04 Apr 2023 18:52:52 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:server-0.7.0`

```console
$ docker pull notary@sha256:581c6109ca091149245c98490372227e4f5a523b12440c1791252a44f8b1e7b3
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
$ docker pull notary@sha256:38033e73a87483aa995831a0ace0aa5fbc5faea7debaaf5a8049b4dcf1a32778
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7957732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e59645ea6776ba06b6a3a1d85ba272d3b8a6eeab645e01d62d6af7747cbd755b`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:32:09 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 04 Apr 2023 18:32:09 GMT
ENV INSTALLDIR=/notary/server
# Tue, 04 Apr 2023 18:32:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 04 Apr 2023 18:32:09 GMT
WORKDIR /notary/server
# Tue, 04 Apr 2023 18:32:09 GMT
COPY /notary-server ./ # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
RUN ./notary-server --version # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
COPY ./server-config.json . # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
USER notary
# Tue, 04 Apr 2023 18:32:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:32:09 GMT
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
	-	`sha256:ae6033ff6c5306c860d176e4f63ee95200657bdf39dcac9aa5996a52c9cd2bce`  
		Last Modified: Tue, 04 Apr 2023 18:52:30 GMT  
		Size: 5.1 MB (5147706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cb2ce27c29e726a10db7f3602fff9eac81142d5cb5860961f0cfc25e4b17ed`  
		Last Modified: Tue, 04 Apr 2023 18:52:27 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b58d530011c6e6507355770a9fa7dccec9b417e55adff23aa8318bbe2419c8`  
		Last Modified: Tue, 04 Apr 2023 18:52:27 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a9201e2f6bd50eb77bd885b968b7f2cea0067972b0f8a22c0acd7cd7038140`  
		Last Modified: Tue, 04 Apr 2023 18:52:27 GMT  
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
$ docker pull notary@sha256:e694df0d62760b881cfcfdf4a98068265fd3642afc15d5c4897ae25ac46d5139
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7445278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:221135de97cdf2fdc284d293c93798e3c839dfa109544965655cfccdd42c8ff7`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:31:29 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 04 Apr 2023 18:31:29 GMT
ENV INSTALLDIR=/notary/server
# Tue, 04 Apr 2023 18:31:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 04 Apr 2023 18:31:29 GMT
WORKDIR /notary/server
# Tue, 04 Apr 2023 18:31:29 GMT
COPY /notary-server ./ # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
RUN ./notary-server --version # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
COPY ./server-config.json . # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
USER notary
# Tue, 04 Apr 2023 18:31:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:31:29 GMT
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
	-	`sha256:4d5ccf3043141a3e6c39b3471be9e091c376d20c9b936984977a454a12cc8041`  
		Last Modified: Tue, 04 Apr 2023 18:51:03 GMT  
		Size: 4.7 MB (4733700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c7c215b81721208ca96fdbe5b1e708e0ffa5771a485ea301f55e9c43ee9d85`  
		Last Modified: Tue, 04 Apr 2023 18:51:02 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73678ec06be8c4ac10f7a68fb7ccc299c396b8800ad93e8628ad0b12239cd2e2`  
		Last Modified: Tue, 04 Apr 2023 18:51:02 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d5c7b604457ddb60c19aa06f5be53a3d1655f69d13329dedc9529049a579fe`  
		Last Modified: Tue, 04 Apr 2023 18:51:02 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; 386

```console
$ docker pull notary@sha256:1d95a7d4aefd2fdb61afd5ba0754e36945df32d1168565fd3dcdd22ebe910b91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7762889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39ce85b2a309ee388a19183ba7877bd5c16c2a78f08772b1499e4900b15ad3ad`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:38:09 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 04 Apr 2023 18:38:09 GMT
ENV INSTALLDIR=/notary/server
# Tue, 04 Apr 2023 18:38:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 04 Apr 2023 18:38:09 GMT
WORKDIR /notary/server
# Tue, 04 Apr 2023 18:38:09 GMT
COPY /notary-server ./ # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
RUN ./notary-server --version # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
COPY ./server-config.json . # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
USER notary
# Tue, 04 Apr 2023 18:38:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:38:09 GMT
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
	-	`sha256:a84b63ff713e3e110d439b56101a4e629b5a3cb4d013fa7b4c038ad4b4f6dd6b`  
		Last Modified: Tue, 04 Apr 2023 18:58:58 GMT  
		Size: 4.9 MB (4949845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479755b6f7b68df076a0131604e6628f5d46cd881499f8d888ac361a5ae44f4d`  
		Last Modified: Tue, 04 Apr 2023 18:58:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5eaff1e003f8017370ff5f8720c9e9b8ae830ceac6176a016e1f379d965e8d`  
		Last Modified: Tue, 04 Apr 2023 18:58:57 GMT  
		Size: 420.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fdc9eb5debe908895457bef757f802c43e900eb1b833dd89503a8cb3b5173e`  
		Last Modified: Tue, 04 Apr 2023 18:58:57 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:7c076eec186e8038fe69d54a66989e3a91c56f3a4b38f8770c67faab608cbd9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7445323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:493fb1d65fca182158bf5095a234c55aa5be5de759cadfde45559337025b3b82`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:38:42 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 04 Apr 2023 18:38:42 GMT
ENV INSTALLDIR=/notary/server
# Tue, 04 Apr 2023 18:38:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 04 Apr 2023 18:38:42 GMT
WORKDIR /notary/server
# Tue, 04 Apr 2023 18:38:42 GMT
COPY /notary-server ./ # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
RUN ./notary-server --version # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
COPY ./server-config.json . # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
USER notary
# Tue, 04 Apr 2023 18:38:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:38:42 GMT
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
	-	`sha256:ad4a590a465c27aa5a29bd297d1e68effa8acc419174358cdd0a8a6a84820dfa`  
		Last Modified: Tue, 04 Apr 2023 18:59:52 GMT  
		Size: 4.6 MB (4638418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5b8c26bdc75f5cd1e421d00063098d1fe5659e74739dfaa895453deb4cfe87`  
		Last Modified: Tue, 04 Apr 2023 18:59:51 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab45b68267c877393096be43ae3bb328e2070659d00516492d9c7159c75b952`  
		Last Modified: Tue, 04 Apr 2023 18:59:51 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f997fefe5793a23fad058d49b3da7ec402d10ed3bf37ee62d2a37f7e77ab1f0`  
		Last Modified: Tue, 04 Apr 2023 18:59:51 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:1ff9463ad5fca4543b72138ab861eb2674ecf8cad3e5fda7680134102c8a7b3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7571574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8728d93ff4f8d6b5e2bfb139a2c18ad0866f6d1693deba4967e7959a0ddf402`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:33:21 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 04 Apr 2023 18:33:21 GMT
ENV INSTALLDIR=/notary/server
# Tue, 04 Apr 2023 18:33:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 04 Apr 2023 18:33:21 GMT
WORKDIR /notary/server
# Tue, 04 Apr 2023 18:33:21 GMT
COPY /notary-server ./ # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
RUN ./notary-server --version # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
COPY ./server-config.json . # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
USER notary
# Tue, 04 Apr 2023 18:33:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:33:21 GMT
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
	-	`sha256:bef149a60bf86421301321480e056107d4635bca444c4588f5f9a59de57ae26d`  
		Last Modified: Tue, 04 Apr 2023 18:52:53 GMT  
		Size: 5.0 MB (4975954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a351f9f76c66a4782e7980ec804334bfda5ef29f54e6d8a19e8820afb8e7dc8f`  
		Last Modified: Tue, 04 Apr 2023 18:52:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2889b67f069c689b59a55d397bd670e6be326a822558227f79cd022a27a7f430`  
		Last Modified: Tue, 04 Apr 2023 18:52:52 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3a26d38711527b618620bd74986103d2c7087732b789714f8f4a062f567e99`  
		Last Modified: Tue, 04 Apr 2023 18:52:52 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer`

```console
$ docker pull notary@sha256:406003ab82570040c77414264a95843d3b056ec906dc3a64e0057e24a950e837
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
$ docker pull notary@sha256:36d5c10b7fde28f47fce62d458a8398e81195cb9085a9a5afcfe8792e92ae8db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a03dacf3a641aed14323882cef198c3d6da241e873ed59268098f825d1756e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:32:09 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 04 Apr 2023 18:32:09 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 04 Apr 2023 18:32:09 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 04 Apr 2023 18:32:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 04 Apr 2023 18:32:09 GMT
WORKDIR /notary/signer
# Tue, 04 Apr 2023 18:32:09 GMT
COPY /notary-signer ./ # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
RUN ./notary-signer --version # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
COPY ./signer-config.json . # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
USER notary
# Tue, 04 Apr 2023 18:32:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:32:09 GMT
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
	-	`sha256:3162af884d4105a755eb0eaecb14228b81920360fc42fdf7484389c692fc9a92`  
		Last Modified: Tue, 04 Apr 2023 18:52:38 GMT  
		Size: 4.8 MB (4762756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21466f806fbddbee778d9c699e8a1de7dd4920b00014a19a6bf10214585f9f98`  
		Last Modified: Tue, 04 Apr 2023 18:52:37 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea38bb7e276ef7634747a41ca594dc90d953dde8269c78b6ede293baafd7bde`  
		Last Modified: Tue, 04 Apr 2023 18:52:37 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9a1b8810ef4a9ade9f4871d3847a80e805bd0491587276bf2cca651fed662b`  
		Last Modified: Tue, 04 Apr 2023 18:52:37 GMT  
		Size: 381.0 B  
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
$ docker pull notary@sha256:0fcf82f13d8b2b6fcd735afc36a393df135d47feac65320974799fc96d9ebcaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7103769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aea1cfecae4d2efef3cb3614c16f8712bb6d628cc768a9b11c20ceb04314617d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:31:29 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 04 Apr 2023 18:31:29 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 04 Apr 2023 18:31:29 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 04 Apr 2023 18:31:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 04 Apr 2023 18:31:29 GMT
WORKDIR /notary/signer
# Tue, 04 Apr 2023 18:31:29 GMT
COPY /notary-signer ./ # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
RUN ./notary-signer --version # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
COPY ./signer-config.json . # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
USER notary
# Tue, 04 Apr 2023 18:31:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:31:29 GMT
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
	-	`sha256:15ded91381c6b10246e8fe33e83d363b0b8989c23c3300cdb0011578847230a4`  
		Last Modified: Tue, 04 Apr 2023 18:51:12 GMT  
		Size: 4.4 MB (4392261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fdff19ed1adf1e41ddc030af19dd548c16c0fb71a13bd886d31baf1155cb50`  
		Last Modified: Tue, 04 Apr 2023 18:51:11 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354cb6183cd1e5f3260e888b2fa003d25601630afd351a6ccc02109f1fc1db6d`  
		Last Modified: Tue, 04 Apr 2023 18:51:11 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5532397d492b525c603a77b1872616c6e6d9f6d0d040416ac98e8d63f2ca37`  
		Last Modified: Tue, 04 Apr 2023 18:51:11 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:bee5c7dc5937c6037312775c3a6251b8033bea7daca2e4f3d0081f4268be62fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7391088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3774259b3895c88596a21a9a8cac6cde603b64ec9805b266f98d03488652d54a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:38:09 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 04 Apr 2023 18:38:09 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 04 Apr 2023 18:38:09 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 04 Apr 2023 18:38:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 04 Apr 2023 18:38:09 GMT
WORKDIR /notary/signer
# Tue, 04 Apr 2023 18:38:09 GMT
COPY /notary-signer ./ # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
RUN ./notary-signer --version # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
COPY ./signer-config.json . # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
USER notary
# Tue, 04 Apr 2023 18:38:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:38:09 GMT
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
	-	`sha256:46856f637b7a93b957c804e390f837a183801519d18fc07bf5aa637df2ce30b7`  
		Last Modified: Tue, 04 Apr 2023 18:59:07 GMT  
		Size: 4.6 MB (4578107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912db02b25431d058cb884e1a4b8b417675456b236ccd6f7dea77dd6576e832c`  
		Last Modified: Tue, 04 Apr 2023 18:59:06 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cd65501f2bc844c4b770e4eacca5f926e2d6be106b2af3e6be140ec06d0c32`  
		Last Modified: Tue, 04 Apr 2023 18:59:06 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bf5225f62fb57bacf859ead575260ab141868300e9786e1cd8fdff6472b08`  
		Last Modified: Tue, 04 Apr 2023 18:59:06 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:1bd32d013e4ee806d728d076008dae95de9e5ca1c9bf529db71ce43c761c12fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7103340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07348a6922db2deaff97e4d1ad35de2caa2f8f3aad997dd77d49bfea8b68079e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:38:42 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 04 Apr 2023 18:38:42 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 04 Apr 2023 18:38:42 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 04 Apr 2023 18:38:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 04 Apr 2023 18:38:42 GMT
WORKDIR /notary/signer
# Tue, 04 Apr 2023 18:38:42 GMT
COPY /notary-signer ./ # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
RUN ./notary-signer --version # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
COPY ./signer-config.json . # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
USER notary
# Tue, 04 Apr 2023 18:38:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:38:42 GMT
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
	-	`sha256:0ff1714e341c85dd971ba41d74bdaa073d525ccbf8c33cd6d3467a1699212201`  
		Last Modified: Tue, 04 Apr 2023 19:00:02 GMT  
		Size: 4.3 MB (4296501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7034896014762380cb09a2ba85d5e418a6b40e06496d7a3b0fc3c9aa6ff60a5f`  
		Last Modified: Tue, 04 Apr 2023 19:00:01 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a292ccb70d0c5d4c4be697b830a2ac21033613d93dc32e7e068c06cdf83b94b`  
		Last Modified: Tue, 04 Apr 2023 19:00:01 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b686f2dafaa4a0757515ba98efc1351c5ec1e1e277ed9adef82ca916037300`  
		Last Modified: Tue, 04 Apr 2023 19:00:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:334366b6fd0f9b2475e52ae2b224c68c8a0e343854ad92d170b1a5dcec69d716
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7202063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8426d7573f81420d78a45ca52eeb30a7619203e49f37300559c5dfa07b4d656d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:33:21 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 04 Apr 2023 18:33:21 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 04 Apr 2023 18:33:21 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 04 Apr 2023 18:33:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 04 Apr 2023 18:33:21 GMT
WORKDIR /notary/signer
# Tue, 04 Apr 2023 18:33:21 GMT
COPY /notary-signer ./ # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
RUN ./notary-signer --version # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
COPY ./signer-config.json . # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
USER notary
# Tue, 04 Apr 2023 18:33:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:33:21 GMT
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
	-	`sha256:6d65ac856817c57ca3a19cb326e4cde24a9e96e836b9e0fa903a1501aa7965dd`  
		Last Modified: Tue, 04 Apr 2023 18:52:59 GMT  
		Size: 4.6 MB (4606507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e63347de19b00def29df66f6b46ab2d2cc1087eeedeb1481df8e3d1e0b4be`  
		Last Modified: Tue, 04 Apr 2023 18:52:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a05482ca17b13a4443a2e11ff755118c6c2146cceb13673dafe958752e57aaf`  
		Last Modified: Tue, 04 Apr 2023 18:52:58 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79085d620222e4c4888f18334b2b3a46ab823fe7f8c4371127f020681195a0db`  
		Last Modified: Tue, 04 Apr 2023 18:52:58 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer-0.7.0`

```console
$ docker pull notary@sha256:406003ab82570040c77414264a95843d3b056ec906dc3a64e0057e24a950e837
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
$ docker pull notary@sha256:36d5c10b7fde28f47fce62d458a8398e81195cb9085a9a5afcfe8792e92ae8db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a03dacf3a641aed14323882cef198c3d6da241e873ed59268098f825d1756e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:32:09 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 04 Apr 2023 18:32:09 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 04 Apr 2023 18:32:09 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 04 Apr 2023 18:32:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 04 Apr 2023 18:32:09 GMT
WORKDIR /notary/signer
# Tue, 04 Apr 2023 18:32:09 GMT
COPY /notary-signer ./ # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
RUN ./notary-signer --version # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
COPY ./signer-config.json . # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:32:09 GMT
USER notary
# Tue, 04 Apr 2023 18:32:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:32:09 GMT
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
	-	`sha256:3162af884d4105a755eb0eaecb14228b81920360fc42fdf7484389c692fc9a92`  
		Last Modified: Tue, 04 Apr 2023 18:52:38 GMT  
		Size: 4.8 MB (4762756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21466f806fbddbee778d9c699e8a1de7dd4920b00014a19a6bf10214585f9f98`  
		Last Modified: Tue, 04 Apr 2023 18:52:37 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea38bb7e276ef7634747a41ca594dc90d953dde8269c78b6ede293baafd7bde`  
		Last Modified: Tue, 04 Apr 2023 18:52:37 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9a1b8810ef4a9ade9f4871d3847a80e805bd0491587276bf2cca651fed662b`  
		Last Modified: Tue, 04 Apr 2023 18:52:37 GMT  
		Size: 381.0 B  
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
$ docker pull notary@sha256:0fcf82f13d8b2b6fcd735afc36a393df135d47feac65320974799fc96d9ebcaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7103769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aea1cfecae4d2efef3cb3614c16f8712bb6d628cc768a9b11c20ceb04314617d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:31:29 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 04 Apr 2023 18:31:29 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 04 Apr 2023 18:31:29 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 04 Apr 2023 18:31:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 04 Apr 2023 18:31:29 GMT
WORKDIR /notary/signer
# Tue, 04 Apr 2023 18:31:29 GMT
COPY /notary-signer ./ # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
RUN ./notary-signer --version # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
COPY ./signer-config.json . # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:31:29 GMT
USER notary
# Tue, 04 Apr 2023 18:31:29 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:31:29 GMT
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
	-	`sha256:15ded91381c6b10246e8fe33e83d363b0b8989c23c3300cdb0011578847230a4`  
		Last Modified: Tue, 04 Apr 2023 18:51:12 GMT  
		Size: 4.4 MB (4392261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fdff19ed1adf1e41ddc030af19dd548c16c0fb71a13bd886d31baf1155cb50`  
		Last Modified: Tue, 04 Apr 2023 18:51:11 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354cb6183cd1e5f3260e888b2fa003d25601630afd351a6ccc02109f1fc1db6d`  
		Last Modified: Tue, 04 Apr 2023 18:51:11 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5532397d492b525c603a77b1872616c6e6d9f6d0d040416ac98e8d63f2ca37`  
		Last Modified: Tue, 04 Apr 2023 18:51:11 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; 386

```console
$ docker pull notary@sha256:bee5c7dc5937c6037312775c3a6251b8033bea7daca2e4f3d0081f4268be62fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7391088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3774259b3895c88596a21a9a8cac6cde603b64ec9805b266f98d03488652d54a`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:38:09 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 04 Apr 2023 18:38:09 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 04 Apr 2023 18:38:09 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 04 Apr 2023 18:38:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 04 Apr 2023 18:38:09 GMT
WORKDIR /notary/signer
# Tue, 04 Apr 2023 18:38:09 GMT
COPY /notary-signer ./ # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
RUN ./notary-signer --version # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
COPY ./signer-config.json . # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:38:09 GMT
USER notary
# Tue, 04 Apr 2023 18:38:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:38:09 GMT
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
	-	`sha256:46856f637b7a93b957c804e390f837a183801519d18fc07bf5aa637df2ce30b7`  
		Last Modified: Tue, 04 Apr 2023 18:59:07 GMT  
		Size: 4.6 MB (4578107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912db02b25431d058cb884e1a4b8b417675456b236ccd6f7dea77dd6576e832c`  
		Last Modified: Tue, 04 Apr 2023 18:59:06 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cd65501f2bc844c4b770e4eacca5f926e2d6be106b2af3e6be140ec06d0c32`  
		Last Modified: Tue, 04 Apr 2023 18:59:06 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314bf5225f62fb57bacf859ead575260ab141868300e9786e1cd8fdff6472b08`  
		Last Modified: Tue, 04 Apr 2023 18:59:06 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:1bd32d013e4ee806d728d076008dae95de9e5ca1c9bf529db71ce43c761c12fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7103340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07348a6922db2deaff97e4d1ad35de2caa2f8f3aad997dd77d49bfea8b68079e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:38:42 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 04 Apr 2023 18:38:42 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 04 Apr 2023 18:38:42 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 04 Apr 2023 18:38:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 04 Apr 2023 18:38:42 GMT
WORKDIR /notary/signer
# Tue, 04 Apr 2023 18:38:42 GMT
COPY /notary-signer ./ # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
RUN ./notary-signer --version # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
COPY ./signer-config.json . # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:38:42 GMT
USER notary
# Tue, 04 Apr 2023 18:38:42 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:38:42 GMT
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
	-	`sha256:0ff1714e341c85dd971ba41d74bdaa073d525ccbf8c33cd6d3467a1699212201`  
		Last Modified: Tue, 04 Apr 2023 19:00:02 GMT  
		Size: 4.3 MB (4296501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7034896014762380cb09a2ba85d5e418a6b40e06496d7a3b0fc3c9aa6ff60a5f`  
		Last Modified: Tue, 04 Apr 2023 19:00:01 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a292ccb70d0c5d4c4be697b830a2ac21033613d93dc32e7e068c06cdf83b94b`  
		Last Modified: Tue, 04 Apr 2023 19:00:01 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b686f2dafaa4a0757515ba98efc1351c5ec1e1e277ed9adef82ca916037300`  
		Last Modified: Tue, 04 Apr 2023 19:00:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:334366b6fd0f9b2475e52ae2b224c68c8a0e343854ad92d170b1a5dcec69d716
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7202063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8426d7573f81420d78a45ca52eeb30a7619203e49f37300559c5dfa07b4d656d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 04 Apr 2023 18:33:21 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 04 Apr 2023 18:33:21 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 04 Apr 2023 18:33:21 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 04 Apr 2023 18:33:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 04 Apr 2023 18:33:21 GMT
WORKDIR /notary/signer
# Tue, 04 Apr 2023 18:33:21 GMT
COPY /notary-signer ./ # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
RUN ./notary-signer --version # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
COPY ./signer-config.json . # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 04 Apr 2023 18:33:21 GMT
USER notary
# Tue, 04 Apr 2023 18:33:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 04 Apr 2023 18:33:21 GMT
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
	-	`sha256:6d65ac856817c57ca3a19cb326e4cde24a9e96e836b9e0fa903a1501aa7965dd`  
		Last Modified: Tue, 04 Apr 2023 18:52:59 GMT  
		Size: 4.6 MB (4606507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7e63347de19b00def29df66f6b46ab2d2cc1087eeedeb1481df8e3d1e0b4be`  
		Last Modified: Tue, 04 Apr 2023 18:52:58 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a05482ca17b13a4443a2e11ff755118c6c2146cceb13673dafe958752e57aaf`  
		Last Modified: Tue, 04 Apr 2023 18:52:58 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79085d620222e4c4888f18334b2b3a46ab823fe7f8c4371127f020681195a0db`  
		Last Modified: Tue, 04 Apr 2023 18:52:58 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
