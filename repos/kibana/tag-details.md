<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kibana`

-	[`kibana:6.8.20`](#kibana6820)
-	[`kibana:7.14.2`](#kibana7142)

## `kibana:6.8.20`

**does not exist** (yet?)

## `kibana:7.14.2`

```console
$ docker pull kibana@sha256:d3eaf39c5aae353a9edae380030188ed712547a31954c8057d069ef8f2d8cbba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kibana:7.14.2` - linux; amd64

```console
$ docker pull kibana@sha256:fb12b4b85381ed5286cb8b78552b18f5fe8d562f9e21ab67db580f972ce8d3be
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **479.9 MB (479917367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:750d302f8aff79b4c978e7d75aebc69b906306ee9f606b0b715662fd6dd88c10`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Tue, 08 Dec 2020 00:22:52 GMT
ADD file:bd7a2aed6ede423b719ceb2f723e4ecdfa662b28639c8429731c878e86fb138b in / 
# Tue, 08 Dec 2020 00:22:52 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Tue, 08 Dec 2020 00:22:53 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 10:03:46 GMT
EXPOSE 5601
# Wed, 15 Sep 2021 10:05:19 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y         fontconfig freetype shadow-utils nss  &&       yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Wed, 15 Sep 2021 10:05:22 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Wed, 15 Sep 2021 10:05:23 GMT
RUN mkdir /usr/share/fonts/local
# Wed, 15 Sep 2021 10:05:24 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Wed, 15 Sep 2021 10:05:24 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Wed, 15 Sep 2021 10:05:25 GMT
RUN fc-cache -v
# Wed, 15 Sep 2021 10:05:53 GMT
COPY --chown=1000:0dir:5f6b8d9ab50c94c1869550679c94f21c8d86cca4431d24cbe02799273bc85d71 in /usr/share/kibana 
# Wed, 15 Sep 2021 10:06:03 GMT
WORKDIR /usr/share/kibana
# Wed, 15 Sep 2021 10:06:04 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Wed, 15 Sep 2021 10:06:04 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 15 Sep 2021 10:06:04 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Sep 2021 10:06:04 GMT
COPY --chown=1000:0file:ab38106de0b2164e20c73bb3449b4682fb9c654eac5b38ed7f560f16ed9c9105 in /usr/share/kibana/config/kibana.yml 
# Wed, 15 Sep 2021 10:06:04 GMT
COPY --chown=1000:0file:b0123e8ae9fc4209bee508fdcf33ab86f8cb2b84bfc9b53695ed8289f423a7aa in /usr/local/bin/ 
# Wed, 15 Sep 2021 10:06:06 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Wed, 15 Sep 2021 10:06:07 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Wed, 15 Sep 2021 10:06:08 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Wed, 15 Sep 2021 10:06:08 GMT
LABEL org.label-schema.build-date=2021-09-15T09:14:27.489Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=6b971d6410ca4a99271f2abf9d3de68b7a3653a5 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.14.2 org.opencontainers.image.created=2021-09-15T09:14:27.489Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=6b971d6410ca4a99271f2abf9d3de68b7a3653a5 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.14.2
# Wed, 15 Sep 2021 10:06:08 GMT
USER kibana
# Wed, 15 Sep 2021 10:06:08 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Wed, 15 Sep 2021 10:06:08 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:7a0437f04f83f084b7ed68ad9c4a4947e12fc4e1b006b38129bac89114ec3621`  
		Last Modified: Tue, 08 Dec 2020 00:23:32 GMT  
		Size: 75.2 MB (75181999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5efb728eeac098e47f2290fbf364efed7651356035295779eadec44a077cd37`  
		Last Modified: Tue, 21 Sep 2021 18:25:57 GMT  
		Size: 97.1 MB (97125071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205af3f4fe7e8d370fbf55aca6686e58528290e6dd3543913a7df5ee28a69546`  
		Last Modified: Tue, 21 Sep 2021 18:25:33 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b675a316464b37c89c0dbe369d201c67d7149b4dac1fe668e94c2dc3d87a60`  
		Last Modified: Tue, 21 Sep 2021 18:25:30 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9599c0ecc7001507ea45f250b05aa50dff6901f9c5fb476d6a0684d1f141d1e`  
		Last Modified: Tue, 21 Sep 2021 18:25:32 GMT  
		Size: 16.5 MB (16460487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d629d594e22b1534f85314cf86e854a81cd4a6de1e3146812d045ff5dc61f7`  
		Last Modified: Tue, 21 Sep 2021 18:25:29 GMT  
		Size: 8.3 KB (8313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198b71084307cda3058c7de61b03de8ec2dce488e29ad8dc5ea86c7c8e1a89d1`  
		Last Modified: Tue, 21 Sep 2021 18:26:31 GMT  
		Size: 290.9 MB (290927787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc660aca6b34a871f4091564a1e7f1d427c717d1b5cd0a87389b2bb34cf3a63f`  
		Last Modified: Tue, 21 Sep 2021 18:25:29 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8e735b24f23ebabc321eb6c9d84134e91c7bd88f22071fb5817bf8be374333`  
		Last Modified: Tue, 21 Sep 2021 18:25:26 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce943f752a9416951310822c18f029a446b09a9f5f24410789b4f3ae286666dc`  
		Last Modified: Tue, 21 Sep 2021 18:25:26 GMT  
		Size: 4.5 KB (4450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454ce91b9a9c7983e16a94af0051d23f931b72005f3c97a0489d5b4f2a1aab0e`  
		Last Modified: Tue, 21 Sep 2021 18:25:26 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d828deac6d84c1df7c8af03127a20e21d81b69afdb014ae9610396bb55860ffd`  
		Last Modified: Tue, 21 Sep 2021 18:25:27 GMT  
		Size: 196.7 KB (196724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251fb998452901ab47697a2bfccaed5254c33c8cc212c12f0036ac43c215ac45`  
		Last Modified: Tue, 21 Sep 2021 18:25:26 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kibana:7.14.2` - linux; arm64 variant v8

```console
$ docker pull kibana@sha256:df93c52a1a69b0a9669568e55904838899c3529cf97a1bfe2f31fd6958b2835f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **494.7 MB (494698344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d009537c70323b68e77263e852e66998acb3a8a308d6c3443abf560dac53373`
-	Entrypoint: `["\/bin\/tini","--"]`
-	Default Command: `["\/usr\/local\/bin\/kibana-docker"]`

```dockerfile
# Mon, 07 Dec 2020 23:42:06 GMT
ADD file:edd6e1253ec7bbb67b5a28d40c7d28b34a443c2cfa327bebf55c8b0b19484bf9 in / 
# Mon, 07 Dec 2020 23:42:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201204
# Mon, 07 Dec 2020 23:42:10 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 11:27:34 GMT
EXPOSE 5601
# Wed, 15 Sep 2021 11:28:27 GMT
RUN for iter in {1..10}; do       yum update --setopt=tsflags=nodocs -y &&       yum install --setopt=tsflags=nodocs -y         fontconfig freetype shadow-utils nss  &&       yum clean all && exit_code=0 && break || exit_code=$? && echo "yum error: retry $iter in 10s" &&       sleep 10;     done;     (exit $exit_code)
# Wed, 15 Sep 2021 11:28:30 GMT
RUN set -e ;     TINI_BIN="" ;     case "$(arch)" in         aarch64)             TINI_BIN='tini-arm64' ;             ;;         x86_64)             TINI_BIN='tini-amd64' ;             ;;         *) echo >&2 "Unsupported architecture $(arch)" ; exit 1 ;;     esac ;   TINI_VERSION='v0.19.0' ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}" ;   curl --retry 8 -S -L -O "https://github.com/krallin/tini/releases/download/${TINI_VERSION}/${TINI_BIN}.sha256sum" ;   sha256sum -c "${TINI_BIN}.sha256sum" ;   rm "${TINI_BIN}.sha256sum" ;   mv "${TINI_BIN}" /bin/tini ;   chmod +x /bin/tini
# Wed, 15 Sep 2021 11:28:30 GMT
RUN mkdir /usr/share/fonts/local
# Wed, 15 Sep 2021 11:28:32 GMT
RUN curl -L -o /usr/share/fonts/local/NotoSansCJK-Regular.ttc https://github.com/googlefonts/noto-cjk/raw/NotoSansV2.001/NotoSansCJK-Regular.ttc
# Wed, 15 Sep 2021 11:28:33 GMT
RUN echo "5dcd1c336cc9344cb77c03a0cd8982ca8a7dc97d620fd6c9c434e02dcb1ceeb3  /usr/share/fonts/local/NotoSansCJK-Regular.ttc" | sha256sum -c -
# Wed, 15 Sep 2021 11:28:33 GMT
RUN fc-cache -v
# Wed, 15 Sep 2021 11:29:38 GMT
COPY --chown=1000:0dir:be0625ffa331f34da20eed08950ef87b35e468e0451a986a0cb81b69a774e2e9 in /usr/share/kibana 
# Wed, 15 Sep 2021 11:29:40 GMT
WORKDIR /usr/share/kibana
# Wed, 15 Sep 2021 11:29:41 GMT
RUN ln -s /usr/share/kibana /opt/kibana
# Wed, 15 Sep 2021 11:29:41 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 15 Sep 2021 11:29:41 GMT
ENV PATH=/usr/share/kibana/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 15 Sep 2021 11:29:41 GMT
COPY --chown=1000:0file:ab38106de0b2164e20c73bb3449b4682fb9c654eac5b38ed7f560f16ed9c9105 in /usr/share/kibana/config/kibana.yml 
# Wed, 15 Sep 2021 11:29:41 GMT
COPY --chown=1000:0file:b0123e8ae9fc4209bee508fdcf33ab86f8cb2b84bfc9b53695ed8289f423a7aa in /usr/local/bin/ 
# Wed, 15 Sep 2021 11:29:42 GMT
RUN chmod g+ws /usr/share/kibana &&     find /usr/share/kibana -gid 0 -and -not -perm /g+w -exec chmod g+w {} \;
# Wed, 15 Sep 2021 11:29:45 GMT
RUN find / -xdev -perm -4000 -exec chmod u-s {} +
# Wed, 15 Sep 2021 11:29:45 GMT
RUN groupadd --gid 1000 kibana &&     useradd --uid 1000 --gid 1000 -G 0       --home-dir /usr/share/kibana --no-create-home       kibana
# Wed, 15 Sep 2021 11:29:45 GMT
LABEL org.label-schema.build-date=2021-09-15T11:24:32.280Z org.label-schema.license=Elastic License org.label-schema.name=Kibana org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/kibana org.label-schema.usage=https://www.elastic.co/guide/en/kibana/reference/index.html org.label-schema.vcs-ref=6b971d6410ca4a99271f2abf9d3de68b7a3653a5 org.label-schema.vcs-url=https://github.com/elastic/kibana org.label-schema.vendor=Elastic org.label-schema.version=7.14.2 org.opencontainers.image.created=2021-09-15T11:24:32.280Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/kibana/reference/index.html org.opencontainers.image.licenses=Elastic License org.opencontainers.image.revision=6b971d6410ca4a99271f2abf9d3de68b7a3653a5 org.opencontainers.image.source=https://github.com/elastic/kibana org.opencontainers.image.title=Kibana org.opencontainers.image.url=https://www.elastic.co/products/kibana org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.14.2
# Wed, 15 Sep 2021 11:29:45 GMT
USER kibana
# Wed, 15 Sep 2021 11:29:46 GMT
ENTRYPOINT ["/bin/tini" "--"]
# Wed, 15 Sep 2021 11:29:46 GMT
CMD ["/usr/local/bin/kibana-docker"]
```

-	Layers:
	-	`sha256:333cbcae3fb80b9a46084ae4caea81a84aafda9700fb646ab89206d0cfe213fd`  
		Last Modified: Mon, 07 Dec 2020 23:42:49 GMT  
		Size: 75.6 MB (75613064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e453fd7ae3a1693bb26b51abaf02c3ce72287115d5945e887974f9bcab3b5d1`  
		Last Modified: Fri, 15 Oct 2021 18:44:22 GMT  
		Size: 97.1 MB (97092623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2488a2de20761b29df803fc27b5705a9db439e702a65e114a4a13dd8456252`  
		Last Modified: Fri, 15 Oct 2021 18:44:07 GMT  
		Size: 9.1 KB (9103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80265f15b7a47a107482cc849d1e4976520c527e7b318f396c286c2d90b018f8`  
		Last Modified: Fri, 15 Oct 2021 18:44:05 GMT  
		Size: 193.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd8b71e01d273fb0c1f0faa801c4f588b6452c559473038386fbcd8ede7a837`  
		Last Modified: Fri, 15 Oct 2021 18:44:06 GMT  
		Size: 16.5 MB (16460485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298b7da4371b7c47665788b29772296c7f9de991c64ca075a8234fc435efd511`  
		Last Modified: Fri, 15 Oct 2021 18:44:05 GMT  
		Size: 8.3 KB (8274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb8c50dc701831cdfd1abb5b5d5fa729e017bcfa28139dc732e480b532f45fb`  
		Last Modified: Fri, 15 Oct 2021 18:44:46 GMT  
		Size: 305.3 MB (305309923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40493d5585a99b37702337f81821b504fed076760c1f65b2a73b38e4cc1d8b3`  
		Last Modified: Fri, 15 Oct 2021 18:44:05 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734c26f887f9477f2a37e49dda2171ab9d212d87664a93f2eeab30fe8cd4f7cf`  
		Last Modified: Fri, 15 Oct 2021 18:44:02 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a880e973d87367bb6517b0477956a57a547449b37d06cc7f4062faea1b489db`  
		Last Modified: Fri, 15 Oct 2021 18:44:02 GMT  
		Size: 4.5 KB (4452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7547535cfb24aae0a9de6cba54c4040eda4f248b7ddec394d557417a066a8970`  
		Last Modified: Fri, 15 Oct 2021 18:44:02 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9600f583bed0d6b7294059c0962f762ee3dad9c55deeea6138badb3453643d86`  
		Last Modified: Fri, 15 Oct 2021 18:44:02 GMT  
		Size: 197.4 KB (197412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014e9c4a647cf6e1a5cf87830802b22d980566477e1c84aa457bc19bd79c6bdc`  
		Last Modified: Fri, 15 Oct 2021 18:44:02 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
