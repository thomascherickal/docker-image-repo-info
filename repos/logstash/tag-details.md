<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:7.17.13`](#logstash71713)
-	[`logstash:8.10.1`](#logstash8101)

## `logstash:7.17.13`

```console
$ docker pull logstash@sha256:205e6bb80eda3e0912a1475eeae8c41fae17dab73337dcd4a2501ff2cb977005
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:7.17.13` - linux; amd64

```console
$ docker pull logstash@sha256:596d903402966164334d38373e48ba5f85c91dce03523c4d9f95569af0ce19ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **441.8 MB (441833995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b3073bfb3bf20c65e02792c748368d9ec1d518cca99b23d7fc1de517fddda74`
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
# Tue, 29 Aug 2023 12:47:46 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 29 Aug 2023 12:47:46 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 29 Aug 2023 12:48:03 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.13-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.13 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 29 Aug 2023 12:48:03 GMT
WORKDIR /usr/share/logstash
# Tue, 29 Aug 2023 12:48:04 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 29 Aug 2023 12:48:04 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Aug 2023 12:48:04 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 29 Aug 2023 12:48:04 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 29 Aug 2023 12:48:04 GMT
ADD config/log4j2.properties config/ # buildkit
# Tue, 29 Aug 2023 12:48:04 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 29 Aug 2023 12:48:04 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 29 Aug 2023 12:48:04 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 29 Aug 2023 12:48:04 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 29 Aug 2023 12:48:04 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 29 Aug 2023 12:48:04 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 29 Aug 2023 12:48:04 GMT
USER 1000
# Tue, 29 Aug 2023 12:48:04 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 29 Aug 2023 12:48:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.13 org.opencontainers.image.version=7.17.13 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-08-29T12:32:19+00:00 org.opencontainers.image.created=2023-08-29T12:32:19+00:00
# Tue, 29 Aug 2023 12:48:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fe34beff15fcddc19b3d739827897fd04abef4f951770b1640e696d1999291`  
		Last Modified: Fri, 08 Sep 2023 05:26:59 GMT  
		Size: 44.6 MB (44555715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103dfd3d5810a1a1db0cc61af270e109fec70ab1b181fb6f169dcf3ef5be4ac0`  
		Last Modified: Fri, 08 Sep 2023 05:26:54 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fabf29352f45b1742ab868f6dc02275b86ec162604933a727c532ea03eed77`  
		Last Modified: Fri, 08 Sep 2023 05:27:20 GMT  
		Size: 366.8 MB (366844936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33474fbbc276e9940864c002c09ff2224b0a39915e6dcf9f035da422ca6a29a`  
		Last Modified: Fri, 08 Sep 2023 05:26:54 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bef82fffd525f24fc964a08df0aeb2e185021675e7cfc9400465e8dca51b680`  
		Last Modified: Fri, 08 Sep 2023 05:26:53 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c608f9d9880413bbc2757cab40c2e7376637fd78946dfa2a49b1453654834e93`  
		Last Modified: Fri, 08 Sep 2023 05:26:51 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86698dc5df38888031dcb159d78a75392eb5a2823024aa50e1c0f17e4bd38965`  
		Last Modified: Fri, 08 Sep 2023 05:26:51 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb509c99c0c97e6a8fecaae5878f01076c872024de433e7dc4e02fbe91824f6`  
		Last Modified: Fri, 08 Sep 2023 05:26:51 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f376629b40d26d3407539bbfb92f950917666b8c59025fecfc3b663a25574bc3`  
		Last Modified: Fri, 08 Sep 2023 05:26:52 GMT  
		Size: 1.8 MB (1845554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33276697c3a28d89f01299c7d291853f9a97833630fe6174c5a4a0d670862b5e`  
		Last Modified: Fri, 08 Sep 2023 05:26:52 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33276697c3a28d89f01299c7d291853f9a97833630fe6174c5a4a0d670862b5e`  
		Last Modified: Fri, 08 Sep 2023 05:26:52 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:7.17.13` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:1e261ec63ea1fc57eecd742dbf537ad158ac8aa354127d98f65f45acedfbea73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.6 MB (428591171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba2b287b529218992f257de967e4f2ab6b39bfc63b61369bcaded88854b6ca61`
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
# Tue, 29 Aug 2023 12:45:15 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 29 Aug 2023 12:45:15 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 29 Aug 2023 12:45:26 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.13-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.13 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 29 Aug 2023 12:45:26 GMT
WORKDIR /usr/share/logstash
# Tue, 29 Aug 2023 12:45:26 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 29 Aug 2023 12:45:26 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Aug 2023 12:45:26 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 29 Aug 2023 12:45:26 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 29 Aug 2023 12:45:26 GMT
ADD config/log4j2.properties config/ # buildkit
# Tue, 29 Aug 2023 12:45:26 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 29 Aug 2023 12:45:26 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 29 Aug 2023 12:45:26 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 29 Aug 2023 12:45:26 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 29 Aug 2023 12:45:26 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 29 Aug 2023 12:45:27 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 29 Aug 2023 12:45:27 GMT
USER 1000
# Tue, 29 Aug 2023 12:45:27 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 29 Aug 2023 12:45:27 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.13 org.opencontainers.image.version=7.17.13 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-08-29T12:32:29+00:00 org.opencontainers.image.created=2023-08-29T12:32:29+00:00
# Tue, 29 Aug 2023 12:45:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5ea6c0a6e78fd90fa1c399208e0f14c1921366555f78829413d37a36715b0e`  
		Last Modified: Thu, 07 Sep 2023 23:43:38 GMT  
		Size: 36.1 MB (36069997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb4bcf9489e2909161fa9daf039479bdbcad05922bb7ab0f11a9d9876bfb641`  
		Last Modified: Thu, 07 Sep 2023 23:43:35 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56aadfb7bd16702a7aaf82f3ae1da7fb5259fd33ff0a7132b4c5db676be3d628`  
		Last Modified: Thu, 07 Sep 2023 23:43:55 GMT  
		Size: 363.6 MB (363581868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbf37db6582af9148061e2ce65bba0e0570141b5e9c6097402e72b2abefb3eb`  
		Last Modified: Thu, 07 Sep 2023 23:43:35 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753a71f4582f6a21100aa94ba6cc4fa8d8ef221a0743dcf7f7dc6bcd4424ae58`  
		Last Modified: Thu, 07 Sep 2023 23:43:35 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544f798f8ae4be9a4eb881952c7978cb109c48d695a8b85cbda153ef4b9cc5fd`  
		Last Modified: Thu, 07 Sep 2023 23:43:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55608cfd1a69a72cc44c8a84d40e76e1718803d8a1aa5726e3a6d16a918e78fa`  
		Last Modified: Thu, 07 Sep 2023 23:43:33 GMT  
		Size: 301.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cbcfe6d2d95a111def3e77a6f0c9f9497513c76973e11bcb0c5bba3f1aeed2`  
		Last Modified: Thu, 07 Sep 2023 23:43:32 GMT  
		Size: 2.9 KB (2850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa6cbec40cff015c83ea9f462dbb1a41ac918a6b32acd9792e4ea83394f54bd`  
		Last Modified: Thu, 07 Sep 2023 23:43:33 GMT  
		Size: 1.7 MB (1731585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044af80824dae93e4d4b92b40e843a968924c023b1ccb29a435e67849d0c0ee6`  
		Last Modified: Thu, 07 Sep 2023 23:43:33 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044af80824dae93e4d4b92b40e843a968924c023b1ccb29a435e67849d0c0ee6`  
		Last Modified: Thu, 07 Sep 2023 23:43:33 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:8.10.1`

```console
$ docker pull logstash@sha256:71f3cc2d7c45e974cd03eeb83012801d28ce95fc148f8d29d367fd48de95ec70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:8.10.1` - linux; amd64

```console
$ docker pull logstash@sha256:3b3353cdbb45c3cd84d683c8973b5b4c922a34297f0f007dc4b3a9472abf577e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.4 MB (424392594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83d72340954a62d414d4fbe583df4fbebe465b80b7c8d1e3b2c75c96b4fa54f8`
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
# Tue, 12 Sep 2023 12:23:58 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 12 Sep 2023 12:23:58 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 12 Sep 2023 12:24:14 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.10.1-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.10.1 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 12 Sep 2023 12:24:14 GMT
WORKDIR /usr/share/logstash
# Tue, 12 Sep 2023 12:24:14 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Sep 2023 12:24:14 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Sep 2023 12:24:14 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 12 Sep 2023 12:24:14 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 12 Sep 2023 12:24:14 GMT
COPY config/log4j2.properties config/ # buildkit
# Tue, 12 Sep 2023 12:24:14 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Tue, 12 Sep 2023 12:24:14 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 12 Sep 2023 12:24:14 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 12 Sep 2023 12:24:14 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 12 Sep 2023 12:24:14 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 12 Sep 2023 12:24:14 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 12 Sep 2023 12:24:14 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 12 Sep 2023 12:24:14 GMT
USER 1000
# Tue, 12 Sep 2023 12:24:14 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 12 Sep 2023 12:24:14 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.10.1 org.opencontainers.image.version=8.10.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-09-12T12:06:28+00:00 org.opencontainers.image.created=2023-09-12T12:06:28+00:00
# Tue, 12 Sep 2023 12:24:14 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed77f4a79dd4b82507f4420990e9ede2b876c4a2f4b3522831d164556ac11b7`  
		Last Modified: Mon, 18 Sep 2023 14:48:57 GMT  
		Size: 44.9 MB (44858922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54c43ef5b9053991e457c5b21e4e40389061e1a79fbd290b21557974b6e61a7`  
		Last Modified: Mon, 18 Sep 2023 14:48:46 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f585fcd1d86dc211493ed91395c6a057d7e74e415daa763cdd32cff4c2094d`  
		Last Modified: Tue, 19 Sep 2023 00:30:57 GMT  
		Size: 349.1 MB (349097753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5b79073e355e48ac93bda3372e56af5fa46db28c6e0952e70231bfef49a14`  
		Last Modified: Tue, 19 Sep 2023 00:30:01 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e4ce4ad57a4668fe6351226deb5e6a2431e4cd292f75a21d37bacba4a6abb8`  
		Last Modified: Tue, 19 Sep 2023 00:30:01 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf65bc38e594e8b05423bf2090c01b18a67952cab5f8d7971ab55f8332923ae`  
		Last Modified: Tue, 19 Sep 2023 00:30:01 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5992ba2ae7ce1cc2302041e8ab3a078b3f45f7f26879829482623ee0c96708f5`  
		Last Modified: Tue, 19 Sep 2023 00:30:00 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd36d8213d9d3cef92566db8ad877b3a3d8a8dfdc31bac3c72914d99659c856`  
		Last Modified: Tue, 19 Sep 2023 00:29:57 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483079d1aedc13b57c5167ff122770e0aac9b677cb283f26410273f2b242e3f7`  
		Last Modified: Tue, 19 Sep 2023 00:29:55 GMT  
		Size: 3.7 KB (3660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a987531bbdd8e18ce2490051d302ba032bfbb6803aeb1411582be9f812fc088`  
		Last Modified: Tue, 19 Sep 2023 00:29:57 GMT  
		Size: 1.8 MB (1845522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100df3ebe98aeed55687083937ef6818ab6c7bf9a2a7f1c7f8ed84481fb66f65`  
		Last Modified: Tue, 19 Sep 2023 00:29:55 GMT  
		Size: 713.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100df3ebe98aeed55687083937ef6818ab6c7bf9a2a7f1c7f8ed84481fb66f65`  
		Last Modified: Tue, 19 Sep 2023 00:29:55 GMT  
		Size: 713.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:8.10.1` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:e07bd08a7838fdaf16c7bb403dbae5e6183b5c5e73badf01349eee4673de0499
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.0 MB (412995784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17125c95505cb428b4f1dd82f3cd94a5094219132a7ee57a763e28c703adf5d4`
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
# Tue, 12 Sep 2023 12:08:55 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 12 Sep 2023 12:08:55 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 12 Sep 2023 12:09:06 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.10.1-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.10.1 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 12 Sep 2023 12:09:06 GMT
WORKDIR /usr/share/logstash
# Tue, 12 Sep 2023 12:09:06 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Sep 2023 12:09:06 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Sep 2023 12:09:06 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 12 Sep 2023 12:09:06 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 12 Sep 2023 12:09:06 GMT
COPY config/log4j2.properties config/ # buildkit
# Tue, 12 Sep 2023 12:09:06 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Tue, 12 Sep 2023 12:09:06 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 12 Sep 2023 12:09:06 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 12 Sep 2023 12:09:06 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 12 Sep 2023 12:09:06 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 12 Sep 2023 12:09:06 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 12 Sep 2023 12:09:06 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 12 Sep 2023 12:09:06 GMT
USER 1000
# Tue, 12 Sep 2023 12:09:06 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 12 Sep 2023 12:09:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.10.1 org.opencontainers.image.version=8.10.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-09-12T11:53:47+00:00 org.opencontainers.image.created=2023-09-12T11:53:47+00:00
# Tue, 12 Sep 2023 12:09:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff9bb460b8bcf00f2cf3600cbaaec96ea32849002aa1c0472c1dc431667aa4e`  
		Last Modified: Tue, 19 Sep 2023 23:42:04 GMT  
		Size: 36.2 MB (36175687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eec45aed11f6657b16cc18bab678979102e5b345a249e58f0dab80e7bfb8904`  
		Last Modified: Tue, 19 Sep 2023 23:41:59 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa59f9c9bc6a8dc906451ac6e14f90c5ca6a8804ddd3a41e2dfc0da936df8e3`  
		Last Modified: Tue, 19 Sep 2023 23:42:20 GMT  
		Size: 347.9 MB (347878216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dcb9d16e75e3258ea3b05c9e26e027fb17e2124481d29189152e7ea82bc332`  
		Last Modified: Tue, 19 Sep 2023 23:41:59 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71353a233bf1863e517c4313b239aa317ebe9014ed6a2936d846f0bb7e391c67`  
		Last Modified: Tue, 19 Sep 2023 23:41:59 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ca263bff1dc5d1c5984a37a8cfb06b7154feb073cf61860070d3abf83c87a3`  
		Last Modified: Tue, 19 Sep 2023 23:41:58 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a977c22bbf5d91b94984af5632a661137e2e712a771c0bc565c9d506488fc3`  
		Last Modified: Tue, 19 Sep 2023 23:41:56 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f296c60c822257403864de90d53c8c6915d6408e54e9892e76cd1e3772ab1b90`  
		Last Modified: Tue, 19 Sep 2023 23:41:56 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc393f8d7e86a5e398b5ad79ade76729c70f05873f24038f7702d17653c00171`  
		Last Modified: Tue, 19 Sep 2023 23:41:56 GMT  
		Size: 3.7 KB (3664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7d6f4bc9c570dd746aac95dd1ab123af3095e77ed07e25a724d0c74e4c2c49`  
		Last Modified: Tue, 19 Sep 2023 23:41:57 GMT  
		Size: 1.7 MB (1731563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8b41319e5320bc2cb3110a2b50b521649e451cb690d4cb9741b896b227b84e`  
		Last Modified: Tue, 19 Sep 2023 23:41:56 GMT  
		Size: 714.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8b41319e5320bc2cb3110a2b50b521649e451cb690d4cb9741b896b227b84e`  
		Last Modified: Tue, 19 Sep 2023 23:41:56 GMT  
		Size: 714.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
