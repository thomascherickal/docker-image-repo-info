<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:7.17.11`](#logstash71711)
-	[`logstash:7.17.12`](#logstash71712)
-	[`logstash:8.8.2`](#logstash882)
-	[`logstash:8.9.0`](#logstash890)
-	[`logstash:8.9.1`](#logstash891)

## `logstash:7.17.11`

```console
$ docker pull logstash@sha256:2f9f491331c11d9622c8a3cbae3c1318a0fe33e7a14a63ed5856ab983d846d00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:7.17.11` - linux; amd64

```console
$ docker pull logstash@sha256:d7bab72c50d802e66f2e79b8a5b8a86a38c9b571a72859dd10565f2807223f6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.1 MB (444123621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f42202f569f8d52197f77af1836124769a1b51049155bf853dd8f856e6bf95a0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Wed, 21 Jun 2023 14:02:22 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Wed, 21 Jun 2023 14:02:22 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Wed, 21 Jun 2023 14:02:39 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.11-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.11 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Wed, 21 Jun 2023 14:02:39 GMT
WORKDIR /usr/share/logstash
# Wed, 21 Jun 2023 14:02:39 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 21 Jun 2023 14:02:39 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Jun 2023 14:02:39 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Wed, 21 Jun 2023 14:02:39 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Wed, 21 Jun 2023 14:02:40 GMT
ADD config/log4j2.properties config/ # buildkit
# Wed, 21 Jun 2023 14:02:40 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Wed, 21 Jun 2023 14:02:40 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Wed, 21 Jun 2023 14:02:40 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 21 Jun 2023 14:02:40 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Wed, 21 Jun 2023 14:02:40 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Wed, 21 Jun 2023 14:02:40 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Wed, 21 Jun 2023 14:02:40 GMT
USER 1000
# Wed, 21 Jun 2023 14:02:40 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Wed, 21 Jun 2023 14:02:40 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.11 org.opencontainers.image.version=7.17.11 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-06-21T13:45:54+00:00 org.opencontainers.image.created=2023-06-21T13:45:54+00:00
# Wed, 21 Jun 2023 14:02:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb69c4adc8bff1a501c212d96af6debe52988fb1c2af2d09996f63e32ef6fe5`  
		Last Modified: Tue, 29 Aug 2023 00:29:04 GMT  
		Size: 46.5 MB (46460870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fd06b20a4c9252392a8184527187e1537f1430f17178c94e9fce0ec408762`  
		Last Modified: Tue, 29 Aug 2023 00:28:59 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3c57d52dd5b6d020d63822cdfeca4163912cd778b9a9fbe773df7a3462e33f`  
		Last Modified: Tue, 29 Aug 2023 00:29:24 GMT  
		Size: 367.3 MB (367263081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8339ca9db139efd19922a28eb34b003472fcc356665311dd39f34e1acaa65bc`  
		Last Modified: Tue, 29 Aug 2023 00:28:58 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49489b26aac536b4c94a32050322125cf32a2098679e4433ddf9472a83f0d977`  
		Last Modified: Tue, 29 Aug 2023 00:28:58 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5f1ebe89e9e3ccc5b380d1ebbcb74fc5bb836ca44e89948a56e78dfd948ecd`  
		Last Modified: Tue, 29 Aug 2023 00:28:56 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588f61b436a2dd946fb57754581d011936112e5c2e82794119cda10418ba3d57`  
		Last Modified: Tue, 29 Aug 2023 00:28:56 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4921431ca2bedc2d5eae72a7d3cdf22ed1c1af23ae74cb4a251610750657f99d`  
		Last Modified: Tue, 29 Aug 2023 00:28:56 GMT  
		Size: 2.9 KB (2865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79911c60069df1d3e7a4aa4a27e234914afdd9c76a127895f768f65f32030391`  
		Last Modified: Tue, 29 Aug 2023 00:28:56 GMT  
		Size: 1.8 MB (1812019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39aacd4ae86c5d43aa6d772fbc6f173307e9c84a9d941db576c3c3e3afb759b`  
		Last Modified: Tue, 29 Aug 2023 00:28:56 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39aacd4ae86c5d43aa6d772fbc6f173307e9c84a9d941db576c3c3e3afb759b`  
		Last Modified: Tue, 29 Aug 2023 00:28:56 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:7.17.11` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:6a61c6e232a64e755bc04eea9056c18568a0835673ba59e5f62fcce5e75f98d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **431.4 MB (431440834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73e695dbacd12b79f0af6f12327ee099e9531d573102ad52dc677482bac34487`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Wed, 21 Jun 2023 13:59:51 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Wed, 21 Jun 2023 13:59:51 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Wed, 21 Jun 2023 14:00:02 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.11-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.11 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Wed, 21 Jun 2023 14:00:02 GMT
WORKDIR /usr/share/logstash
# Wed, 21 Jun 2023 14:00:02 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 21 Jun 2023 14:00:02 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Jun 2023 14:00:02 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Wed, 21 Jun 2023 14:00:02 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Wed, 21 Jun 2023 14:00:02 GMT
ADD config/log4j2.properties config/ # buildkit
# Wed, 21 Jun 2023 14:00:02 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Wed, 21 Jun 2023 14:00:02 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Wed, 21 Jun 2023 14:00:02 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 21 Jun 2023 14:00:02 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Wed, 21 Jun 2023 14:00:02 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Wed, 21 Jun 2023 14:00:03 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Wed, 21 Jun 2023 14:00:03 GMT
USER 1000
# Wed, 21 Jun 2023 14:00:03 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Wed, 21 Jun 2023 14:00:03 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.11 org.opencontainers.image.version=7.17.11 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-06-21T13:47:17+00:00 org.opencontainers.image.created=2023-06-21T13:47:17+00:00
# Wed, 21 Jun 2023 14:00:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d6a3f86248d7c9fddf83b7d69d47af42f1f268d6705f39f19fb4ae1608603d`  
		Last Modified: Mon, 28 Aug 2023 23:47:00 GMT  
		Size: 38.5 MB (38504893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e9e518f37bf12e36e489f981d4766632b9c5322cc34d72bf78ecac977f4b20`  
		Last Modified: Mon, 28 Aug 2023 23:46:56 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287f0786ef7366c9582f172f3964c8918c03ac5338dd3971df069d4fad777990`  
		Last Modified: Mon, 28 Aug 2023 23:47:17 GMT  
		Size: 364.0 MB (364035896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12258c9cf443c21e5543f0bf43bf7f12553e836a317063a5c86763bef5ca14fb`  
		Last Modified: Mon, 28 Aug 2023 23:46:56 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651b4d1b813d7e56e4e3263d32d1884ddf460651de2d814539d188af234662d6`  
		Last Modified: Mon, 28 Aug 2023 23:46:56 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e451c000262b737ed0047c4bbd9f1d8394a84f73cb1d25ccf22356840e07a`  
		Last Modified: Mon, 28 Aug 2023 23:46:54 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9c7194f23f083de5f6403e8a3d47db6b0acc676ac92f3e56ec833c51f2d718`  
		Last Modified: Mon, 28 Aug 2023 23:46:54 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d03f2894bda72386c0173392c927f9e6e65e1a69f365bede65dac70bca5e381`  
		Last Modified: Mon, 28 Aug 2023 23:46:54 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ee0058dfff80604b603e9aa8c19de60836c8117737b8fd4a76d148a6cbf36b`  
		Last Modified: Mon, 28 Aug 2023 23:46:54 GMT  
		Size: 1.7 MB (1692452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24595bc69ab369f30d8a7d25a3e361e29f522f995c25a488c349411c7cc74e1b`  
		Last Modified: Mon, 28 Aug 2023 23:46:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24595bc69ab369f30d8a7d25a3e361e29f522f995c25a488c349411c7cc74e1b`  
		Last Modified: Mon, 28 Aug 2023 23:46:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:7.17.12`

```console
$ docker pull logstash@sha256:2fd41b546f9577408c8d48220521ab567ae1901d0d0a1eeffd30b2cc9f5d3918
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:7.17.12` - linux; amd64

```console
$ docker pull logstash@sha256:7ee30dead16a7399ff8ebb74aa7980de7d0a18a03944b6dca574b1f8562dcd97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **440.8 MB (440800786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc5b22368b89f6663d1717846f2515e63c84a4e62d22eca2ad47d39aeebbc8ae`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 10:38:07 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 18 Jul 2023 10:38:07 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.12-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.12 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
WORKDIR /usr/share/logstash
# Tue, 18 Jul 2023 10:38:23 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 18 Jul 2023 10:38:23 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Jul 2023 10:38:23 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
ADD config/log4j2.properties config/ # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 18 Jul 2023 10:38:23 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 18 Jul 2023 10:38:23 GMT
USER 1000
# Tue, 18 Jul 2023 10:38:23 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 18 Jul 2023 10:38:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.12 org.opencontainers.image.version=7.17.12 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-07-18T10:23:11+00:00 org.opencontainers.image.created=2023-07-18T10:23:11+00:00
# Tue, 18 Jul 2023 10:38:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1252d9f3b297e5c3c6f7a6b1052bb8c4774203031e96ec19e180a66ae7b61c3`  
		Last Modified: Thu, 03 Aug 2023 07:24:58 GMT  
		Size: 43.9 MB (43942679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e999dd0a3d26da5c89e4b7cfd15b74f31062e90ae64b9242a3d66dc71585c9`  
		Last Modified: Thu, 03 Aug 2023 07:24:48 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e09a86198b4c2e0ac06fb4cfe12e77ab8a68aa2a48cd37781406521faa6bca`  
		Last Modified: Thu, 03 Aug 2023 07:25:21 GMT  
		Size: 366.5 MB (366458608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2926ddeca1dc60e7ab1599046df086177ac00bee5d78cc1f065e03aafc2e657`  
		Last Modified: Thu, 03 Aug 2023 07:24:47 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94275b63b2f4e420a003e8de4e445d7df4fdf37d1510f64de3cccc17c6f9ab88`  
		Last Modified: Thu, 03 Aug 2023 07:24:47 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1555d37737bb0ecb1a0f5bbfac985e9b32c02dd5d0d4802ee7bed408818bcb0e`  
		Last Modified: Thu, 03 Aug 2023 07:24:41 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01e2f66b7c97d64dae2561b516ead6a0b4d6359e2a704539d4998e27622b5af`  
		Last Modified: Thu, 03 Aug 2023 07:24:41 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a9bf571b75c9ad6eb46d9061a6dcd341403fbb9b2e8a0a70a172388c7a0d5d`  
		Last Modified: Thu, 03 Aug 2023 07:24:41 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ee26d382606e60f1e0768a3b889cdb3b6413c3c55b3abad3747290da35c618`  
		Last Modified: Thu, 03 Aug 2023 07:24:43 GMT  
		Size: 1.8 MB (1812378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7ff156fedab31f1acf57892cc8d66c9503acb37e662386bc7f06ed75d19279`  
		Last Modified: Thu, 03 Aug 2023 07:24:42 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7ff156fedab31f1acf57892cc8d66c9503acb37e662386bc7f06ed75d19279`  
		Last Modified: Thu, 03 Aug 2023 07:24:42 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:7.17.12` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:d70a822a314243d0ba3f1ecb557c06e65bec667324d6f11faaf203ea019a59d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.9 MB (427949674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8a1e5828f0eeffbfb3bfe2704646d23ac468b82bb1dd44627ae3c81a32da4e4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 10:37:27 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 18 Jul 2023 10:37:27 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.12-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.12 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
WORKDIR /usr/share/logstash
# Tue, 18 Jul 2023 10:37:38 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 18 Jul 2023 10:37:38 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Jul 2023 10:37:38 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
ADD config/log4j2.properties config/ # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 18 Jul 2023 10:37:38 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 18 Jul 2023 10:37:39 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 18 Jul 2023 10:37:39 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 18 Jul 2023 10:37:39 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 18 Jul 2023 10:37:39 GMT
USER 1000
# Tue, 18 Jul 2023 10:37:39 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 18 Jul 2023 10:37:39 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.12 org.opencontainers.image.version=7.17.12 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-07-18T10:24:54+00:00 org.opencontainers.image.created=2023-07-18T10:24:54+00:00
# Tue, 18 Jul 2023 10:37:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f656e2e146169db0197119b3cfff78c553a228761fdf62d4b88d4d088a1290`  
		Last Modified: Wed, 23 Aug 2023 23:49:34 GMT  
		Size: 35.8 MB (35824273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed7b6342b1c5d17a38bda4d4872243564a3e920da950553dcfd1ba0a6450e0d`  
		Last Modified: Wed, 23 Aug 2023 23:49:30 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cad957d9dc297ba08b75d3341facce9f9e16426996b56bb3c0855831bfdf6e6`  
		Last Modified: Wed, 23 Aug 2023 23:49:51 GMT  
		Size: 363.2 MB (363227400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d2a71cf994720643a08bb67a56a8105ea88ec156f5e282c74bf770e47ee924`  
		Last Modified: Wed, 23 Aug 2023 23:49:30 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5238d7e910b0e8042c04ae6c4d879bb2802b01f7aab6722af443b1d7dabd99`  
		Last Modified: Wed, 23 Aug 2023 23:49:30 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba297f4b40223b8fdad514908eda5ea58d1cdedad45287ce461621292f065f32`  
		Last Modified: Wed, 23 Aug 2023 23:49:28 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0560c0b3ce97853c8bf46909e51b1a1df082ec80fa578088334f6053ed0720f8`  
		Last Modified: Wed, 23 Aug 2023 23:49:28 GMT  
		Size: 301.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0081570ecad3a57b2a9489baeea7251820b2a3e0e6ab115413f4b996416e2036`  
		Last Modified: Wed, 23 Aug 2023 23:49:28 GMT  
		Size: 2.8 KB (2849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f281dde0d67cb6236f4e8813495726c0e06086f0eb8a0da881a890a7de52b0d`  
		Last Modified: Wed, 23 Aug 2023 23:49:28 GMT  
		Size: 1.7 MB (1692529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d0cb7d2cae30387d1717267cdcfd8fd096cd47c23b86a3a5ca2d88ef0172da`  
		Last Modified: Wed, 23 Aug 2023 23:49:28 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d0cb7d2cae30387d1717267cdcfd8fd096cd47c23b86a3a5ca2d88ef0172da`  
		Last Modified: Wed, 23 Aug 2023 23:49:28 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:8.8.2`

```console
$ docker pull logstash@sha256:6a2f3271ae27585d61c99eb5b9a2e566255a26dccfcf33eea971d18d29bbb9b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:8.8.2` - linux; amd64

```console
$ docker pull logstash@sha256:0d1f7b8a7e846ef54ad904fb7292294e3e8315dfad374aac483142930d932dee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.1 MB (423139221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98494fd39ccbaf76764ab530b41f8820d3afc17614a975ed6146f95bef9f0052`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Wed, 21 Jun 2023 14:03:34 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Wed, 21 Jun 2023 14:03:34 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Wed, 21 Jun 2023 14:03:49 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.8.2-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.8.2 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Wed, 21 Jun 2023 14:03:49 GMT
WORKDIR /usr/share/logstash
# Wed, 21 Jun 2023 14:03:49 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 21 Jun 2023 14:03:49 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Jun 2023 14:03:49 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Wed, 21 Jun 2023 14:03:49 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Wed, 21 Jun 2023 14:03:49 GMT
COPY config/log4j2.properties config/ # buildkit
# Wed, 21 Jun 2023 14:03:49 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Wed, 21 Jun 2023 14:03:49 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Wed, 21 Jun 2023 14:03:49 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Wed, 21 Jun 2023 14:03:49 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 21 Jun 2023 14:03:49 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Wed, 21 Jun 2023 14:03:49 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Wed, 21 Jun 2023 14:03:49 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Wed, 21 Jun 2023 14:03:49 GMT
USER 1000
# Wed, 21 Jun 2023 14:03:49 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Wed, 21 Jun 2023 14:03:49 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.8.2 org.opencontainers.image.version=8.8.2 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-06-21T13:46:18+00:00 org.opencontainers.image.created=2023-06-21T13:46:18+00:00
# Wed, 21 Jun 2023 14:03:49 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789f6fbd7d32984f197e9dc674c73ef26519774f16254267a600a032b1272a31`  
		Last Modified: Fri, 30 Jun 2023 02:07:56 GMT  
		Size: 46.5 MB (46460741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0535fd170f26abc54346a054ce69954ce37fe93bdd4e6b633dda783362eb0247`  
		Last Modified: Fri, 30 Jun 2023 02:07:41 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7807d1e61c76bafb09244dcb684d0a97809e642a8b14b3cba0a13fc5c5495794`  
		Last Modified: Fri, 30 Jun 2023 02:09:07 GMT  
		Size: 346.3 MB (346275945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f178a3345415e2309dc5503b9ef30d6e049e3c850a75d2b066ede54d62d3b826`  
		Last Modified: Fri, 30 Jun 2023 02:07:38 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0e06c1f5d7f569517c6dafe3f75671269d5c54d39829db89884dc6fde5adb2`  
		Last Modified: Fri, 30 Jun 2023 02:07:37 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326858fef28416689241ce827c2bc768de52c97badea9efd6fe167c35db4a59`  
		Last Modified: Fri, 30 Jun 2023 02:07:37 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5814131b9e5ce765979155240acf8f1167588236b794ce027ab1f8c1c9f90c`  
		Last Modified: Fri, 30 Jun 2023 02:07:36 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578c7ad8cea2ea9d553ef0f077d2aee3582cc7816322c8cf0b5dec6765fa231b`  
		Last Modified: Fri, 30 Jun 2023 02:07:32 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd48044cac9dfeddf61a77b2978612d76858b4cf2ed1aef2ff4d560f098331e`  
		Last Modified: Fri, 30 Jun 2023 02:07:32 GMT  
		Size: 3.7 KB (3664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac771a510503cd1dd3f6a28649224bf74260574d003aad98aa5fbe5f61621f44`  
		Last Modified: Fri, 30 Jun 2023 02:07:33 GMT  
		Size: 1.8 MB (1812282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc11c88c665ceccd027167b43ba9e773cb6e4f0b6cbb9081a470fdb9d80d6a7`  
		Last Modified: Fri, 30 Jun 2023 02:07:31 GMT  
		Size: 716.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc11c88c665ceccd027167b43ba9e773cb6e4f0b6cbb9081a470fdb9d80d6a7`  
		Last Modified: Fri, 30 Jun 2023 02:07:31 GMT  
		Size: 716.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:8.8.2` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:34a5d64a41f416527545bcf62bdf0cf3ceecabab319f2973a151b6c57ca5fa08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.5 MB (412492366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b62cb6820e3601d5198f21ce776987316fb99ff34dcc395d43a9575f71de5757`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Wed, 21 Jun 2023 14:02:19 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Wed, 21 Jun 2023 14:02:20 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Wed, 21 Jun 2023 14:02:31 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.8.2-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.8.2 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Wed, 21 Jun 2023 14:02:31 GMT
WORKDIR /usr/share/logstash
# Wed, 21 Jun 2023 14:02:31 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 21 Jun 2023 14:02:31 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Jun 2023 14:02:31 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Wed, 21 Jun 2023 14:02:31 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Wed, 21 Jun 2023 14:02:31 GMT
COPY config/log4j2.properties config/ # buildkit
# Wed, 21 Jun 2023 14:02:31 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Wed, 21 Jun 2023 14:02:31 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Wed, 21 Jun 2023 14:02:31 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Wed, 21 Jun 2023 14:02:31 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 21 Jun 2023 14:02:31 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Wed, 21 Jun 2023 14:02:31 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Wed, 21 Jun 2023 14:02:31 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Wed, 21 Jun 2023 14:02:31 GMT
USER 1000
# Wed, 21 Jun 2023 14:02:31 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Wed, 21 Jun 2023 14:02:31 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.8.2 org.opencontainers.image.version=8.8.2 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-06-21T13:47:23+00:00 org.opencontainers.image.created=2023-06-21T13:47:23+00:00
# Wed, 21 Jun 2023 14:02:31 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad76b59642dbf733a4a84273e911e2e2b4748fb9f274490f9b613d188e57a51a`  
		Last Modified: Wed, 19 Jul 2023 20:08:24 GMT  
		Size: 38.5 MB (38504760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d2db1ecafc08427da6dc5b1c985363b2bf2e961012e929489b53cf10a2d564`  
		Last Modified: Wed, 19 Jul 2023 20:08:07 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ff06939125ccfdbe5f3f6e707fbc583f20ba3f255d53215f19e78efd6f11ed`  
		Last Modified: Wed, 19 Jul 2023 20:09:44 GMT  
		Size: 345.1 MB (345084703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab140737f4c7d3e331fb3a4ef1fd52c1a0c87290fae9579e9d9edc46de7718e`  
		Last Modified: Wed, 19 Jul 2023 20:08:03 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0026a91b12ed03369a8f104abf6a03ca542452ee218df182ad9481962e7be9c`  
		Last Modified: Wed, 19 Jul 2023 20:08:01 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5031f8426c4e4ace4c7f7eb78e26df9aab15f3d820b59148b9feffea4c47a03`  
		Last Modified: Wed, 19 Jul 2023 20:07:59 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c825e0f63ea8414f432a422e653485cc7308eac812df5473e73686258639a30`  
		Last Modified: Wed, 19 Jul 2023 20:07:58 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b752d4dda263f089fcbb4af22ad62047ef6e52784b0aaab8ea10338b21ff82c`  
		Last Modified: Wed, 19 Jul 2023 20:07:57 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa2fe633c8a576d31dfeecf436edb26de51a184be8a82bc45c3ad8b1b46894b`  
		Last Modified: Wed, 19 Jul 2023 20:07:55 GMT  
		Size: 3.7 KB (3663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06c72c0591c77208524ced54bcbc68a18d909b6bda0c856b0a5e7c39981bc91`  
		Last Modified: Wed, 19 Jul 2023 20:07:54 GMT  
		Size: 1.7 MB (1692713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085ac50da0b250cf55143ab67ce30eda6960489aee1c7c64d138e93854f5ce47`  
		Last Modified: Wed, 19 Jul 2023 20:07:52 GMT  
		Size: 714.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085ac50da0b250cf55143ab67ce30eda6960489aee1c7c64d138e93854f5ce47`  
		Last Modified: Wed, 19 Jul 2023 20:07:52 GMT  
		Size: 714.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:8.9.0`

```console
$ docker pull logstash@sha256:dba961d40055104d178014934da84ed925e08c190ee8fc10b9964c60568b479c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:8.9.0` - linux; amd64

```console
$ docker pull logstash@sha256:18b879ab85fdd1830d4a858a739c60a06d31fed6cc16478f8cc3d68ff99d383c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.9 MB (420872907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b71b698e0aee788b7c68e003d69b5f58eb84485af54f9e305e838b9a49840ab`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 22:34:30 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 18 Jul 2023 22:34:30 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 18 Jul 2023 22:34:45 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.9.0-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.9.0 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 18 Jul 2023 22:34:45 GMT
WORKDIR /usr/share/logstash
# Tue, 18 Jul 2023 22:34:45 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 18 Jul 2023 22:34:45 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Jul 2023 22:34:45 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 18 Jul 2023 22:34:45 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 18 Jul 2023 22:34:45 GMT
COPY config/log4j2.properties config/ # buildkit
# Tue, 18 Jul 2023 22:34:45 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Tue, 18 Jul 2023 22:34:45 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 18 Jul 2023 22:34:45 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 18 Jul 2023 22:34:45 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 18 Jul 2023 22:34:45 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 18 Jul 2023 22:34:45 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 18 Jul 2023 22:34:45 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 18 Jul 2023 22:34:45 GMT
USER 1000
# Tue, 18 Jul 2023 22:34:45 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 18 Jul 2023 22:34:45 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.9.0 org.opencontainers.image.version=8.9.0 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-07-18T22:17:06+00:00 org.opencontainers.image.created=2023-07-18T22:17:06+00:00
# Tue, 18 Jul 2023 22:34:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc971b7f21961bd51e9079b454b8052b521ab79d397506c147fb3657ac3b53ea`  
		Last Modified: Thu, 27 Jul 2023 00:58:57 GMT  
		Size: 43.9 MB (43943740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bc82c7dbf7cf1e8cbcdf1bc47c51e5a0a124431c72337de48d9bc2eb6fbf1d`  
		Last Modified: Thu, 27 Jul 2023 00:58:03 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1076ef9ff32c33f2f0308dbbdec1076741e299b2abd0cfef7b61ed92dbf5d28`  
		Last Modified: Thu, 27 Jul 2023 00:58:55 GMT  
		Size: 346.5 MB (346526672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a9333ee7d3662f5a3e6e50d29b31e82fe94aeea19eecea08f44e6118d75498`  
		Last Modified: Thu, 27 Jul 2023 00:57:59 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179064d066eb7977022eb3f76f0f08e58ce8044f97fe04eedc634563e42b49d5`  
		Last Modified: Thu, 27 Jul 2023 00:57:58 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001f78af36a6271105080b6ac6b1f49591dd77d323073ce2085c527e4ef1a3c8`  
		Last Modified: Thu, 27 Jul 2023 00:57:58 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e48cee616660a5efd99f3a5fec292c03a729dec03478d6538bc246d3118654`  
		Last Modified: Thu, 27 Jul 2023 00:57:56 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516a421972e98fcf7280497ce61e744ce34fed849b26742643876a7a89c574e5`  
		Last Modified: Thu, 27 Jul 2023 00:57:53 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98c15e15795c701478cfdca30869ccf4e0b129d1fa5e1b78bd62f99386ebad2`  
		Last Modified: Thu, 27 Jul 2023 00:57:53 GMT  
		Size: 3.7 KB (3660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20fcff799df999806d4c52a97281276426bd1daff0e7c114200fb6c7dbafcac`  
		Last Modified: Thu, 27 Jul 2023 00:57:55 GMT  
		Size: 1.8 MB (1812749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39598a11b350938033acdaa4a867ab82b376dce4fffa8cdfea05c6d468c8e146`  
		Last Modified: Thu, 27 Jul 2023 00:57:51 GMT  
		Size: 715.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39598a11b350938033acdaa4a867ab82b376dce4fffa8cdfea05c6d468c8e146`  
		Last Modified: Thu, 27 Jul 2023 00:57:51 GMT  
		Size: 715.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:8.9.0` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:e4a561da021cb17d581152618a59d0672c28a97706277ab5bfc164afd5eaa67f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **410.1 MB (410063134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2283e0c1e588730631f015e77983ff4027b087a48c679243a307b78931d95303`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 22:34:30 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 18 Jul 2023 22:34:31 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 18 Jul 2023 22:34:40 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.9.0-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.9.0 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 18 Jul 2023 22:34:40 GMT
WORKDIR /usr/share/logstash
# Tue, 18 Jul 2023 22:34:40 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 18 Jul 2023 22:34:40 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Jul 2023 22:34:40 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 18 Jul 2023 22:34:40 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 18 Jul 2023 22:34:40 GMT
COPY config/log4j2.properties config/ # buildkit
# Tue, 18 Jul 2023 22:34:40 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Tue, 18 Jul 2023 22:34:40 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 18 Jul 2023 22:34:41 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 18 Jul 2023 22:34:41 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 18 Jul 2023 22:34:41 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 18 Jul 2023 22:34:41 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 18 Jul 2023 22:34:41 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 18 Jul 2023 22:34:41 GMT
USER 1000
# Tue, 18 Jul 2023 22:34:41 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 18 Jul 2023 22:34:41 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.9.0 org.opencontainers.image.version=8.9.0 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-07-18T22:19:14+00:00 org.opencontainers.image.created=2023-07-18T22:19:14+00:00
# Tue, 18 Jul 2023 22:34:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233276fcf149bfb2d73fda0a92abb6960d5873f327b32b4dcb527b8570444dbd`  
		Last Modified: Thu, 17 Aug 2023 15:11:01 GMT  
		Size: 35.8 MB (35824239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e9941d7770ddfc7da17d0745630fb7ea427d8d9beb58a64c4d0161233cd10fb`  
		Last Modified: Thu, 17 Aug 2023 15:10:45 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630b808c2b1d4b077e694f12767bebf66c360acc0af114223490fa58d23efab5`  
		Last Modified: Thu, 17 Aug 2023 15:11:58 GMT  
		Size: 345.3 MB (345338026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59f11f4ec43d20d9d1f1f673d2e1429174a54a3c9cd456d18a4872d0488cc10`  
		Last Modified: Thu, 17 Aug 2023 15:10:43 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a203f885d0daada5aa506a137ed88e9aeecf3d8157a0a72985609deafab92d95`  
		Last Modified: Thu, 17 Aug 2023 15:10:42 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc92bd5d4e9eb848f8636fd3f9b5a089d90e21daac60363f2aad5c0c795bfd0`  
		Last Modified: Thu, 17 Aug 2023 15:10:42 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3b04efff6abde82d32db3fba20643df84dfd4965b5410d1186e8aa84443b29`  
		Last Modified: Thu, 17 Aug 2023 15:10:42 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283bb0f7a1e2b67f070542a44772f19c3f055cf7c257b11a2f5cd5c35abb5250`  
		Last Modified: Thu, 17 Aug 2023 15:10:40 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391fd6e857abb37207a280cde0a0c363a12d027746a27045ff3d419f0fd8029b`  
		Last Modified: Thu, 17 Aug 2023 15:10:39 GMT  
		Size: 3.7 KB (3659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226639cd5dd0e3b30e429b08fd50b47a04bdf736e6d40b3131e2af2c03eb7835`  
		Last Modified: Thu, 17 Aug 2023 15:10:40 GMT  
		Size: 1.7 MB (1692789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9bc68fab5b9dbfb25d82d403ad53bb69d5559fa2d5a759b8171025ba222a42`  
		Last Modified: Thu, 17 Aug 2023 15:10:39 GMT  
		Size: 712.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9bc68fab5b9dbfb25d82d403ad53bb69d5559fa2d5a759b8171025ba222a42`  
		Last Modified: Thu, 17 Aug 2023 15:10:39 GMT  
		Size: 712.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:8.9.1`

```console
$ docker pull logstash@sha256:0bb447991e28a292f628e8d2d8348aa7bf04b1b4c15420e757ff4082976b1894
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:8.9.1` - linux; amd64

```console
$ docker pull logstash@sha256:c6426f31ecd51af6f42d09e1e0fa06a659876cda6e82d30dced4c57aac3385e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **423.8 MB (423846956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6936c50aa9f5575bda6355a4483442bb93564ab579e1c41eb1061d39e6f291f2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Wed, 09 Aug 2023 09:33:59 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Wed, 09 Aug 2023 09:34:00 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Wed, 09 Aug 2023 09:34:15 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.9.1-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.9.1 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Wed, 09 Aug 2023 09:34:15 GMT
WORKDIR /usr/share/logstash
# Wed, 09 Aug 2023 09:34:15 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 09 Aug 2023 09:34:15 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 09:34:15 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Wed, 09 Aug 2023 09:34:15 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Wed, 09 Aug 2023 09:34:15 GMT
COPY config/log4j2.properties config/ # buildkit
# Wed, 09 Aug 2023 09:34:15 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Wed, 09 Aug 2023 09:34:15 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Wed, 09 Aug 2023 09:34:16 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Wed, 09 Aug 2023 09:34:16 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 09 Aug 2023 09:34:16 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Wed, 09 Aug 2023 09:34:16 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Wed, 09 Aug 2023 09:34:16 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Wed, 09 Aug 2023 09:34:16 GMT
USER 1000
# Wed, 09 Aug 2023 09:34:16 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Wed, 09 Aug 2023 09:34:16 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.9.1 org.opencontainers.image.version=8.9.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-08-09T09:16:22+00:00 org.opencontainers.image.created=2023-08-09T09:16:22+00:00
# Wed, 09 Aug 2023 09:34:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5359ae0673f6465c56eef216725f93611ccbd885a57a2e45db4327b6e2d299`  
		Last Modified: Mon, 21 Aug 2023 01:12:58 GMT  
		Size: 44.2 MB (44199436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db56260ef5189b04b8bc545509160efe39418817da141051932c823f11658b41`  
		Last Modified: Mon, 21 Aug 2023 01:12:42 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775fc9f3b712d34a2e72897f65c9eb64a2a8e6760704ed92061a61f310747714`  
		Last Modified: Mon, 21 Aug 2023 01:14:26 GMT  
		Size: 349.2 MB (349211378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eacb679e6c68b4a6f96c0301bbf6707ae5b40cb09bd49429e593b3e937c573`  
		Last Modified: Mon, 21 Aug 2023 01:12:39 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371c474647f3a9e7999594e7027ab6775dcf8f036afa02c4a3d765cb64e10502`  
		Last Modified: Mon, 21 Aug 2023 01:12:37 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d330bd7cfeed9bcd7ac5a551003f84ec670d9f200e27e84b95afaecf9efd6e1`  
		Last Modified: Mon, 21 Aug 2023 01:12:37 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b9fdbb7215070b6f1da81f59b564195f2e8eb52c31660b36b29736e10ce223`  
		Last Modified: Mon, 21 Aug 2023 01:12:33 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0ff13c9e7e53683a04815aa2aba5ee38326492dc85111b86fdb03e82ec5475`  
		Last Modified: Mon, 21 Aug 2023 01:12:32 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676641b254abdc3e180c98dae3023debeb83f2f0f895f00d6bd402c15062ccb6`  
		Last Modified: Mon, 21 Aug 2023 01:12:32 GMT  
		Size: 3.7 KB (3658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2084757ec44b4717016898ddfa1b87fac148998c34d61062ff6c4102b1f6c7`  
		Last Modified: Mon, 21 Aug 2023 01:12:34 GMT  
		Size: 1.8 MB (1845755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e194c1340f610d95bfa4e2674a249a7ca7da20def3b0999101a940c18f9ea4b`  
		Last Modified: Mon, 21 Aug 2023 01:12:29 GMT  
		Size: 713.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e194c1340f610d95bfa4e2674a249a7ca7da20def3b0999101a940c18f9ea4b`  
		Last Modified: Mon, 21 Aug 2023 01:12:29 GMT  
		Size: 713.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:8.9.1` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:f05007232cbea8260b19985dc93f678d6df21f6573425f3189b69c8cfc3f527f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **412.9 MB (412878009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35359e0ff01a56a25d15b2a07eb80f539804b59228f2044974c60c0682a17c41`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Wed, 09 Aug 2023 09:33:45 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Wed, 09 Aug 2023 09:33:46 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.9.1-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.9.1 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
WORKDIR /usr/share/logstash
# Wed, 09 Aug 2023 09:33:57 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 09 Aug 2023 09:33:57 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 09:33:57 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
COPY config/log4j2.properties config/ # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 09 Aug 2023 09:33:57 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Wed, 09 Aug 2023 09:33:57 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Wed, 09 Aug 2023 09:33:58 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Wed, 09 Aug 2023 09:33:58 GMT
USER 1000
# Wed, 09 Aug 2023 09:33:58 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Wed, 09 Aug 2023 09:33:58 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.9.1 org.opencontainers.image.version=8.9.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-08-09T09:18:39+00:00 org.opencontainers.image.created=2023-08-09T09:18:39+00:00
# Wed, 09 Aug 2023 09:33:58 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2f56f1fc0d4f5cceae94a8523ca467ed142176439825de68c798e80192e565`  
		Last Modified: Wed, 23 Aug 2023 23:49:05 GMT  
		Size: 35.9 MB (35932005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8e875a123e6aa7ec6ac07589c20ef9db6fe2ae7c22d1e4023e494dbb6fb817`  
		Last Modified: Wed, 23 Aug 2023 23:49:00 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add229aa6531457e942490d0c9641318aad1be6f4e3e105159a8d329c862656c`  
		Last Modified: Wed, 23 Aug 2023 23:49:21 GMT  
		Size: 348.0 MB (348003915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e855164e968b4367c4c4520a17314de145b5fa341388d77e275fbb707a0d45eb`  
		Last Modified: Wed, 23 Aug 2023 23:48:59 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4ff0af73d95373ad3d295cf48a86d7b9149ee050e6a1d235d64ad3c84c659d`  
		Last Modified: Wed, 23 Aug 2023 23:48:59 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122591da54f2a672df995488e8ce0f44d3520f39f6ab06047bc9ffd3b648c8f8`  
		Last Modified: Wed, 23 Aug 2023 23:48:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a536cfd44c31fb9c2e7015ace6b05bdecc5a283178b849ddf44a062d7e7afb3d`  
		Last Modified: Wed, 23 Aug 2023 23:48:57 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7665b9b744acfb88017f4c5f9a9a40eaf20fe07989549cfc32d9fc631498239c`  
		Last Modified: Wed, 23 Aug 2023 23:48:57 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf44f9ce281a1091f5f597c047ab5bcca248833a9907cc921f18b2e879cfb06c`  
		Last Modified: Wed, 23 Aug 2023 23:48:57 GMT  
		Size: 3.7 KB (3663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6ee346489fef9a8fbbff680574d521c63615e1e234f022f0214abe781c9452`  
		Last Modified: Wed, 23 Aug 2023 23:48:58 GMT  
		Size: 1.7 MB (1731755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67393b314f805c926ccd95d69053134780f725a101a7c19d5e504c7ad4fa228a`  
		Last Modified: Wed, 23 Aug 2023 23:48:57 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67393b314f805c926ccd95d69053134780f725a101a7c19d5e504c7ad4fa228a`  
		Last Modified: Wed, 23 Aug 2023 23:48:57 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
