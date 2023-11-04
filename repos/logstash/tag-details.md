<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:7.17.14`](#logstash71714)
-	[`logstash:8.10.3`](#logstash8103)
-	[`logstash:8.10.4`](#logstash8104)

## `logstash:7.17.14`

```console
$ docker pull logstash@sha256:4c6a4510c70519fc2407978e2cd94ada9f36e75ceae06015462c0dafbcc3597f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:7.17.14` - linux; amd64

```console
$ docker pull logstash@sha256:c48538d579270d7c6310ff97b092d4c6bb4d21c4775dcd6892ec55084563a562
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **449.2 MB (449159622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52cc476a69e28cc52f1693e993d2d80e029dfb0ff4f6bbd1b7601083e66abbb9`
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
# Wed, 04 Oct 2023 20:57:59 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Wed, 04 Oct 2023 20:57:59 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Wed, 04 Oct 2023 20:58:16 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.14-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.14 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Wed, 04 Oct 2023 20:58:16 GMT
WORKDIR /usr/share/logstash
# Wed, 04 Oct 2023 20:58:16 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 04 Oct 2023 20:58:16 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 20:58:16 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Wed, 04 Oct 2023 20:58:16 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Wed, 04 Oct 2023 20:58:16 GMT
ADD config/log4j2.properties config/ # buildkit
# Wed, 04 Oct 2023 20:58:17 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Wed, 04 Oct 2023 20:58:17 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Wed, 04 Oct 2023 20:58:17 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 20:58:17 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 20:58:17 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 20:58:17 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Wed, 04 Oct 2023 20:58:17 GMT
USER 1000
# Wed, 04 Oct 2023 20:58:17 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Wed, 04 Oct 2023 20:58:17 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.14 org.opencontainers.image.version=7.17.14 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-10-04T20:42:06+00:00 org.opencontainers.image.created=2023-10-04T20:42:06+00:00
# Wed, 04 Oct 2023 20:58:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b107fdeb890390bbf4f65ae06f02e6e795ffa91229587c4b591c92d1ffc417`  
		Last Modified: Mon, 16 Oct 2023 20:40:10 GMT  
		Size: 51.9 MB (51877041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb675bf90dfbc25f88d969ed5d80cafda779a6d5c532d3a8893494681890472`  
		Last Modified: Mon, 16 Oct 2023 20:40:05 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32891a2ae2b653645f4eada15556b945a9b9c09a7d3d666c12ebd544770495fa`  
		Last Modified: Fri, 03 Nov 2023 00:29:15 GMT  
		Size: 366.8 MB (366849372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9168fc7838a496a51b803e4c4831d51a5274b1c56e82f077814a51d31e3a25`  
		Last Modified: Fri, 03 Nov 2023 00:28:50 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc57d4b552c6b37be445b955acdb109d96cedd72a83c771f418a53ff4807ad93`  
		Last Modified: Fri, 03 Nov 2023 00:28:50 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298517f290b1b02321e542d608375e7c32714984d6dd73b1f24d03f91f850a2b`  
		Last Modified: Fri, 03 Nov 2023 00:28:47 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382424169d35f0b7fd88ace97f6e8dec0077154616b527c512ddcd3f18a994ac`  
		Last Modified: Fri, 03 Nov 2023 00:28:48 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20745bfc622e947bab450b4d85ee8922aede6dca50a87a040cbc6c9bedf2ac54`  
		Last Modified: Fri, 03 Nov 2023 00:28:48 GMT  
		Size: 2.9 KB (2857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f104298fd5baca4a4316fe46ceaf4c0b25d78512a30562bb16fe06f16c0a13`  
		Last Modified: Fri, 03 Nov 2023 00:28:48 GMT  
		Size: 1.8 MB (1845412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7718ac05fbcbde0f045da76bdfcf6ed4c3aa26849b4b61be20b05d0d8afd1635`  
		Last Modified: Fri, 03 Nov 2023 00:28:48 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7718ac05fbcbde0f045da76bdfcf6ed4c3aa26849b4b61be20b05d0d8afd1635`  
		Last Modified: Fri, 03 Nov 2023 00:28:48 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:7.17.14` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:6ea5bdac812616d570900dad33c326713c7a893b9ad3b91f9198ffaaffd47a2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **434.4 MB (434391590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:946d678c8e0f94906289d983b96e33b766da7999c3432161134a3daa5a7075c4`
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
# Wed, 04 Oct 2023 20:39:28 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Wed, 04 Oct 2023 20:39:28 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Wed, 04 Oct 2023 20:39:40 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.14-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.14 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Wed, 04 Oct 2023 20:39:40 GMT
WORKDIR /usr/share/logstash
# Wed, 04 Oct 2023 20:39:40 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 04 Oct 2023 20:39:40 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 20:39:40 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Wed, 04 Oct 2023 20:39:40 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Wed, 04 Oct 2023 20:39:40 GMT
ADD config/log4j2.properties config/ # buildkit
# Wed, 04 Oct 2023 20:39:40 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Wed, 04 Oct 2023 20:39:40 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Wed, 04 Oct 2023 20:39:40 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 20:39:41 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 20:39:41 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 20:39:41 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Wed, 04 Oct 2023 20:39:41 GMT
USER 1000
# Wed, 04 Oct 2023 20:39:41 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Wed, 04 Oct 2023 20:39:41 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.14 org.opencontainers.image.version=7.17.14 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-10-04T20:26:30+00:00 org.opencontainers.image.created=2023-10-04T20:26:30+00:00
# Wed, 04 Oct 2023 20:39:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8570723baef81aa71f25cc4d6367edcfee15d403fdc10efc46c66ef25ffb5714`  
		Last Modified: Thu, 02 Nov 2023 23:44:26 GMT  
		Size: 41.9 MB (41871429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0831b7063265cb07b8ccdde4e1175aad813fd318b9d946bf8147f7fa265d46`  
		Last Modified: Thu, 02 Nov 2023 23:44:22 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbfd58f0e726287d3b2b777700b1c70e5a2579548b2801ed48e862c966d0661`  
		Last Modified: Thu, 02 Nov 2023 23:44:43 GMT  
		Size: 363.6 MB (363581002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4f80b55754a4f469081ab2870b370f2390526a1467ee401ab5803476be06f4`  
		Last Modified: Thu, 02 Nov 2023 23:44:22 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bb4874287977598ef6ef816828bbe9aeb111b07ac14ed75453ae09a82dac8e`  
		Last Modified: Thu, 02 Nov 2023 23:44:22 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ec214a887992f334d709d5bcd4cef28511151b0cd79c1389c78484ef9cff6c`  
		Last Modified: Thu, 02 Nov 2023 23:44:20 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fb258ad04aaccd6f52ceb4faa7af07348205b31ce41ed1c2d8ca2fd1df611c`  
		Last Modified: Thu, 02 Nov 2023 23:44:20 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1496addb12ddc8e0c27636eaaf5be0889b4c23bf17e413d689ca4d61b3cbcc15`  
		Last Modified: Thu, 02 Nov 2023 23:44:20 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1385ea9453048b50ae21f31203fc9421a32c88414ab7e87cd3c7a4fd61a2b9ad`  
		Last Modified: Thu, 02 Nov 2023 23:44:20 GMT  
		Size: 1.7 MB (1731455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7b57460578d71d5c3fd21ab5e9c3c558e92b99471e3d95795ee5b739c35ae7`  
		Last Modified: Thu, 02 Nov 2023 23:44:20 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7b57460578d71d5c3fd21ab5e9c3c558e92b99471e3d95795ee5b739c35ae7`  
		Last Modified: Thu, 02 Nov 2023 23:44:20 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:8.10.3`

```console
$ docker pull logstash@sha256:9beee9d97d60aa65a78715d1fbdc3e15322596df8f57fdf3caaf12a6766b6a18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `logstash:8.10.3` - linux; amd64

```console
$ docker pull logstash@sha256:a343ca31ce3665b487d31cd02143d25e499678b76afded7b27eb3fdc944a0368
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **431.8 MB (431847754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51c61d200ef318f0c8be16de32aff44456eb824fbe73c483e3b439b891e202b5`
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
# Wed, 04 Oct 2023 17:04:41 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Wed, 04 Oct 2023 17:04:42 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Wed, 04 Oct 2023 17:04:56 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.10.3-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.10.3 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Wed, 04 Oct 2023 17:04:56 GMT
WORKDIR /usr/share/logstash
# Wed, 04 Oct 2023 17:04:56 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 04 Oct 2023 17:04:56 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 04 Oct 2023 17:04:56 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Wed, 04 Oct 2023 17:04:56 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Wed, 04 Oct 2023 17:04:56 GMT
COPY config/log4j2.properties config/ # buildkit
# Wed, 04 Oct 2023 17:04:56 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Wed, 04 Oct 2023 17:04:56 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Wed, 04 Oct 2023 17:04:56 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Wed, 04 Oct 2023 17:04:56 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 04 Oct 2023 17:04:56 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 17:04:56 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Wed, 04 Oct 2023 17:04:56 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Wed, 04 Oct 2023 17:04:56 GMT
USER 1000
# Wed, 04 Oct 2023 17:04:56 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Wed, 04 Oct 2023 17:04:56 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.10.3 org.opencontainers.image.version=8.10.3 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-10-04T16:45:48+00:00 org.opencontainers.image.created=2023-10-04T16:45:48+00:00
# Wed, 04 Oct 2023 17:04:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c3383400494f86abad6900163532176b39161c4dac00f02811abf5dd9145b4`  
		Last Modified: Tue, 10 Oct 2023 11:55:22 GMT  
		Size: 51.8 MB (51790800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a39f3cfce515e97f9bd624c91c763ff4bb5b9e0dad8e8a6bbf277a1cc98617`  
		Last Modified: Tue, 10 Oct 2023 11:52:21 GMT  
		Size: 1.8 KB (1832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3f3705f59575ac5ae7edd4eed29b2aa2d7eb1ac85a191e4475943a2c98fed1`  
		Last Modified: Wed, 11 Oct 2023 23:45:15 GMT  
		Size: 349.6 MB (349621031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e19addd415b188977d0c9a336af31a7e03b3ab68b9c44dcb181dc116b699a0`  
		Last Modified: Wed, 11 Oct 2023 23:44:23 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8849bee9c0eb44d20553fa9e22fe10967ee26337ead708390783cab483fae4d`  
		Last Modified: Wed, 11 Oct 2023 23:44:22 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8206904a466a84c37c597d14119080278ad0a0753e2e3948d75fb4f8da958c3`  
		Last Modified: Wed, 11 Oct 2023 23:44:21 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee7776c48fd0abd52a7c76bc530b85920c4b2ddd8558879296a18b4cbb91764`  
		Last Modified: Wed, 11 Oct 2023 23:44:19 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942f94df0fd14bfed2d7c236689d670bff1124893e10e1db9857c07122dbfc59`  
		Last Modified: Wed, 11 Oct 2023 23:44:18 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552a8473494df1da01e00d2ca8060bcf00d9acdd7dd660d1a87372b94907d60b`  
		Last Modified: Wed, 11 Oct 2023 23:44:17 GMT  
		Size: 3.7 KB (3659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c3061e47fc6fb399481d6ba8ffebcf405132f672442cba18e8d7fecc1885c7`  
		Last Modified: Wed, 11 Oct 2023 23:44:18 GMT  
		Size: 1.8 MB (1845527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb30d60fc89a1a2b86b73f86a0bc435cac1540d9ae80cf1b53faf125cc81754`  
		Last Modified: Wed, 11 Oct 2023 23:44:14 GMT  
		Size: 715.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb30d60fc89a1a2b86b73f86a0bc435cac1540d9ae80cf1b53faf125cc81754`  
		Last Modified: Wed, 11 Oct 2023 23:44:14 GMT  
		Size: 715.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:8.10.4`

```console
$ docker pull logstash@sha256:6492b76ff69ce7717d28556003ff7233369c5622cba7d6b6935e05ea2db8a170
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:8.10.4` - linux; amd64

```console
$ docker pull logstash@sha256:1131cec9271195b611ad413fccbd0e64bd5e0e2eb0cc4635a9433d369a50830a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **432.1 MB (432060540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8148449f39acc8813c98e839b264fd8a480e6f709a1ca11b4c287fe96705e570`
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
# Tue, 10 Oct 2023 17:34:54 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 10 Oct 2023 17:34:54 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 10 Oct 2023 17:35:03 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.10.4-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.10.4 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 10 Oct 2023 17:35:03 GMT
WORKDIR /usr/share/logstash
# Tue, 10 Oct 2023 17:35:03 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 10 Oct 2023 17:35:03 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 17:35:03 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 10 Oct 2023 17:35:03 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 10 Oct 2023 17:35:04 GMT
COPY config/log4j2.properties config/ # buildkit
# Tue, 10 Oct 2023 17:35:04 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Tue, 10 Oct 2023 17:35:04 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 10 Oct 2023 17:35:04 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 10 Oct 2023 17:35:04 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 10 Oct 2023 17:35:04 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 10 Oct 2023 17:35:04 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 10 Oct 2023 17:35:04 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 10 Oct 2023 17:35:04 GMT
USER 1000
# Tue, 10 Oct 2023 17:35:04 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 10 Oct 2023 17:35:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.10.4 org.opencontainers.image.version=8.10.4 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-10-10T17:23:58+00:00 org.opencontainers.image.created=2023-10-10T17:23:58+00:00
# Tue, 10 Oct 2023 17:35:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d03e41d9da07b0dfa3d53b004927e34cb939ec0c9cc981f0d95b64aeb5aa59`  
		Last Modified: Tue, 17 Oct 2023 20:30:16 GMT  
		Size: 51.9 MB (51918416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f16ce226f0706c8e24cf919796958c713f06709aa489290dc56fe5ad4ece17`  
		Last Modified: Tue, 17 Oct 2023 20:29:59 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6e4dcc1090add70b305c6a7fbdc088dad89226aa089fe3e8a55fd3b917f046`  
		Last Modified: Tue, 17 Oct 2023 20:31:18 GMT  
		Size: 349.7 MB (349705711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7394657b38310e1d680bf0e1325e1b9dc3cb152f8ea7658d1815c33e53a4f2b6`  
		Last Modified: Tue, 17 Oct 2023 20:29:56 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a859a8e523c3c217f9e7b9654da7edfe30215e272c500634375695c686eaae`  
		Last Modified: Tue, 17 Oct 2023 20:29:53 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0fc993e38a4afd2fce0670a3384bab22457e9e55c6924429bd0c5ba454f729`  
		Last Modified: Tue, 17 Oct 2023 20:29:53 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90783c443677f47db89a75ab088b8bb7c173a89540cd42f69764ca42637395c`  
		Last Modified: Tue, 17 Oct 2023 20:29:50 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea9b1cddfb6abc24b7e9d4453cf288af4298ac6db70ea54ae7493fd75163e1f`  
		Last Modified: Tue, 17 Oct 2023 20:29:50 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7c867dcd167511c432bc773aed049072702449ad6667442a3ecbc54080c631`  
		Last Modified: Tue, 17 Oct 2023 20:29:47 GMT  
		Size: 3.7 KB (3657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc66a741d02ecca72f8d3c3ec00a0ec565ad35a483e9e6c5e08e06f5b3e7c2a7`  
		Last Modified: Tue, 17 Oct 2023 20:29:47 GMT  
		Size: 1.8 MB (1846028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6363ffb5a919f21b460c76851d14b2b7bb67ac472d9b640af854a36cc99c1587`  
		Last Modified: Tue, 17 Oct 2023 20:29:44 GMT  
		Size: 715.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6363ffb5a919f21b460c76851d14b2b7bb67ac472d9b640af854a36cc99c1587`  
		Last Modified: Tue, 17 Oct 2023 20:29:44 GMT  
		Size: 715.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:8.10.4` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:0d3dbab8bcf0875040f4301b051015ab7d9e4e51368499a665e5ab4757768882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.3 MB (419319934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bad54333c7a312b23e0d8db831817ba4f27bca4e8ade528105dc2915976e4a95`
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
# Tue, 10 Oct 2023 17:40:23 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 10 Oct 2023 17:40:24 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 10 Oct 2023 17:40:37 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.10.4-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.10.4 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 10 Oct 2023 17:40:37 GMT
WORKDIR /usr/share/logstash
# Tue, 10 Oct 2023 17:40:37 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 10 Oct 2023 17:40:37 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 17:40:37 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 10 Oct 2023 17:40:37 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 10 Oct 2023 17:40:37 GMT
COPY config/log4j2.properties config/ # buildkit
# Tue, 10 Oct 2023 17:40:37 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Tue, 10 Oct 2023 17:40:37 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 10 Oct 2023 17:40:37 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 10 Oct 2023 17:40:37 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 10 Oct 2023 17:40:37 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 10 Oct 2023 17:40:37 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 10 Oct 2023 17:40:37 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 10 Oct 2023 17:40:37 GMT
USER 1000
# Tue, 10 Oct 2023 17:40:37 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 10 Oct 2023 17:40:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.10.4 org.opencontainers.image.version=8.10.4 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-10-10T17:26:22+00:00 org.opencontainers.image.created=2023-10-10T17:26:22+00:00
# Tue, 10 Oct 2023 17:40:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720285ce7e9a441a31a8ae42c569f27843fbd67c4986c8790c991697fd54ba47`  
		Last Modified: Tue, 17 Oct 2023 20:10:44 GMT  
		Size: 41.9 MB (41890032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd372ab9ee3f285039d1162836668b5fbe31d3f7d8582ae009fd8a3a4456d7ac`  
		Last Modified: Tue, 17 Oct 2023 20:10:25 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9400bdc71b5fe8a8bf78a58d3d7d2fefceec9dd0cee169721142cf808f65e5f2`  
		Last Modified: Tue, 17 Oct 2023 20:11:44 GMT  
		Size: 348.5 MB (348487985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f18f404a0224c219d0ca859571cad466b89707aacb671f395e57819182c79a`  
		Last Modified: Tue, 17 Oct 2023 20:10:22 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beef200c3bf58ba400f21cbff9c979796f701c2894140775b1cfbae4c746b1ed`  
		Last Modified: Tue, 17 Oct 2023 20:10:19 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630baded7f4c765423f807cb3da6d26eeda79b5aa9fd424f4e25e22e56840542`  
		Last Modified: Tue, 17 Oct 2023 20:10:19 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a6558e014b1a9f627ff4ce1b57528766a8b23952ac5ad3058ee2d6a80925de`  
		Last Modified: Tue, 17 Oct 2023 20:10:16 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2250b082795e1943e5191a19b8314bcf04d0f40c34bcbfd0657accbc84348e`  
		Last Modified: Tue, 17 Oct 2023 20:10:16 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb75e3e8d094f8e014c33aa28a309494ec4c28e3ad76ec1236becb2a7a441b7`  
		Last Modified: Tue, 17 Oct 2023 20:10:13 GMT  
		Size: 3.7 KB (3659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0300fad054fd32016a862ecc088cd0b36353a0c8901b374eeae1ba9d58666f`  
		Last Modified: Tue, 17 Oct 2023 20:10:13 GMT  
		Size: 1.7 MB (1731596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69efcea99f39d6da3df6318efec17080e6540ff96fdf1e78927fac975c784e2`  
		Last Modified: Tue, 17 Oct 2023 20:10:10 GMT  
		Size: 714.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69efcea99f39d6da3df6318efec17080e6540ff96fdf1e78927fac975c784e2`  
		Last Modified: Tue, 17 Oct 2023 20:10:10 GMT  
		Size: 714.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
