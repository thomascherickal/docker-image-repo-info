<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.23`](#kibana6823)
-	[`kibana:7.17.7`](#kibana7177)
-	[`kibana:8.4.3`](#kibana843)

## `kibana:6.8.23`

```console
$ docker pull kibana@sha256:dd123d133fa7e995f83eef23df6aad30c589711e6171fee8db63097a7706eae7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kibana:6.8.23` - linux; amd64

```console
$ docker pull kibana@sha256:adb468810c34ccc141f01ea79135d5a2f48d09890ecd08ce59ec94444f0a09f1
```

-	Docker Version: 20.10.10
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.8 MB (325750637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e174261beaec7ef8b8fc7e3df6b62b87e442f3451d408e7fe4525b151a061ebd`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Thu, 06 Jan 2022 22:40:29 GMT
EXPOSE 5601
# Thu, 06 Jan 2022 22:41:30 GMT
RUN yum update -y && yum install -y fontconfig freetype && yum clean all
# Thu, 06 Jan 2022 22:42:25 GMT
COPY --chown=1000:0dir:91d1ac171c4ceb98ce1764191b4bde36072fa18167199a2214eb559670a34b06 in /usr/share/kibana 
# Thu, 06 Jan 2022 22:42:28 GMT
WORKDIR /usr/share/kibana
# Thu, 06 Jan 2022 22:42:29 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Thu, 06 Jan 2022 22:42:30 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 06 Jan 2022 22:42:30 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:42:31 GMT
COPY --chown=1000:0file:60b6181f28c99b362092ea6139b6d4112ddd0bef32d52563c33b26bdc2b51318 in /usr/share/kibana/config/kibana.yml 
# Thu, 06 Jan 2022 22:42:31 GMT
COPY --chown=1000:0file:7d472d1939e23e2f10e7c5fd1e9166eefd646214aa0d8a1c09d92af71c9cbd87 in /usr/local/bin/ 
# Thu, 06 Jan 2022 22:42:34 GMT
RUN chmod g+ws /usr/share/kibana && find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Thu, 06 Jan 2022 22:42:39 GMT
RUN groupadd --gid 1000 kibana && useradd --uid 1000 --gid 1000 --home-dir /usr/share/kibana --no-create-home kibana
# Thu, 06 Jan 2022 22:42:39 GMT
USER kibana
# Thu, 06 Jan 2022 22:42:40 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=kibana org.label-schema.version=6.8.23 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.license=Elastic License license=Elastic License
# Thu, 06 Jan 2022 22:42:41 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842e4249e10492c4ab35d3e76f93cad922781f7d61752e1b4b3ca25636b5c56f`  
		Last Modified: Thu, 13 Jan 2022 16:11:43 GMT  
		Size: 61.0 MB (61010271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f4609300d658bf52b006741f5590abdf93d8d575e0ddf04ce5be28e82b50a4`  
		Last Modified: Thu, 13 Jan 2022 16:11:58 GMT  
		Size: 188.6 MB (188638449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784cf3007996898653e12b85f6cf71597349b95377a60e1c57d40aaf682ddc3e`  
		Last Modified: Thu, 13 Jan 2022 16:11:32 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e291dafdd6a7112a1b18f88f42cbef2225094f58f18d2f364d0d34006b69e1`  
		Last Modified: Thu, 13 Jan 2022 16:11:30 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c90f666fc9fbd62181b8b51f391386e0a1a137451605b6f0a105171abe51380`  
		Last Modified: Thu, 13 Jan 2022 16:11:29 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8abc3a9f73c2948571140a610a8c9f79b87c33bcbfdf320cd0f6e5d9fbe944`  
		Last Modified: Thu, 13 Jan 2022 16:11:29 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73634fb3f49af52529a1b025a3cebf50531fdbcbdb3876b7b00908dfe9dc0a85`  
		Last Modified: Thu, 13 Jan 2022 16:11:29 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:7.17.7`

**does not exist** (yet?)

## `kibana:8.4.3`

```console
$ docker pull kibana@sha256:88b09cc593f6808cb9dfc8c3c13d94aa3c798b16f0a40d66247bd5be91a318d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:8.4.3` - linux; amd64

```console
$ docker pull kibana@sha256:5f307a3a79dc3ec84c5b99d363e9b3dc5f859fb4feba57c180ff0a8526b7bc4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.7 MB (342719349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b14d91e49f3f9e306570ede88c4b0cf4591b47a0e2d4094fdd86128b75170217`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Wed, 28 Sep 2022 11:37:24 GMT
RUN EXPOSE map[5601/tcp:{}]
# Wed, 28 Sep 2022 11:37:24 GMT
RUN RUN /bin/sh -c for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Wed, 28 Sep 2022 11:37:25 GMT
RUN RUN /bin/sh -c set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Wed, 28 Sep 2022 11:37:25 GMT
RUN RUN /bin/sh -c mkdir /usr/share/fonts/local # buildkit
# Wed, 28 Sep 2022 11:37:26 GMT
RUN RUN /bin/sh -c curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Wed, 28 Sep 2022 11:37:26 GMT
RUN RUN /bin/sh -c echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Wed, 28 Sep 2022 11:37:27 GMT
RUN RUN /bin/sh -c fc-cache -v # buildkit
# Wed, 28 Sep 2022 11:38:38 GMT
RUN COPY /usr/share/kibana /usr/share/kibana # buildkit
# Wed, 28 Sep 2022 11:38:38 GMT
RUN WORKDIR /usr/share/kibana
# Wed, 28 Sep 2022 11:38:38 GMT
RUN RUN /bin/sh -c ln -s /usr/share/kibana /opt/kibana # buildkit
# Wed, 28 Sep 2022 11:38:38 GMT
RUN ENV ELASTIC_CONTAINER=true
# Wed, 28 Sep 2022 11:38:38 GMT
RUN ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Sep 2022 11:38:38 GMT
RUN COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Wed, 28 Sep 2022 11:38:38 GMT
RUN COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Wed, 28 Sep 2022 11:38:39 GMT
RUN RUN /bin/sh -c chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Wed, 28 Sep 2022 11:38:40 GMT
RUN RUN /bin/sh -c find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Wed, 28 Sep 2022 11:38:40 GMT
RUN RUN /bin/sh -c groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Wed, 28 Sep 2022 11:38:40 GMT
RUN LABEL org.label-schema.build-date=2022-09-28T11:09:19.930Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=1ceb607762eaafa726c61d6eee5b95359142d4c4 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.4.3 org.opencontainers.image.created=2022-09-28T11:09:19.930Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=1ceb607762eaafa726c61d6eee5b95359142d4c4 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.4.3
# Wed, 28 Sep 2022 11:38:40 GMT
RUN ENTRYPOINT ["/bin/tini" "--"]
# Wed, 28 Sep 2022 11:38:40 GMT
RUN CMD ["/usr/local/bin/kibana-docker"]
# Wed, 28 Sep 2022 11:38:40 GMT
RUN USER kibana
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c95cdd3809aeffa052653ed9f2cd301f3a8bfe94b628d4f8bb6573bd30e4b2`  
		Last Modified: Thu, 06 Oct 2022 09:23:06 GMT  
		Size: 11.2 MB (11166303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe091b6a49593f3b58b35fc302aa77a5ea719f3b951a50fe037b38d3fff704dc`  
		Last Modified: Thu, 06 Oct 2022 09:23:04 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fe6a6db22d19357c969fd9a73b8fb2c636187996f5f8b33e4c686f3fbded6d`  
		Last Modified: Thu, 06 Oct 2022 09:23:02 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d993a889c9ea6323084f9158e4f5ed9320434a9ae4a83ad375bae8074a821965`  
		Last Modified: Thu, 06 Oct 2022 09:23:04 GMT  
		Size: 16.5 MB (16460503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2dca2aaa53daf8e756f5ce546d9a1654be1a8882f097faa96690c1237c066`  
		Last Modified: Thu, 06 Oct 2022 09:23:02 GMT  
		Size: 5.3 KB (5285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6e56886911836539667b34b64cfeb1b26f502a00e33d419a1450e70aa73080`  
		Last Modified: Thu, 06 Oct 2022 09:23:34 GMT  
		Size: 286.3 MB (286308301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4244fdb06704b3039965c4ef9061e8d9a4bab15b5c7c41ad4b3f588456124df`  
		Last Modified: Thu, 06 Oct 2022 09:23:01 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286ad49fcc58ddf18c8956f52c68872e4580dd50430ebeb10e0fe71a6da3d028`  
		Last Modified: Thu, 06 Oct 2022 09:23:00 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63fb82ebd5a98cd11473807e7af43fe50ca9069c6c0a593393eb22aff0d5dd2`  
		Last Modified: Thu, 06 Oct 2022 09:22:59 GMT  
		Size: 4.4 KB (4379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee9f00166598d3bbf97b25d82cfaf5fd0c5ccb834349fc263baa16b26e75d58`  
		Last Modified: Thu, 06 Oct 2022 09:22:59 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6bd03fa52f1d0f7ef26b95df04488acce270adb04f6ad6e04f4876c2d069a5`  
		Last Modified: Thu, 06 Oct 2022 09:22:59 GMT  
		Size: 189.4 KB (189393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66e3c6d7cd76c0190b5ba4c7e0be238eedfe7d939cad5ba44e1492e02e7f656`  
		Last Modified: Thu, 06 Oct 2022 09:23:00 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:8.4.3` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:23103dc87e49513ffa646bf238e7cc5e07ad8e2f4918792b9b3efec70a137f7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.8 MB (355844574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72f1bf113a574e99afecc49816b639e27c632385843c443f8f12f196d06e3920`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Wed, 28 Sep 2022 11:40:41 GMT
RUN EXPOSE map[5601/tcp:{}]
# Wed, 28 Sep 2022 11:40:41 GMT
RUN RUN /bin/sh -c for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code) # buildkit
# Wed, 28 Sep 2022 11:40:44 GMT
RUN RUN /bin/sh -c set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini # buildkit
# Wed, 28 Sep 2022 11:40:44 GMT
RUN RUN /bin/sh -c mkdir /usr/share/fonts/local # buildkit
# Wed, 28 Sep 2022 11:40:47 GMT
RUN RUN /bin/sh -c curl --retry 8 -S -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc # buildkit
# Wed, 28 Sep 2022 11:40:47 GMT
RUN RUN /bin/sh -c echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c - # buildkit
# Wed, 28 Sep 2022 11:40:48 GMT
RUN RUN /bin/sh -c fc-cache -v # buildkit
# Wed, 28 Sep 2022 11:41:57 GMT
RUN COPY /usr/share/kibana /usr/share/kibana # buildkit
# Wed, 28 Sep 2022 11:41:57 GMT
RUN WORKDIR /usr/share/kibana
# Wed, 28 Sep 2022 11:41:57 GMT
RUN RUN /bin/sh -c ln -s /usr/share/kibana /opt/kibana # buildkit
# Wed, 28 Sep 2022 11:41:57 GMT
RUN ENV ELASTIC_CONTAINER=true
# Wed, 28 Sep 2022 11:41:57 GMT
RUN ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Sep 2022 11:41:57 GMT
RUN COPY config/kibana.yml /usr/share/kibana/config/kibana.yml # buildkit
# Wed, 28 Sep 2022 11:41:57 GMT
RUN COPY bin/kibana-docker /usr/local/bin/ # buildkit
# Wed, 28 Sep 2022 11:41:58 GMT
RUN RUN /bin/sh -c chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \; # buildkit
# Wed, 28 Sep 2022 11:41:59 GMT
RUN RUN /bin/sh -c find / -xdev -perm -4000 -exec chmod u-s {} + # buildkit
# Wed, 28 Sep 2022 11:42:00 GMT
RUN RUN /bin/sh -c groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana # buildkit
# Wed, 28 Sep 2022 11:42:00 GMT
RUN LABEL org.label-schema.build-date=2022-09-28T11:09:19.930Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=1ceb607762eaafa726c61d6eee5b95359142d4c4 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.4.3 org.opencontainers.image.created=2022-09-28T11:09:19.930Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=1ceb607762eaafa726c61d6eee5b95359142d4c4 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.4.3
# Wed, 28 Sep 2022 11:42:00 GMT
RUN ENTRYPOINT ["/bin/tini" "--"]
# Wed, 28 Sep 2022 11:42:00 GMT
RUN CMD ["/usr/local/bin/kibana-docker"]
# Wed, 28 Sep 2022 11:42:00 GMT
RUN USER kibana
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f6d914fbbd3bf4bbf098daf05624b2176ce3c0f3364caaac200933ee53150d`  
		Last Modified: Thu, 06 Oct 2022 07:49:58 GMT  
		Size: 11.0 MB (11017279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ee8c33d15a408c9bfc241a719c96dcce59776ef4aebc5029e17df9240f5b75`  
		Last Modified: Thu, 06 Oct 2022 07:49:56 GMT  
		Size: 9.1 KB (9096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984aa82f15d4ae32d65fffa5b6bd7bdb0ec9790502cc7643df265043cf114747`  
		Last Modified: Thu, 06 Oct 2022 07:49:54 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3ff86cfc7ecefb4e86891ecc9d0ffa5da7c159a921ebb6dcdd1da8974ca94a`  
		Last Modified: Thu, 06 Oct 2022 07:49:56 GMT  
		Size: 16.5 MB (16460493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2934e9ae4904311a4b8e16f5a2e4ec2a24cf0aa148720ad9abc8bc9e05273d`  
		Last Modified: Thu, 06 Oct 2022 07:49:54 GMT  
		Size: 5.3 KB (5287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0976038ba3c144b0b1ec99ac2eaf985d0dcfa48d8904c9b907f75e15fd1dd3d7`  
		Last Modified: Thu, 06 Oct 2022 07:50:33 GMT  
		Size: 301.0 MB (300969850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a122d2da28f92a3d6ea5a01ba9eada0442814607cff465a97be5f8c55ed3679d`  
		Last Modified: Thu, 06 Oct 2022 07:49:54 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660b1e5e2d8af1f28aa68201e3c4dfaa593695b4dbfdea9b085faff87e174d66`  
		Last Modified: Thu, 06 Oct 2022 07:49:52 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3049ed1ecf1cdd569628b5caca9ac0f450fecfa4601e973f683a7f87e3a68b3`  
		Last Modified: Thu, 06 Oct 2022 07:49:52 GMT  
		Size: 4.4 KB (4380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2c97efe65f1ecd77cfe64e5e887951d494dd0e191e69f21e40f20c6d098942`  
		Last Modified: Thu, 06 Oct 2022 07:49:52 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cab3dc8aba0873462969e9fb3c1abda671b215327bac7376e2205773ef4022`  
		Last Modified: Thu, 06 Oct 2022 07:49:52 GMT  
		Size: 183.4 KB (183396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f077744e177b0e2affa4f1c50ff24ec06934e9763ee848dd4001a6973da19e0`  
		Last Modified: Thu, 06 Oct 2022 07:49:52 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
