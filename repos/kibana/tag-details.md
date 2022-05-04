<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.23`](#kibana6823)
-	[`kibana:7.17.3`](#kibana7173)
-	[`kibana:8.2.0`](#kibana820)

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

## `kibana:7.17.3`

```console
$ docker pull kibana@sha256:e2e2031c15be40af4369fe04db4d91d65976b39c06f70447d878a1d44b9915be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.17.3` - linux; amd64

```console
$ docker pull kibana@sha256:2bea450207ac0574ea7b3cc4318c260100ed7722043c9e05cf857a2ff6e56050
```

-	Docker Version: 20.10.14
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.9 MB (324937357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4897f4b8b6ee94dc47ac4dc1274419806d370ea5351204caacc711fd24843b18`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:50 GMT
ADD file:b83df51ab7caf8a4dc35f730f5a18a59403300c59eecae4cf5779cba0f6fda6e in / 
# Tue, 05 Apr 2022 22:20:51 GMT
CMD ["bash"]
# Tue, 19 Apr 2022 09:09:34 GMT
EXPOSE 5601
# Tue, 19 Apr 2022 09:09:52 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Tue, 19 Apr 2022 09:09:53 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Tue, 19 Apr 2022 09:09:53 GMT
RUN mkdir /usr/share/fonts/local
# Tue, 19 Apr 2022 09:09:54 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Tue, 19 Apr 2022 09:09:55 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Tue, 19 Apr 2022 09:09:56 GMT
RUN fc-cache -v
# Tue, 19 Apr 2022 09:10:18 GMT
COPY --chown=1000:0dir:7e38b46db342337f732630ffefe1e08787c4a0d81898f5d9b6ea4631e27926f2 in /usr/share/kibana 
# Tue, 19 Apr 2022 09:10:26 GMT
WORKDIR /usr/share/kibana
# Tue, 19 Apr 2022 09:10:26 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Tue, 19 Apr 2022 09:10:26 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 19 Apr 2022 09:10:26 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Apr 2022 09:10:27 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Tue, 19 Apr 2022 09:10:27 GMT
COPY file:64ce3ba9275bed6c9214b200cd3b7913d52068df7094bee2baccc5b713d391f7 in /usr/local/bin/ 
# Tue, 19 Apr 2022 09:10:28 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Tue, 19 Apr 2022 09:10:29 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Tue, 19 Apr 2022 09:10:30 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Tue, 19 Apr 2022 09:10:30 GMT
LABEL org.label-schema.build-date=2022-04-19T08:22:01.788Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=dcd0a101ed880bb10a4dcf511b91fd611d8c805d org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.3 org.opencontainers.image.created=2022-04-19T08:22:01.788Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=dcd0a101ed880bb10a4dcf511b91fd611d8c805d org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.3
# Tue, 19 Apr 2022 09:10:30 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Tue, 19 Apr 2022 09:10:30 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Tue, 19 Apr 2022 09:10:30 GMT
USER kibana
```

-	Layers:
	-	`sha256:e0b25ef516347a097d75f8aea6bc0f42a4e8e70b057e84d85098d51f96d458f9`  
		Last Modified: Tue, 05 Apr 2022 13:14:03 GMT  
		Size: 28.6 MB (28566292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9440443b08eec92ff612b85f90f6a222d0f51f1638a616df0c5fd66fdfa09d21`  
		Last Modified: Thu, 21 Apr 2022 21:47:42 GMT  
		Size: 11.1 MB (11104556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e97b0672be8f3883010e630253121cd69d6610e32275a17a3ee52845741a3`  
		Last Modified: Thu, 21 Apr 2022 21:47:40 GMT  
		Size: 9.5 KB (9526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aee45d3a5070a0a89d68d564d536015f2fd51e4d15976ee7bcb55269c28935b`  
		Last Modified: Thu, 21 Apr 2022 21:47:38 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9cd1a53684f0b291e74c318294c37f556b4c29b1f577f9c49368186464d86a`  
		Last Modified: Thu, 21 Apr 2022 21:47:39 GMT  
		Size: 16.5 MB (16460475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c3a32db2527717d18fdaec8cc4626c056bfd4aa985fbe00ec4ad66ad6b2359`  
		Last Modified: Thu, 21 Apr 2022 21:47:38 GMT  
		Size: 5.3 KB (5275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b931a580503e92f559a067657b0e1e5aa2fd87a5e5149ec45c485c0b2c14e92`  
		Last Modified: Thu, 21 Apr 2022 21:48:09 GMT  
		Size: 268.6 MB (268594419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5b3379fce708dba1be025f32353fbaf36185302cf1cb4ffdafd2ebc40ddd91`  
		Last Modified: Thu, 21 Apr 2022 21:47:38 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a844e9e78246da9700954e79aed2446d778a64b2a50cfacc5b0c5fa687141c`  
		Last Modified: Thu, 21 Apr 2022 21:47:35 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5c92edaabe39726c4ec16c21c4e6c9790f054e8e8c2270f1a210ec0bca6420`  
		Last Modified: Thu, 21 Apr 2022 21:47:35 GMT  
		Size: 4.5 KB (4498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b5eef01620ff76f54606aa6baf4d03c44085cf5ec4f532db3d5c4bf75b17dd`  
		Last Modified: Thu, 21 Apr 2022 21:47:35 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80b734e506d28d51f8b6e515cef6a6eb5ab1ca537de9c5791a28e79621d793b`  
		Last Modified: Thu, 21 Apr 2022 21:47:35 GMT  
		Size: 189.4 KB (189380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df86baf43ead418a0f9d4c82ce16e9663493178c2c9f4ed14892f41874a41e4`  
		Last Modified: Thu, 21 Apr 2022 21:47:35 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.17.3` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:38cd91104b951c3e5c1779450c33026b2887fca37599cdc34ed178f2616196f6
```

-	Docker Version: 20.10.14
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.0 MB (338005045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:107620ecfd4d083efd1dee52e9f710a2a4aed45a167b266d0663e4a3f4ec1f09`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 05 Apr 2022 22:40:59 GMT
ADD file:113ba5e7bc74d50e8d35449f8a62712359e2f00146e03eee822c28c8c6f59368 in / 
# Tue, 05 Apr 2022 22:41:00 GMT
CMD ["bash"]
# Tue, 19 Apr 2022 10:29:07 GMT
EXPOSE 5601
# Tue, 19 Apr 2022 10:29:26 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Tue, 19 Apr 2022 10:29:27 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Tue, 19 Apr 2022 10:29:27 GMT
RUN mkdir /usr/share/fonts/local
# Tue, 19 Apr 2022 10:29:29 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Tue, 19 Apr 2022 10:29:30 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Tue, 19 Apr 2022 10:29:31 GMT
RUN fc-cache -v
# Tue, 19 Apr 2022 10:29:51 GMT
COPY --chown=1000:0dir:5db978ad9b6fdd684cfbe022c45182dab754221d68507b7317eeb8a54c82a678 in /usr/share/kibana 
# Tue, 19 Apr 2022 10:29:53 GMT
WORKDIR /usr/share/kibana
# Tue, 19 Apr 2022 10:29:53 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Tue, 19 Apr 2022 10:29:53 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 19 Apr 2022 10:29:53 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Apr 2022 10:29:53 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Tue, 19 Apr 2022 10:29:54 GMT
COPY file:64ce3ba9275bed6c9214b200cd3b7913d52068df7094bee2baccc5b713d391f7 in /usr/local/bin/ 
# Tue, 19 Apr 2022 10:29:55 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Tue, 19 Apr 2022 10:29:56 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Tue, 19 Apr 2022 10:29:56 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Tue, 19 Apr 2022 10:29:56 GMT
LABEL org.label-schema.build-date=2022-04-19T10:26:25.756Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=dcd0a101ed880bb10a4dcf511b91fd611d8c805d org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.17.3 org.opencontainers.image.created=2022-04-19T10:26:25.756Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=dcd0a101ed880bb10a4dcf511b91fd611d8c805d org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.3
# Tue, 19 Apr 2022 10:29:56 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Tue, 19 Apr 2022 10:29:57 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Tue, 19 Apr 2022 10:29:57 GMT
USER kibana
```

-	Layers:
	-	`sha256:185e8a4c100571f111d924b5d4399d89f163bf95d71ce2c6a33f656a66c52f0a`  
		Last Modified: Tue, 05 Apr 2022 13:15:01 GMT  
		Size: 27.2 MB (27169393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e16bacd88a10988a4a0cb93ed2f3cd4dc776f2943ce158e9e091a2df11ed5ae`  
		Last Modified: Thu, 21 Apr 2022 22:19:17 GMT  
		Size: 11.0 MB (10969949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd6dc9bd2a8ed83a9ac217cbf688d00c2babb7097b8cd485528cb0deef7a826`  
		Last Modified: Thu, 21 Apr 2022 22:19:15 GMT  
		Size: 9.1 KB (9098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c01244521bb2ec26931483e61b0f546aaff6c6277c23f6b521572c13a88496`  
		Last Modified: Thu, 21 Apr 2022 22:19:13 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896dc47fc272276a441f2f11126aff06fddd2b8c35534bd330294dccae0aa463`  
		Last Modified: Thu, 21 Apr 2022 22:19:14 GMT  
		Size: 16.5 MB (16460491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5e2591959765c61e09bef85e27ec53df6a63e5111e6ec947c0492f51b0a098`  
		Last Modified: Thu, 21 Apr 2022 22:19:12 GMT  
		Size: 5.3 KB (5282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603d027a88b3b53c6376f431455a38eff6d32350e48f35fe15346871c4f27c20`  
		Last Modified: Thu, 21 Apr 2022 22:19:49 GMT  
		Size: 283.2 MB (283200007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9499396d0882ef0989fedf6fe2889cb9881416181f09cc2853594b0c6264804`  
		Last Modified: Thu, 21 Apr 2022 22:19:13 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282dc7c433c299c1011d19cdfee2fd3c2d39958d1d74cd5d9349d02449da7834`  
		Last Modified: Thu, 21 Apr 2022 22:19:10 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed993b04a4bba4be1e65e8ada578d2d91a9d981d12696b90edc9f9368b3ee8c9`  
		Last Modified: Thu, 21 Apr 2022 22:19:10 GMT  
		Size: 4.5 KB (4495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1433df36de1311b37bcb6da1217bfaff61e03c2a19e98c718b04b670808e4037`  
		Last Modified: Thu, 21 Apr 2022 22:19:10 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eff7ca77e718cde9ee30106981fff4f2cb299f97457081230bcf5196b5b0f6`  
		Last Modified: Thu, 21 Apr 2022 22:19:10 GMT  
		Size: 183.4 KB (183388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ac9ce69ccf7c5e91281b102028eea2d667ef0146da56b22d48896184c5b357`  
		Last Modified: Thu, 21 Apr 2022 22:19:10 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kibana:8.2.0`

```console
$ docker pull kibana@sha256:f772170b5b42e2897e86425de4591486e4b0f940001e4be63dc9f250fa3ce19c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `kibana:8.2.0` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:8697e888198b1f566ed893beb668fd8da9e3ffc22d1f2e39648ed5f2c4b2d113
```

-	Docker Version: 20.10.14
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.7 MB (329740016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25a77103b5a5018742aa68a7d460cff60add175d4a5e226422463e604f2c456e`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 05 Apr 2022 22:40:59 GMT
ADD file:113ba5e7bc74d50e8d35449f8a62712359e2f00146e03eee822c28c8c6f59368 in / 
# Tue, 05 Apr 2022 22:41:00 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:49:34 GMT
EXPOSE 5601
# Wed, 20 Apr 2022 13:49:52 GMT
RUN for iter in {1..10}; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update  &&       apt-get upgrade -y  &&       apt-get install -y --no-install-recommends        fontconfig fonts-liberation libnss3 libfontconfig1 ca-certificates curl &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* && exit_code=0 && break || exit_code=$? && echo "apt-get error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Wed, 20 Apr 2022 13:49:54 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Wed, 20 Apr 2022 13:49:54 GMT
RUN mkdir /usr/share/fonts/local
# Wed, 20 Apr 2022 13:49:56 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Wed, 20 Apr 2022 13:49:57 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Wed, 20 Apr 2022 13:49:57 GMT
RUN fc-cache -v
# Wed, 20 Apr 2022 13:50:18 GMT
COPY --chown=1000:0dir:595e9dfaa24b56f7c0cf9abcf9dc661cdb5c86f44a85156c173d3946869b7d27 in /usr/share/kibana 
# Wed, 20 Apr 2022 13:50:20 GMT
WORKDIR /usr/share/kibana
# Wed, 20 Apr 2022 13:50:20 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Wed, 20 Apr 2022 13:50:20 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 20 Apr 2022 13:50:21 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 13:50:21 GMT
COPY --chown=1000:0file:6db5413736a28ead04731f52a5ef1acaa8f3ca1c1d2eaf6bb2b80d8f232794a2 in /usr/share/kibana/config/kibana.yml 
# Wed, 20 Apr 2022 13:50:21 GMT
COPY file:4c812d22025ebeffc4e88b8a90cb0d82f6a1927b5a276613da7b94cf1abddbed in /usr/local/bin/ 
# Wed, 20 Apr 2022 13:50:22 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Wed, 20 Apr 2022 13:50:23 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Wed, 20 Apr 2022 13:50:24 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Wed, 20 Apr 2022 13:50:24 GMT
LABEL org.label-schema.build-date=2022-04-20T13:46:22.099Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=9a5003d8cf0062bf24ef64d6712b44823888cc03 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=8.2.0 org.opencontainers.image.created=2022-04-20T13:46:22.099Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=9a5003d8cf0062bf24ef64d6712b44823888cc03 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.2.0
# Wed, 20 Apr 2022 13:50:24 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Wed, 20 Apr 2022 13:50:24 GMT
CMD ["/usr/local/bin/kibana-docker"]
# Wed, 20 Apr 2022 13:50:24 GMT
USER kibana
```

-	Layers:
	-	`sha256:185e8a4c100571f111d924b5d4399d89f163bf95d71ce2c6a33f656a66c52f0a`  
		Last Modified: Tue, 05 Apr 2022 13:15:01 GMT  
		Size: 27.2 MB (27169393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ba2f33d9b6f485c70d567d3783c3c891385c8e78a3252a57723f7a3366ee3d`  
		Last Modified: Wed, 04 May 2022 21:46:10 GMT  
		Size: 11.6 MB (11570885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee54424e5d5cd912734f1817aa41a0b6002e9e01bca5bbea86af47b916daa78`  
		Last Modified: Wed, 04 May 2022 21:46:08 GMT  
		Size: 9.1 KB (9097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bc6c0e01ffe0ff32a5d01dd24b670bd95123a5ccd0a54191c0713275166a16`  
		Last Modified: Wed, 04 May 2022 21:46:06 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9ec7923140859bd3ddf80c64dc18694edf54c75a8bed41929bb203c20d25ca`  
		Last Modified: Wed, 04 May 2022 21:46:08 GMT  
		Size: 16.5 MB (16460488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ddb7c3f065160ab2e48229cd52daf5c7da95c1adbd31970ff50c2e4fe2e6df`  
		Last Modified: Wed, 04 May 2022 21:46:06 GMT  
		Size: 5.3 KB (5284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f5daa852bc341be683a02ee59630fba49d418062da3ee31d6b6cf9c5c226c8`  
		Last Modified: Wed, 04 May 2022 21:46:41 GMT  
		Size: 274.3 MB (274334233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa000faecfbf35320c99c25172eff6a4790f29b98f6c06891f83f769bcc7124a`  
		Last Modified: Wed, 04 May 2022 21:46:06 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51712893b9ba296a36a8b33b8248a184b8247fd790ba74029467819415b1428c`  
		Last Modified: Wed, 04 May 2022 21:46:03 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a1c5dc7de9a4c10946a6043b6cf18edb2b6ad943495e757db7db5e155d8388`  
		Last Modified: Wed, 04 May 2022 21:46:03 GMT  
		Size: 4.3 KB (4301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb65cedff3a279b86d14b119b691b21ecf07df6e091285f9d95e06116ded6aee`  
		Last Modified: Wed, 04 May 2022 21:46:03 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502ea37338827fdf7dee675ae52710025611cd8421b44c689773db0b1e11a796`  
		Last Modified: Wed, 04 May 2022 21:46:03 GMT  
		Size: 183.4 KB (183388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0724e1de06c2cd4d74cc55a6985cffdb26e746c7aeae700931457db681aab1`  
		Last Modified: Wed, 04 May 2022 21:46:03 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
