<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:7.17.9`](#logstash7179)
-	[`logstash:8.7.0`](#logstash870)

## `logstash:7.17.9`

```console
$ docker pull logstash@sha256:48db6de65f1fde20b0dd0853446c1bedcb11d1213fb5a6332dfa9c692cc3ceb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:7.17.9` - linux; amd64

```console
$ docker pull logstash@sha256:8a747338840cb6e49104a1562f33b570abcef33fc273101069a32b92a3291e9d
```

-	Docker Version: 20.10.22
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **438.8 MB (438827246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44725cae61eec71bd23e8631c176b918c121dcbf305702370270fe65001439ed`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 24 Jan 2023 22:17:31 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Tue, 24 Jan 2023 22:17:32 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Tue, 24 Jan 2023 22:17:55 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.9-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.9 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Tue, 24 Jan 2023 22:17:59 GMT
WORKDIR /usr/share/logstash
# Tue, 24 Jan 2023 22:17:59 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 24 Jan 2023 22:17:59 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 22:17:59 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Tue, 24 Jan 2023 22:17:59 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Tue, 24 Jan 2023 22:17:59 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Tue, 24 Jan 2023 22:18:00 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Tue, 24 Jan 2023 22:18:00 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Tue, 24 Jan 2023 22:18:00 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 24 Jan 2023 22:18:00 GMT
ADD file:ced67dbe23501a3719ed1c54ed9f2f87b1a48ab4ce16e5063914145d7cbed734 in /usr/local/bin/ 
# Tue, 24 Jan 2023 22:18:00 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Tue, 24 Jan 2023 22:18:01 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Tue, 24 Jan 2023 22:18:01 GMT
USER 1000
# Tue, 24 Jan 2023 22:18:01 GMT
EXPOSE 5044 9600
# Tue, 24 Jan 2023 22:18:01 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.9 org.opencontainers.image.version=7.17.9 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-01-24T22:01:46+00:00 org.opencontainers.image.created=2023-01-24T22:01:46+00:00
# Tue, 24 Jan 2023 22:18:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5f7ea055aea7fe08e8f7e798f6dc5bcbfa84121f413243918dc37fe1f90b91`  
		Last Modified: Thu, 02 Feb 2023 23:11:24 GMT  
		Size: 41.4 MB (41362862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fdc4e04fd512db3c86befe51ee955b3732e4b07149a3baf4e774aab2bf465c`  
		Last Modified: Thu, 02 Feb 2023 23:11:08 GMT  
		Size: 1.8 KB (1829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea886dfdca899e749699cec9737455528542fdb68a39ab09146d309b8595499`  
		Last Modified: Thu, 02 Feb 2023 23:12:06 GMT  
		Size: 367.1 MB (367110311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcc18e74b5812fd4f9acce5375f5b5d3e1268f05f9016b78e7bbfe501832cb4`  
		Last Modified: Thu, 02 Feb 2023 23:11:06 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110ad10a595ff40a6e7538ec3c905fdeaa843110d8eca7e57dd34bbda3f72c62`  
		Last Modified: Thu, 02 Feb 2023 23:11:06 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f069a2ebecdd13035537f2a0780a80c9997c1968184f2746019e707a5c3fedf`  
		Last Modified: Thu, 02 Feb 2023 23:11:06 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf535948a5f4e74303a1ad5cba184343f7d6f3f4fe17e3426586996f9a673113`  
		Last Modified: Thu, 02 Feb 2023 23:11:02 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d020f99453e9a58488f38b4269fb7303fcb1b16b2deb67dadd20794fb4306b09`  
		Last Modified: Thu, 02 Feb 2023 23:11:02 GMT  
		Size: 2.9 KB (2851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809919f46c064cc9c4f4623ea15fe3da0daaf0a74e57b862132dbfe2265d40f4`  
		Last Modified: Thu, 02 Feb 2023 23:11:01 GMT  
		Size: 1.8 MB (1770100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e22311e0cf9b2e191427ecaf72446c894dc9811c2d4e31cac919643f072abb`  
		Last Modified: Thu, 02 Feb 2023 23:10:57 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e22311e0cf9b2e191427ecaf72446c894dc9811c2d4e31cac919643f072abb`  
		Last Modified: Thu, 02 Feb 2023 23:10:57 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:7.17.9` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:0a83992e64519b85f040fc94bb20b5f611f707f885dde5c067f92b7185e84660
```

-	Docker Version: 20.10.22
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.5 MB (427451040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b47f1c0ff51367ae955ae7c8f5cd9c77a4f274f019edbf2152bf4c80a8eb3155`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Tue, 24 Jan 2023 22:17:06 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Tue, 24 Jan 2023 22:17:06 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Tue, 24 Jan 2023 22:17:25 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.9-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.9 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Tue, 24 Jan 2023 22:17:28 GMT
WORKDIR /usr/share/logstash
# Tue, 24 Jan 2023 22:17:28 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 24 Jan 2023 22:17:29 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 22:17:29 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Tue, 24 Jan 2023 22:17:29 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Tue, 24 Jan 2023 22:17:29 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Tue, 24 Jan 2023 22:17:29 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Tue, 24 Jan 2023 22:17:30 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Tue, 24 Jan 2023 22:17:30 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 24 Jan 2023 22:17:30 GMT
ADD file:83f91a29fcb81019467f8bd1de10290c5d04ec23b929a6b8eef3fd6e3208404a in /usr/local/bin/ 
# Tue, 24 Jan 2023 22:17:30 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Tue, 24 Jan 2023 22:17:30 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Tue, 24 Jan 2023 22:17:31 GMT
USER 1000
# Tue, 24 Jan 2023 22:17:31 GMT
EXPOSE 5044 9600
# Tue, 24 Jan 2023 22:17:31 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.9 org.opencontainers.image.version=7.17.9 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-01-24T22:04:07+00:00 org.opencontainers.image.created=2023-01-24T22:04:07+00:00
# Tue, 24 Jan 2023 22:17:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdbdc9e3c4ca20d2def637003f01fbfee5e079461c2bf2afa2bae39a951da63`  
		Last Modified: Tue, 07 Feb 2023 22:58:30 GMT  
		Size: 34.7 MB (34728379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d22237706ea632948d69fa74a059182b4f043c3fbef4b821a67cf1c8c47cb2`  
		Last Modified: Tue, 07 Feb 2023 22:58:26 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4838229cd33f201b5395c4cb4a666c2e82d1fc9247f782190e56153a17656dd3`  
		Last Modified: Tue, 07 Feb 2023 22:58:48 GMT  
		Size: 363.9 MB (363873906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce10bfae58270d87e1b2f096e17646aeb92362ce63c8236e6c4d09c57b3a3f39`  
		Last Modified: Tue, 07 Feb 2023 22:58:26 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888ee304434cd86a1dde5858ec54f31e6f2922bdcf33838d78477121bbbac081`  
		Last Modified: Tue, 07 Feb 2023 22:58:26 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d5a146695eb8d6cdbf73af39a22e654ae46be97aa7445ccfa9ac36cccbf8f4`  
		Last Modified: Tue, 07 Feb 2023 22:58:24 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a995c76ab5582895c18ae37084d06eb2bc12f8068f8258f6dc4afd6ecbce93`  
		Last Modified: Tue, 07 Feb 2023 22:58:24 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c44745587e7af9750b7ccffbce7d9dc5e6e437cbf6a1d2845e805425afddc4`  
		Last Modified: Tue, 07 Feb 2023 22:58:24 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd7254666423017892e872df8e289f44326ea905d8d8b212910d2df93d7d4f8`  
		Last Modified: Tue, 07 Feb 2023 22:58:24 GMT  
		Size: 1.6 MB (1648477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7413ffca3e9aa329d54f3c9bf1359ce6171b90791359218ce54e9becda5a1cae`  
		Last Modified: Tue, 07 Feb 2023 22:58:24 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7413ffca3e9aa329d54f3c9bf1359ce6171b90791359218ce54e9becda5a1cae`  
		Last Modified: Tue, 07 Feb 2023 22:58:24 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:8.7.0`

```console
$ docker pull logstash@sha256:199c73c59fc118a9605c49daf0e7f16211b77d47788692a6de4b1d8af7a583f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `logstash:8.7.0` - linux; amd64

```console
$ docker pull logstash@sha256:1ae1be5138b4e6527f5a2f23c8891b393e0773a4b5d57e9937563d5e26b1beef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.9 MB (399854632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ba1fb9c04042cacecf3aa43cd987c30c90ead20330fabc9d346f5ae8324445`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Sun, 26 Mar 2023 04:00:31 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Sun, 26 Mar 2023 04:00:31 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Sun, 26 Mar 2023 04:00:47 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.7.0-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.7.0 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Sun, 26 Mar 2023 04:00:47 GMT
WORKDIR /usr/share/logstash
# Sun, 26 Mar 2023 04:00:47 GMT
ENV ELASTIC_CONTAINER=true
# Sun, 26 Mar 2023 04:00:47 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 26 Mar 2023 04:00:47 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Sun, 26 Mar 2023 04:00:47 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Sun, 26 Mar 2023 04:00:47 GMT
COPY config/log4j2.properties config/ # buildkit
# Sun, 26 Mar 2023 04:00:47 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Sun, 26 Mar 2023 04:00:47 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Sun, 26 Mar 2023 04:00:47 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Sun, 26 Mar 2023 04:00:47 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Sun, 26 Mar 2023 04:00:47 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Sun, 26 Mar 2023 04:00:47 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Sun, 26 Mar 2023 04:00:47 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Sun, 26 Mar 2023 04:00:47 GMT
USER 1000
# Sun, 26 Mar 2023 04:00:47 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Sun, 26 Mar 2023 04:00:47 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.7.0 org.opencontainers.image.version=8.7.0 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-03-26T03:44:05+00:00 org.opencontainers.image.created=2023-03-26T03:44:05+00:00
# Sun, 26 Mar 2023 04:00:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3e74557b41ea71138ba6a5ce95335690081fb279e45d717930865c5fea1eb9`  
		Last Modified: Mon, 03 Apr 2023 08:41:29 GMT  
		Size: 42.0 MB (42019156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0a442d2d68d1280ad2a4db96bcdae884f8a70583702b97fce75b3c14d9a391`  
		Last Modified: Mon, 03 Apr 2023 08:41:17 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4f9acdaf90b1ed7aef43feb246b47e646c8ba43547e0f3d99b4a73b8329068`  
		Last Modified: Mon, 03 Apr 2023 08:41:34 GMT  
		Size: 327.4 MB (327438254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0689e3798b80c7417caca0dac8831ea5846b0e28839dcfc840b8b592dc6cdbcf`  
		Last Modified: Mon, 03 Apr 2023 08:41:15 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a45dd69d17307be08732029692d9610f513a336bf67889bda5b0fcd4bcc5ac`  
		Last Modified: Mon, 03 Apr 2023 08:41:15 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c34cbf0ba0c62b2dab337d5af3af85f48eb2e0402bd8f3126f990209e738a2`  
		Last Modified: Mon, 03 Apr 2023 08:41:15 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d84190a1c371b429edf86df85bba1e6a439e2a65e7955b05b793fad5ab7918`  
		Last Modified: Mon, 03 Apr 2023 08:41:14 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c64a4ea06e3c41ca7b1b4ae3baaa8d61c3415e28501aeebdf8b6bd74e42dff`  
		Last Modified: Mon, 03 Apr 2023 08:41:14 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2916bd753da8e151aecce69ef45c10d241cc210d47a92de345d6a3a9f37195ad`  
		Last Modified: Mon, 03 Apr 2023 08:41:12 GMT  
		Size: 3.7 KB (3659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51257f0e524c9377b2aa8f4f0eecd9a9afb972d4d49d1bc7db590070f742dbd2`  
		Last Modified: Mon, 03 Apr 2023 08:41:13 GMT  
		Size: 1.8 MB (1809442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373b133a6276ca19519faee71acae32cd566402df89911fad2765ccc1f5f505`  
		Last Modified: Mon, 03 Apr 2023 08:41:12 GMT  
		Size: 714.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373b133a6276ca19519faee71acae32cd566402df89911fad2765ccc1f5f505`  
		Last Modified: Mon, 03 Apr 2023 08:41:12 GMT  
		Size: 714.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
