## `notary:signer`

```console
$ docker pull notary@sha256:a2e4364bd825119d4ec8d5f28f89e3917b33ecf4062f1cd8715de62620073b34
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
$ docker pull notary@sha256:82e6cd74a4dd40ffa22a7171e7fd0a013e59f87577b37bd82089cc62cf48bf6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7571272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08054659a657d14063d1a7d6e89021e83b764bba98b922fe7c4d07cfc7535454`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:19:28 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 18:19:28 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 18:19:28 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 18:19:28 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 18:19:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 18:19:28 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 18:19:28 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 18:19:28 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 18:19:28 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 18:19:28 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 18:19:28 GMT
USER notary
# Wed, 29 Mar 2023 18:19:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 18:19:28 GMT
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
	-	`sha256:c8a5272838ec44589c294ff87c9fed67ea835505803f114918c0e9d078c75d6c`  
		Last Modified: Wed, 29 Mar 2023 19:32:03 GMT  
		Size: 4.8 MB (4761329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9029690a2f5060d5204b6e65bbe79c9584edc7f2dd4c0ad30904d9e788c1cb6c`  
		Last Modified: Wed, 29 Mar 2023 19:32:02 GMT  
		Size: 89.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95da760519592321c41dd788dd127d45f8add2a4af924d0d60c269af2b17fc68`  
		Last Modified: Wed, 29 Mar 2023 19:32:02 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c054a9bc9cb6a5f4374f9fc7c2bcdd000d44a564df84e863e7447702fdcbda`  
		Last Modified: Wed, 29 Mar 2023 19:32:02 GMT  
		Size: 372.0 B  
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
$ docker pull notary@sha256:10c586a083e1cf792bb6b0682382049a016d694026a180b33c4c6318518fccd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7101547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:029d8b16e8f0c4de8efb5bcd1c92443c642a4304b88a248e0b001fb2c565535c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 17:39:20 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 17:39:20 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 17:39:20 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 17:39:20 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 17:39:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 17:39:20 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 17:39:20 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 17:39:20 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 17:39:20 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 17:39:20 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 17:39:20 GMT
USER notary
# Wed, 29 Mar 2023 17:39:20 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 17:39:20 GMT
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
	-	`sha256:f118ec6fe198848420882ff6a719579c9fa2b092eaa7f4aa4ea4caf4cc3957f3`  
		Last Modified: Wed, 29 Mar 2023 21:25:38 GMT  
		Size: 4.4 MB (4390054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7070061354df3a61218eac1ea2539ff3be9103f86ee0b09e4fb41827e762722`  
		Last Modified: Wed, 29 Mar 2023 21:25:38 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14d55688805c2e1c614d513ecb4d7f4870837bc8e17163481e6b77a6c96e3b`  
		Last Modified: Wed, 29 Mar 2023 21:25:38 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd5a17a5c82578f1e7e67d83b1d0490a50d5648a66854ebf956001cc36d7c0`  
		Last Modified: Wed, 29 Mar 2023 21:25:38 GMT  
		Size: 376.0 B  
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
$ docker pull notary@sha256:823461cd01b0fd0259a46f88378f2ef26a524180f73e7f7c597ff1a4a0e7d9a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7200771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da5c2782a47cd55a3bd7cdf3bc6e1bbbf51e781214faf08e95d216dd742e1b3`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 17:42:02 GMT
RUN adduser -D -H -g "" notary # buildkit
# Wed, 29 Mar 2023 17:42:02 GMT
EXPOSE map[4444/tcp:{}]
# Wed, 29 Mar 2023 17:42:02 GMT
EXPOSE map[7899/tcp:{}]
# Wed, 29 Mar 2023 17:42:02 GMT
ENV INSTALLDIR=/notary/signer
# Wed, 29 Mar 2023 17:42:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Wed, 29 Mar 2023 17:42:02 GMT
WORKDIR /notary/signer
# Wed, 29 Mar 2023 17:42:02 GMT
COPY /notary-signer ./ # buildkit
# Wed, 29 Mar 2023 17:42:02 GMT
RUN ./notary-signer --version # buildkit
# Wed, 29 Mar 2023 17:42:02 GMT
COPY ./signer-config.json . # buildkit
# Wed, 29 Mar 2023 17:42:02 GMT
COPY ./entrypoint.sh . # buildkit
# Wed, 29 Mar 2023 17:42:02 GMT
USER notary
# Wed, 29 Mar 2023 17:42:02 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 29 Mar 2023 17:42:02 GMT
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
	-	`sha256:6285fd241fb1dfa279dda67f86a82bba946327691def1fa78a39f4c89ada4cca`  
		Last Modified: Wed, 29 Mar 2023 19:02:19 GMT  
		Size: 4.6 MB (4605233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6782926d2ef6333a909143ebaefd4b7625218c9d51736220d706c18042e58514`  
		Last Modified: Wed, 29 Mar 2023 19:02:18 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a74ae17430841be98efe2e7d781cd1e06e782f63bc9e518418223c65faad36`  
		Last Modified: Wed, 29 Mar 2023 19:02:18 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5dc0e9da342d2163be0a01321aec83eebcd17421d2e45306b09d0b270874ee`  
		Last Modified: Wed, 29 Mar 2023 19:02:18 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
