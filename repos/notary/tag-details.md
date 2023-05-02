<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `notary`

-	[`notary:server`](#notaryserver)
-	[`notary:server-0.7.0`](#notaryserver-070)
-	[`notary:signer`](#notarysigner)
-	[`notary:signer-0.7.0`](#notarysigner-070)

## `notary:server`

```console
$ docker pull notary@sha256:3a9a8e087049d5df62e0ffbce9fd63f1769fdd65b0931e2732e64b2c8d82a0cf
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
$ docker pull notary@sha256:a8201173483cb211c24326512f4d6e298acf64694ce15c3562fa5bba50d200e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7512652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c360688283460f13221fb5dae30dc3548b7601f884caebabc4d27ca1babcfda6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:45:24 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:45:24 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 02 May 2023 18:45:24 GMT
ENV INSTALLDIR=/notary/server
# Tue, 02 May 2023 18:45:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 02 May 2023 18:45:24 GMT
WORKDIR /notary/server
# Tue, 02 May 2023 18:45:24 GMT
COPY /notary-server ./ # buildkit
# Tue, 02 May 2023 18:45:24 GMT
RUN ./notary-server --version # buildkit
# Tue, 02 May 2023 18:45:24 GMT
COPY ./server-config.json . # buildkit
# Tue, 02 May 2023 18:45:24 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:45:24 GMT
USER notary
# Tue, 02 May 2023 18:45:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:45:24 GMT
CMD ["notary-server" "--version"]
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
	-	`sha256:ab11cf2ddb415363607d7a44c9acca8d79c797b1ba474fc880f2009dce5575ba`  
		Last Modified: Sat, 08 Apr 2023 00:16:31 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a134c6cc7ea37b2ec046af3175a8cf2387f0977ce0d7bba8f869b7d259781`  
		Last Modified: Tue, 02 May 2023 19:08:03 GMT  
		Size: 4.9 MB (4893575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351534d2c473ad7169471a1c314fa6b5137336e797f74f151cc280b7205a6ba4`  
		Last Modified: Tue, 02 May 2023 19:08:02 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f01fa126d14c1e87100b581d4cfde9dd96bd7af615f780f854529dbf5f1f37`  
		Last Modified: Tue, 02 May 2023 19:08:02 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22ef035e28e63c590c8f53395e52b224c38a95e7aeea0d7000cf2e155a595aa`  
		Last Modified: Tue, 02 May 2023 19:08:02 GMT  
		Size: 382.0 B  
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
$ docker pull notary@sha256:68393a4e185d139e358c8dfaa97ffcbaa667fcd0ff45647de4203f3eda3ab97f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7763826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935cb249bf13bc3961d21f81e31ed017e69da2e0ed7cea17839ccf1353c86776`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:50:10 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:50:10 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 02 May 2023 18:50:10 GMT
ENV INSTALLDIR=/notary/server
# Tue, 02 May 2023 18:50:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 02 May 2023 18:50:10 GMT
WORKDIR /notary/server
# Tue, 02 May 2023 18:50:10 GMT
COPY /notary-server ./ # buildkit
# Tue, 02 May 2023 18:50:10 GMT
RUN ./notary-server --version # buildkit
# Tue, 02 May 2023 18:50:10 GMT
COPY ./server-config.json . # buildkit
# Tue, 02 May 2023 18:50:10 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:50:10 GMT
USER notary
# Tue, 02 May 2023 18:50:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:50:10 GMT
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
	-	`sha256:4f80ad87e3774805092bb5683294c6a76355af6830865e0ac78b13fb860ef24d`  
		Last Modified: Tue, 02 May 2023 19:10:50 GMT  
		Size: 5.0 MB (4950778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3f11638dfa02e7297a61f22a6672d00f03712f5b945084f22cbe7a9dce42bf`  
		Last Modified: Tue, 02 May 2023 19:10:49 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cba988801087fc69387af6c351dab4779ee3ba548f3e874de04a5a1002863e`  
		Last Modified: Tue, 02 May 2023 19:10:49 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cd63622d83cdbc333d9ed47700522ce7a12408cf6728792112599827cce254`  
		Last Modified: Tue, 02 May 2023 19:10:49 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; ppc64le

```console
$ docker pull notary@sha256:995dcdf8f9c15a4a963963fad1d6042b8ad0e06deb28b75ecf775c24399eef57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7446064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:470d9a3e9aea1dd1df8ab6b019d016b59fe2fecd1e65653682819b9898e48fd1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:59:30 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:59:30 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 02 May 2023 18:59:30 GMT
ENV INSTALLDIR=/notary/server
# Tue, 02 May 2023 18:59:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 02 May 2023 18:59:30 GMT
WORKDIR /notary/server
# Tue, 02 May 2023 18:59:30 GMT
COPY /notary-server ./ # buildkit
# Tue, 02 May 2023 18:59:30 GMT
RUN ./notary-server --version # buildkit
# Tue, 02 May 2023 18:59:30 GMT
COPY ./server-config.json . # buildkit
# Tue, 02 May 2023 18:59:30 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:59:30 GMT
USER notary
# Tue, 02 May 2023 18:59:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:59:30 GMT
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
	-	`sha256:ec548c148335efb5453a17cc8d52545e486b867cae158b89083b00eb0203ddfb`  
		Last Modified: Tue, 02 May 2023 19:21:01 GMT  
		Size: 4.6 MB (4639159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4045ae21ea722ca350703b16b17124683d99800f35cc75fdded0ca83275dfc`  
		Last Modified: Tue, 02 May 2023 19:21:00 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eab81832d11ffb94780846be158da2eb98981eb44ca40f7f78576e41bc71c6c`  
		Last Modified: Tue, 02 May 2023 19:21:00 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405f96efaca407897452c1ad302aa1eea404e65957b6b1c755cbdcab9d1961fb`  
		Last Modified: Tue, 02 May 2023 19:21:00 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:46222102af49c089bdd985dc3a9c9e396e4132f7472daf8bbc8c0948eaaedde0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc73865af693435b5f688b2cefee44b2d4bf02679a776101a457ed1d85949b8`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:45:37 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:45:37 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 02 May 2023 18:45:37 GMT
ENV INSTALLDIR=/notary/server
# Tue, 02 May 2023 18:45:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 02 May 2023 18:45:37 GMT
WORKDIR /notary/server
# Tue, 02 May 2023 18:45:37 GMT
COPY /notary-server ./ # buildkit
# Tue, 02 May 2023 18:45:37 GMT
RUN ./notary-server --version # buildkit
# Tue, 02 May 2023 18:45:37 GMT
COPY ./server-config.json . # buildkit
# Tue, 02 May 2023 18:45:37 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:45:37 GMT
USER notary
# Tue, 02 May 2023 18:45:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:45:37 GMT
CMD ["notary-server" "--version"]
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
	-	`sha256:a1be685ead59433921acfa36285b0d513c970b7e82ab7594887f7bdd7ae37527`  
		Last Modified: Tue, 02 May 2023 19:14:48 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab63e1bbe686eb9921ae2cc757a2f3a08a4f9ca3ff21a92c5e585ff02419a8`  
		Last Modified: Tue, 02 May 2023 19:14:49 GMT  
		Size: 5.0 MB (4976490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c85d7ee22e60d478fbf8ea9d90ea62a303179efb20bdc85955876a100ffb6b`  
		Last Modified: Tue, 02 May 2023 19:14:48 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c832954401746d66fbcb12d064382b41ae4fec14f65e876b184628387f802604`  
		Last Modified: Tue, 02 May 2023 19:14:48 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb44149a8d8cccb958cf42b938950bc2199a6db43ff94dd7a1f10585d896467`  
		Last Modified: Tue, 02 May 2023 19:14:48 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:server-0.7.0`

```console
$ docker pull notary@sha256:3a9a8e087049d5df62e0ffbce9fd63f1769fdd65b0931e2732e64b2c8d82a0cf
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
$ docker pull notary@sha256:a8201173483cb211c24326512f4d6e298acf64694ce15c3562fa5bba50d200e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7512652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c360688283460f13221fb5dae30dc3548b7601f884caebabc4d27ca1babcfda6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:45:24 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:45:24 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 02 May 2023 18:45:24 GMT
ENV INSTALLDIR=/notary/server
# Tue, 02 May 2023 18:45:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 02 May 2023 18:45:24 GMT
WORKDIR /notary/server
# Tue, 02 May 2023 18:45:24 GMT
COPY /notary-server ./ # buildkit
# Tue, 02 May 2023 18:45:24 GMT
RUN ./notary-server --version # buildkit
# Tue, 02 May 2023 18:45:24 GMT
COPY ./server-config.json . # buildkit
# Tue, 02 May 2023 18:45:24 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:45:24 GMT
USER notary
# Tue, 02 May 2023 18:45:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:45:24 GMT
CMD ["notary-server" "--version"]
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
	-	`sha256:ab11cf2ddb415363607d7a44c9acca8d79c797b1ba474fc880f2009dce5575ba`  
		Last Modified: Sat, 08 Apr 2023 00:16:31 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a134c6cc7ea37b2ec046af3175a8cf2387f0977ce0d7bba8f869b7d259781`  
		Last Modified: Tue, 02 May 2023 19:08:03 GMT  
		Size: 4.9 MB (4893575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351534d2c473ad7169471a1c314fa6b5137336e797f74f151cc280b7205a6ba4`  
		Last Modified: Tue, 02 May 2023 19:08:02 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f01fa126d14c1e87100b581d4cfde9dd96bd7af615f780f854529dbf5f1f37`  
		Last Modified: Tue, 02 May 2023 19:08:02 GMT  
		Size: 421.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22ef035e28e63c590c8f53395e52b224c38a95e7aeea0d7000cf2e155a595aa`  
		Last Modified: Tue, 02 May 2023 19:08:02 GMT  
		Size: 382.0 B  
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
$ docker pull notary@sha256:68393a4e185d139e358c8dfaa97ffcbaa667fcd0ff45647de4203f3eda3ab97f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7763826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:935cb249bf13bc3961d21f81e31ed017e69da2e0ed7cea17839ccf1353c86776`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:50:10 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:50:10 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 02 May 2023 18:50:10 GMT
ENV INSTALLDIR=/notary/server
# Tue, 02 May 2023 18:50:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 02 May 2023 18:50:10 GMT
WORKDIR /notary/server
# Tue, 02 May 2023 18:50:10 GMT
COPY /notary-server ./ # buildkit
# Tue, 02 May 2023 18:50:10 GMT
RUN ./notary-server --version # buildkit
# Tue, 02 May 2023 18:50:10 GMT
COPY ./server-config.json . # buildkit
# Tue, 02 May 2023 18:50:10 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:50:10 GMT
USER notary
# Tue, 02 May 2023 18:50:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:50:10 GMT
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
	-	`sha256:4f80ad87e3774805092bb5683294c6a76355af6830865e0ac78b13fb860ef24d`  
		Last Modified: Tue, 02 May 2023 19:10:50 GMT  
		Size: 5.0 MB (4950778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3f11638dfa02e7297a61f22a6672d00f03712f5b945084f22cbe7a9dce42bf`  
		Last Modified: Tue, 02 May 2023 19:10:49 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cba988801087fc69387af6c351dab4779ee3ba548f3e874de04a5a1002863e`  
		Last Modified: Tue, 02 May 2023 19:10:49 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cd63622d83cdbc333d9ed47700522ce7a12408cf6728792112599827cce254`  
		Last Modified: Tue, 02 May 2023 19:10:49 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:995dcdf8f9c15a4a963963fad1d6042b8ad0e06deb28b75ecf775c24399eef57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7446064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:470d9a3e9aea1dd1df8ab6b019d016b59fe2fecd1e65653682819b9898e48fd1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:59:30 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:59:30 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 02 May 2023 18:59:30 GMT
ENV INSTALLDIR=/notary/server
# Tue, 02 May 2023 18:59:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 02 May 2023 18:59:30 GMT
WORKDIR /notary/server
# Tue, 02 May 2023 18:59:30 GMT
COPY /notary-server ./ # buildkit
# Tue, 02 May 2023 18:59:30 GMT
RUN ./notary-server --version # buildkit
# Tue, 02 May 2023 18:59:30 GMT
COPY ./server-config.json . # buildkit
# Tue, 02 May 2023 18:59:30 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:59:30 GMT
USER notary
# Tue, 02 May 2023 18:59:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:59:30 GMT
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
	-	`sha256:ec548c148335efb5453a17cc8d52545e486b867cae158b89083b00eb0203ddfb`  
		Last Modified: Tue, 02 May 2023 19:21:01 GMT  
		Size: 4.6 MB (4639159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4045ae21ea722ca350703b16b17124683d99800f35cc75fdded0ca83275dfc`  
		Last Modified: Tue, 02 May 2023 19:21:00 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eab81832d11ffb94780846be158da2eb98981eb44ca40f7f78576e41bc71c6c`  
		Last Modified: Tue, 02 May 2023 19:21:00 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405f96efaca407897452c1ad302aa1eea404e65957b6b1c755cbdcab9d1961fb`  
		Last Modified: Tue, 02 May 2023 19:21:00 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:46222102af49c089bdd985dc3a9c9e396e4132f7472daf8bbc8c0948eaaedde0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7572110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc73865af693435b5f688b2cefee44b2d4bf02679a776101a457ed1d85949b8`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:45:37 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:45:37 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 02 May 2023 18:45:37 GMT
ENV INSTALLDIR=/notary/server
# Tue, 02 May 2023 18:45:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 02 May 2023 18:45:37 GMT
WORKDIR /notary/server
# Tue, 02 May 2023 18:45:37 GMT
COPY /notary-server ./ # buildkit
# Tue, 02 May 2023 18:45:37 GMT
RUN ./notary-server --version # buildkit
# Tue, 02 May 2023 18:45:37 GMT
COPY ./server-config.json . # buildkit
# Tue, 02 May 2023 18:45:37 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:45:37 GMT
USER notary
# Tue, 02 May 2023 18:45:37 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:45:37 GMT
CMD ["notary-server" "--version"]
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
	-	`sha256:a1be685ead59433921acfa36285b0d513c970b7e82ab7594887f7bdd7ae37527`  
		Last Modified: Tue, 02 May 2023 19:14:48 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ab63e1bbe686eb9921ae2cc757a2f3a08a4f9ca3ff21a92c5e585ff02419a8`  
		Last Modified: Tue, 02 May 2023 19:14:49 GMT  
		Size: 5.0 MB (4976490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c85d7ee22e60d478fbf8ea9d90ea62a303179efb20bdc85955876a100ffb6b`  
		Last Modified: Tue, 02 May 2023 19:14:48 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c832954401746d66fbcb12d064382b41ae4fec14f65e876b184628387f802604`  
		Last Modified: Tue, 02 May 2023 19:14:48 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb44149a8d8cccb958cf42b938950bc2199a6db43ff94dd7a1f10585d896467`  
		Last Modified: Tue, 02 May 2023 19:14:48 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer`

```console
$ docker pull notary@sha256:4b7ebb56f2bdb9ea8e33ce422e7aeee0d718ca90e6a6f750848e619305cb7625
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
$ docker pull notary@sha256:38710212115407207fb377199da7b53b2c37cf70c943bcfdc52ae80f0093dbe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7145112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70bba8a230a547302ae5ffdb8fa9bc59dfcfb31901a678c189757b71ff01d872`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:45:24 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:45:24 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 02 May 2023 18:45:24 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 02 May 2023 18:45:24 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 02 May 2023 18:45:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 02 May 2023 18:45:24 GMT
WORKDIR /notary/signer
# Tue, 02 May 2023 18:45:24 GMT
COPY /notary-signer ./ # buildkit
# Tue, 02 May 2023 18:45:24 GMT
RUN ./notary-signer --version # buildkit
# Tue, 02 May 2023 18:45:24 GMT
COPY ./signer-config.json . # buildkit
# Tue, 02 May 2023 18:45:24 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:45:24 GMT
USER notary
# Tue, 02 May 2023 18:45:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:45:24 GMT
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
	-	`sha256:985571b50fceeef45648df5d20772dc5e8ae3412fb9373c2d9864c13ef94dccc`  
		Last Modified: Tue, 02 May 2023 19:08:13 GMT  
		Size: 4.5 MB (4526100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5fc4bcd2b5a38aae7b838686b0833f024382f9659b6851e89e61f659199f35`  
		Last Modified: Tue, 02 May 2023 19:08:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bb90677eca807706f1d222b20d38bf95349c61d35b1c79044c7d46fc009d8a`  
		Last Modified: Tue, 02 May 2023 19:08:12 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a854b9445d63c3ae389e67c3bdee0acdd4c17da77b865582a611676ff3e980a8`  
		Last Modified: Tue, 02 May 2023 19:08:12 GMT  
		Size: 381.0 B  
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
$ docker pull notary@sha256:d7cdf30f4276b066b7d28ddeec5676a10800e9b569d7359bc893b9a695332c03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7392017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bce824baf773077b76c37146a3d47ce75ac298ed9170219f23399a0c94c6069e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:50:10 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:50:10 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 02 May 2023 18:50:10 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 02 May 2023 18:50:10 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 02 May 2023 18:50:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 02 May 2023 18:50:10 GMT
WORKDIR /notary/signer
# Tue, 02 May 2023 18:50:10 GMT
COPY /notary-signer ./ # buildkit
# Tue, 02 May 2023 18:50:10 GMT
RUN ./notary-signer --version # buildkit
# Tue, 02 May 2023 18:50:10 GMT
COPY ./signer-config.json . # buildkit
# Tue, 02 May 2023 18:50:10 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:50:10 GMT
USER notary
# Tue, 02 May 2023 18:50:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:50:10 GMT
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
	-	`sha256:38116ac7a0ae3cc1437fa49411f1be4fa0ed44da6cb74f62aa4a3f1f2794479f`  
		Last Modified: Tue, 02 May 2023 19:10:59 GMT  
		Size: 4.6 MB (4579035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28691e3aff82aca0e479bd4eb9220644c03854b21ae8952b1a713ce6db310e2`  
		Last Modified: Tue, 02 May 2023 19:10:57 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520d3d39c233bfe645c240aedcf1203dc5497bfd4b1273f132a6fac6507ce6de`  
		Last Modified: Tue, 02 May 2023 19:10:57 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe46dd6d15c384ea9d565639b1ba6f61a1442bcbdd1d850a6f20a2d1f94b49a6`  
		Last Modified: Tue, 02 May 2023 19:10:57 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:22e5fe703de89760a0b88205534489b7485d1d3aadd3b3856b5715413f5c646b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7103809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45d225edff552fcc23b40390d1b796549399081dd948634abb462af0c0e2fc8e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:59:30 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:59:30 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 02 May 2023 18:59:30 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 02 May 2023 18:59:30 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 02 May 2023 18:59:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 02 May 2023 18:59:30 GMT
WORKDIR /notary/signer
# Tue, 02 May 2023 18:59:30 GMT
COPY /notary-signer ./ # buildkit
# Tue, 02 May 2023 18:59:30 GMT
RUN ./notary-signer --version # buildkit
# Tue, 02 May 2023 18:59:30 GMT
COPY ./signer-config.json . # buildkit
# Tue, 02 May 2023 18:59:30 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:59:30 GMT
USER notary
# Tue, 02 May 2023 18:59:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:59:30 GMT
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
	-	`sha256:cd8f481dcaf2602b5c07210766e197690dfe7536f23391e9272670041adf9288`  
		Last Modified: Tue, 02 May 2023 19:21:11 GMT  
		Size: 4.3 MB (4296966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cded48918e12d746847b5ba2aae1324b90db1bc277f396d1ba2967beb4f8e7`  
		Last Modified: Tue, 02 May 2023 19:21:10 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f53a16900592987aab71523c5c7f1b47e74f96b5d407b2e01f4df53d5bdcfb`  
		Last Modified: Tue, 02 May 2023 19:21:10 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a552d417236a9ef9e27e299a6c5bdccbf7650d555885d434e88380ccc93f6e`  
		Last Modified: Tue, 02 May 2023 19:21:10 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

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

## `notary:signer-0.7.0`

```console
$ docker pull notary@sha256:4b7ebb56f2bdb9ea8e33ce422e7aeee0d718ca90e6a6f750848e619305cb7625
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
$ docker pull notary@sha256:38710212115407207fb377199da7b53b2c37cf70c943bcfdc52ae80f0093dbe3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7145112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70bba8a230a547302ae5ffdb8fa9bc59dfcfb31901a678c189757b71ff01d872`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:45:24 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:45:24 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 02 May 2023 18:45:24 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 02 May 2023 18:45:24 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 02 May 2023 18:45:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 02 May 2023 18:45:24 GMT
WORKDIR /notary/signer
# Tue, 02 May 2023 18:45:24 GMT
COPY /notary-signer ./ # buildkit
# Tue, 02 May 2023 18:45:24 GMT
RUN ./notary-signer --version # buildkit
# Tue, 02 May 2023 18:45:24 GMT
COPY ./signer-config.json . # buildkit
# Tue, 02 May 2023 18:45:24 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:45:24 GMT
USER notary
# Tue, 02 May 2023 18:45:24 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:45:24 GMT
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
	-	`sha256:985571b50fceeef45648df5d20772dc5e8ae3412fb9373c2d9864c13ef94dccc`  
		Last Modified: Tue, 02 May 2023 19:08:13 GMT  
		Size: 4.5 MB (4526100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5fc4bcd2b5a38aae7b838686b0833f024382f9659b6851e89e61f659199f35`  
		Last Modified: Tue, 02 May 2023 19:08:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bb90677eca807706f1d222b20d38bf95349c61d35b1c79044c7d46fc009d8a`  
		Last Modified: Tue, 02 May 2023 19:08:12 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a854b9445d63c3ae389e67c3bdee0acdd4c17da77b865582a611676ff3e980a8`  
		Last Modified: Tue, 02 May 2023 19:08:12 GMT  
		Size: 381.0 B  
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
$ docker pull notary@sha256:d7cdf30f4276b066b7d28ddeec5676a10800e9b569d7359bc893b9a695332c03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7392017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bce824baf773077b76c37146a3d47ce75ac298ed9170219f23399a0c94c6069e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:50:10 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:50:10 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 02 May 2023 18:50:10 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 02 May 2023 18:50:10 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 02 May 2023 18:50:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 02 May 2023 18:50:10 GMT
WORKDIR /notary/signer
# Tue, 02 May 2023 18:50:10 GMT
COPY /notary-signer ./ # buildkit
# Tue, 02 May 2023 18:50:10 GMT
RUN ./notary-signer --version # buildkit
# Tue, 02 May 2023 18:50:10 GMT
COPY ./signer-config.json . # buildkit
# Tue, 02 May 2023 18:50:10 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:50:10 GMT
USER notary
# Tue, 02 May 2023 18:50:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:50:10 GMT
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
	-	`sha256:38116ac7a0ae3cc1437fa49411f1be4fa0ed44da6cb74f62aa4a3f1f2794479f`  
		Last Modified: Tue, 02 May 2023 19:10:59 GMT  
		Size: 4.6 MB (4579035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28691e3aff82aca0e479bd4eb9220644c03854b21ae8952b1a713ce6db310e2`  
		Last Modified: Tue, 02 May 2023 19:10:57 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520d3d39c233bfe645c240aedcf1203dc5497bfd4b1273f132a6fac6507ce6de`  
		Last Modified: Tue, 02 May 2023 19:10:57 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe46dd6d15c384ea9d565639b1ba6f61a1442bcbdd1d850a6f20a2d1f94b49a6`  
		Last Modified: Tue, 02 May 2023 19:10:57 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:22e5fe703de89760a0b88205534489b7485d1d3aadd3b3856b5715413f5c646b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7103809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45d225edff552fcc23b40390d1b796549399081dd948634abb462af0c0e2fc8e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 18:59:30 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 02 May 2023 18:59:30 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 02 May 2023 18:59:30 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 02 May 2023 18:59:30 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 02 May 2023 18:59:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 02 May 2023 18:59:30 GMT
WORKDIR /notary/signer
# Tue, 02 May 2023 18:59:30 GMT
COPY /notary-signer ./ # buildkit
# Tue, 02 May 2023 18:59:30 GMT
RUN ./notary-signer --version # buildkit
# Tue, 02 May 2023 18:59:30 GMT
COPY ./signer-config.json . # buildkit
# Tue, 02 May 2023 18:59:30 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 02 May 2023 18:59:30 GMT
USER notary
# Tue, 02 May 2023 18:59:30 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 02 May 2023 18:59:30 GMT
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
	-	`sha256:cd8f481dcaf2602b5c07210766e197690dfe7536f23391e9272670041adf9288`  
		Last Modified: Tue, 02 May 2023 19:21:11 GMT  
		Size: 4.3 MB (4296966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cded48918e12d746847b5ba2aae1324b90db1bc277f396d1ba2967beb4f8e7`  
		Last Modified: Tue, 02 May 2023 19:21:10 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f53a16900592987aab71523c5c7f1b47e74f96b5d407b2e01f4df53d5bdcfb`  
		Last Modified: Tue, 02 May 2023 19:21:10 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a552d417236a9ef9e27e299a6c5bdccbf7650d555885d434e88380ccc93f6e`  
		Last Modified: Tue, 02 May 2023 19:21:10 GMT  
		Size: 385.0 B  
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
