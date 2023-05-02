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
