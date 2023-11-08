<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:7.17.14`](#logstash71714)
-	[`logstash:8.11.0`](#logstash8110)

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

## `logstash:8.11.0`

```console
$ docker pull logstash@sha256:ff4ec173e2d1a3c1fcdb9b0d63816b732073d95bb6bff8b20f024b76161f6fba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:8.11.0` - linux; amd64

```console
$ docker pull logstash@sha256:7df79743ad8f36544697b4474bcce6fc951dcc381fb10b3bb83e5fd526b6a673
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.9 MB (426907216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15eae9bea4118e3e76039e6bd62d973e1f7f56f530f991ec8bd3b8f69689966`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Tue, 31 Oct 2023 13:12:09 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 31 Oct 2023 13:12:09 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 31 Oct 2023 13:12:19 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.11.0-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.11.0 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 31 Oct 2023 13:12:19 GMT
WORKDIR /usr/share/logstash
# Tue, 31 Oct 2023 13:12:19 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 31 Oct 2023 13:12:19 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 13:12:19 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 31 Oct 2023 13:12:19 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 31 Oct 2023 13:12:19 GMT
COPY config/log4j2.properties config/ # buildkit
# Tue, 31 Oct 2023 13:12:19 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Tue, 31 Oct 2023 13:12:19 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 31 Oct 2023 13:12:19 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 31 Oct 2023 13:12:19 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 31 Oct 2023 13:12:19 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 31 Oct 2023 13:12:19 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 31 Oct 2023 13:12:20 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 31 Oct 2023 13:12:20 GMT
USER 1000
# Tue, 31 Oct 2023 13:12:20 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 31 Oct 2023 13:12:20 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.11.0 org.opencontainers.image.version=8.11.0 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-10-31T12:59:21+00:00 org.opencontainers.image.created=2023-10-31T12:59:21+00:00
# Tue, 31 Oct 2023 13:12:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a36d757376bdb31c8e55cfbc7a14929274200c927bd2b7698f6557ca015bda7`  
		Last Modified: Wed, 08 Nov 2023 00:36:45 GMT  
		Size: 45.8 MB (45762550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921e753636d12b9697a86f9df104498bed5b67fa16bc4ba48b928729db0a8b5f`  
		Last Modified: Wed, 08 Nov 2023 00:36:39 GMT  
		Size: 1.8 KB (1829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5effca0bca8f712a00edcb2034564744492b4e972bc81c5a8b763e2b10583f37`  
		Last Modified: Wed, 08 Nov 2023 00:37:04 GMT  
		Size: 350.7 MB (350708220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2f2b20a1913b0b9e54efcfec80c789e04fc75fda060271ee1c3b79dab56263`  
		Last Modified: Wed, 08 Nov 2023 00:36:38 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe3232de9e3a6f7c67219429646ba6c8b7aa86c593db70b9b33bbb210f89fac`  
		Last Modified: Wed, 08 Nov 2023 00:36:38 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7850786529fdd782f780e8e7cb791b7e5a4611c926080f90076864c11ea5b2`  
		Last Modified: Wed, 08 Nov 2023 00:36:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99484f4aa9fb1bf60cfdcaf2ae20e22f589b8e9d29c9572e26842537f7aa2b10`  
		Last Modified: Wed, 08 Nov 2023 00:36:36 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1603603713419efbeeedd11bd41110d76d4cf0dee2e097eabaab606cadde42d`  
		Last Modified: Wed, 08 Nov 2023 00:36:36 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7abfd7b517eb1f16682d3bfc9548f451e49a7e2cf23e001940703c5ecbf5e8`  
		Last Modified: Wed, 08 Nov 2023 00:36:36 GMT  
		Size: 3.7 KB (3661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8ea812fb969af5c00f7b80f518bdc903d254bd6ec989f7e98906ba598d0297`  
		Last Modified: Wed, 08 Nov 2023 00:36:36 GMT  
		Size: 1.8 MB (1846038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f868f23db5bab0e95510b2fa6bb6c25fb75cbc426c673338b5ba2a7c55e9a`  
		Last Modified: Wed, 08 Nov 2023 00:36:36 GMT  
		Size: 712.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076f868f23db5bab0e95510b2fa6bb6c25fb75cbc426c673338b5ba2a7c55e9a`  
		Last Modified: Wed, 08 Nov 2023 00:36:36 GMT  
		Size: 712.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:8.11.0` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:5e45ebf81ff2a2ecc3443b7d04927bf80c063c0e60e992c8fb681afe5ec25534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.0 MB (414990646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48615bafa582943667b5fd94db20a45d2ac1d8c940da19e83737eb80f7e3e7a2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Tue, 31 Oct 2023 13:16:57 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 31 Oct 2023 13:16:57 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 31 Oct 2023 13:17:10 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.11.0-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.11.0 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 31 Oct 2023 13:17:10 GMT
WORKDIR /usr/share/logstash
# Tue, 31 Oct 2023 13:17:10 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 31 Oct 2023 13:17:10 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 13:17:10 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 31 Oct 2023 13:17:10 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 31 Oct 2023 13:17:10 GMT
COPY config/log4j2.properties config/ # buildkit
# Tue, 31 Oct 2023 13:17:10 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Tue, 31 Oct 2023 13:17:10 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 31 Oct 2023 13:17:10 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 31 Oct 2023 13:17:10 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 31 Oct 2023 13:17:10 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 31 Oct 2023 13:17:10 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 31 Oct 2023 13:17:11 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 31 Oct 2023 13:17:11 GMT
USER 1000
# Tue, 31 Oct 2023 13:17:11 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 31 Oct 2023 13:17:11 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.11.0 org.opencontainers.image.version=8.11.0 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-10-31T13:01:31+00:00 org.opencontainers.image.created=2023-10-31T13:01:31+00:00
# Tue, 31 Oct 2023 13:17:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b19397d8b86f4f79467b24765398bfd29243be689fb63c24639f082326abffb3`  
		Last Modified: Tue, 07 Nov 2023 23:46:43 GMT  
		Size: 36.5 MB (36523118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4907c53a2a95774b4dabb4ba94d4db5845b743ab62d675b337a4cf01219aa123`  
		Last Modified: Tue, 07 Nov 2023 23:46:39 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:becfdd5d1d2692015d7e0b17fb3c68df7e03d6139d4aa20bc07f029d54e3f62d`  
		Last Modified: Tue, 07 Nov 2023 23:46:58 GMT  
		Size: 349.5 MB (349526712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab0fb2b7fb1bee88c5bfbf616a62e69a6c5f344f476c2669ddb1e9f2d22f716`  
		Last Modified: Tue, 07 Nov 2023 23:46:39 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8affec6045259b98bdab39e796e580d1a1051c480fa43cff2023a96045e8d3eb`  
		Last Modified: Tue, 07 Nov 2023 23:46:37 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dd691087de1e52ab450bd17c46470dec82bd5dbad5e4bd6d13e89adbd99644`  
		Last Modified: Tue, 07 Nov 2023 23:46:37 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2e5bf3526f1faae7e8fd5ea7a769bec2ecb475463b6f325e48225f78c3f613`  
		Last Modified: Tue, 07 Nov 2023 23:46:36 GMT  
		Size: 1.4 KB (1361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b02d0197dcd6596874010bfe8a348bcb869369f825e1c027e11281b2ef98ac5`  
		Last Modified: Tue, 07 Nov 2023 23:46:35 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6059852ae6585d855f5e74b4baff4438a5f6cd5dec8f654e826863e8bc2e297a`  
		Last Modified: Tue, 07 Nov 2023 23:46:35 GMT  
		Size: 3.7 KB (3657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bab966623401f91962bbf5fa072e4a2a3554d28f5b3ec0a096eea19aa919493`  
		Last Modified: Tue, 07 Nov 2023 23:46:36 GMT  
		Size: 1.7 MB (1731597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d4d6c5957f0c8c82f80830787acff043033eea3c4578a0a38d1270ff4b730d`  
		Last Modified: Tue, 07 Nov 2023 23:46:35 GMT  
		Size: 713.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d4d6c5957f0c8c82f80830787acff043033eea3c4578a0a38d1270ff4b730d`  
		Last Modified: Tue, 07 Nov 2023 23:46:35 GMT  
		Size: 713.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
