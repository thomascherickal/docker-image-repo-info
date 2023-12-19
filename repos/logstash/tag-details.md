<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:7.17.16`](#logstash71716)
-	[`logstash:8.11.2`](#logstash8112)
-	[`logstash:8.11.3`](#logstash8113)

## `logstash:7.17.16`

```console
$ docker pull logstash@sha256:fe1d1deae29a50f4debff76f3cc5c35e38e0a1ec85a969e09edffd9b6b44b884
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `logstash:7.17.16` - linux; amd64

```console
$ docker pull logstash@sha256:5697365f635b36c9e1d31e7e9f2267f68f00fc4f043993f24119b56bfeae4ffd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **442.5 MB (442459266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f57c02986aff5a07aefeec38cb21cdcc2fc547cf8638bb8cd3da721616a069f7`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 12 Dec 2023 12:49:29 GMT
ARG RELEASE
# Tue, 12 Dec 2023 12:49:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 12:49:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 12:49:29 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 12 Dec 2023 12:49:29 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Tue, 12 Dec 2023 12:49:29 GMT
CMD ["/bin/bash"]
# Tue, 12 Dec 2023 12:49:29 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN curl -Lo - https://artifacts.elastic.co/downloads/logstash/logstash-7.17.16-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.16 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
WORKDIR /usr/share/logstash
# Tue, 12 Dec 2023 12:49:29 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Dec 2023 12:49:29 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2023 12:49:29 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ADD config/log4j2.properties config/ # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 12 Dec 2023 12:49:29 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
USER 1000
# Tue, 12 Dec 2023 12:49:29 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 12 Dec 2023 12:49:29 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.16 org.opencontainers.image.version=7.17.16 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-12-05T12:24:52+00:00 org.opencontainers.image.created=2023-12-05T12:24:52+00:00
# Tue, 12 Dec 2023 12:49:29 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:527f5363b98e562da03d2e0bbf86fd7c34f487bffd9b27a3cf0a9afea2f0ee1f`  
		Last Modified: Wed, 13 Dec 2023 10:48:59 GMT  
		Size: 27.5 MB (27512774 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b06c5dca594470c89da01558ef1c3de546a60c9b4bf8179cf3c8855e2a8fe0d`  
		Last Modified: Sat, 16 Dec 2023 10:50:16 GMT  
		Size: 46.2 MB (46236266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9fc64dced61e148e93c0c7bc3d0fa499c02a461d2bbaa41210c75b0a827a9190`  
		Last Modified: Sat, 16 Dec 2023 10:50:14 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bd5f9ac6c993a06ad6f4467fd99e7e1ea1bd8a1f9969197fe941f984130ba71`  
		Last Modified: Sat, 16 Dec 2023 10:50:23 GMT  
		Size: 366.9 MB (366860871 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb35e856eef4d12e6be07a3e9e2c2d2ee962f716b571373ea972848c1c633d94`  
		Last Modified: Sat, 16 Dec 2023 10:50:14 GMT  
		Size: 379.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a99d48d7debcb2279967b1bb6d73ec18fb0e4e83ff06ca7935cb8b03d26799e5`  
		Last Modified: Sat, 16 Dec 2023 10:50:15 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0cd3c458bb3eef6b4aebe4144ea8284acde0f9ef48f41f21801b2442575f641`  
		Last Modified: Sat, 16 Dec 2023 10:50:15 GMT  
		Size: 473.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c371eb5570bb1f91b520ff2dbe59a2fd14bf2ff2670058acbaa3670ccb7f7f03`  
		Last Modified: Sat, 16 Dec 2023 10:50:16 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:02c83485e548a3c4d434ee54e21db841aa69db40cdd42044f35133f38aa86994`  
		Last Modified: Sat, 16 Dec 2023 10:50:16 GMT  
		Size: 826.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024c092c7c3ed11178281002b921000945aaaa0004f4f35718b3c6e3dd3f574c`  
		Last Modified: Sat, 16 Dec 2023 10:50:18 GMT  
		Size: 1.8 MB (1844765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ecfc37efa4bc959f0d2daa2f26ff99e19c3ed9fce8d6552297cc66880773d6a2`  
		Last Modified: Sat, 16 Dec 2023 10:50:17 GMT  
		Size: 489.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `logstash:7.17.16` - unknown; unknown

```console
$ docker pull logstash@sha256:2a6733630283a591b0502401da03d91b0cf899a4ba479c986ed11cb0903e52c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2705540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b74c3405ded8f97331269df58cf00fc83ab26ea35bab252979961c449e142a8d`

```dockerfile
```

-	Layers:
	-	`sha256:f9311f864e03030450bad3c70ae5e3ceee348a696c6897da5adc53c4923b8b68`  
		Last Modified: Sat, 16 Dec 2023 10:50:14 GMT  
		Size: 2.7 MB (2673371 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:971351e1ea36e7785ff28f24b50d32219498e73560afdecefae4d118cad5e303`  
		Last Modified: Sat, 16 Dec 2023 10:50:14 GMT  
		Size: 32.2 KB (32169 bytes)  
		MIME: application/vnd.in-toto+json

### `logstash:7.17.16` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:dfe5734a8fca811c6ff3dfbd8ac8a599e2d3664d09f23e8bebdd4a593c67f34b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.2 MB (428156580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0f738760390b11e732b615d6fd436c81f368db0a87da75034bfb02810424a37`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 12 Dec 2023 12:49:29 GMT
ARG RELEASE
# Tue, 12 Dec 2023 12:49:29 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 12:49:29 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 12:49:29 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 12 Dec 2023 12:49:29 GMT
ADD file:9ec8b7bbb2fbc8c90f1f24e19ab22130e03be1cc4727459e1265d2ed652377a1 in / 
# Tue, 12 Dec 2023 12:49:29 GMT
CMD ["/bin/bash"]
# Tue, 12 Dec 2023 12:49:29 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN curl -Lo - https://artifacts.elastic.co/downloads/logstash/logstash-7.17.16-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.16 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
WORKDIR /usr/share/logstash
# Tue, 12 Dec 2023 12:49:29 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Dec 2023 12:49:29 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2023 12:49:29 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ADD config/log4j2.properties config/ # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 12 Dec 2023 12:49:29 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 12 Dec 2023 12:49:29 GMT
USER 1000
# Tue, 12 Dec 2023 12:49:29 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 12 Dec 2023 12:49:29 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.16 org.opencontainers.image.version=7.17.16 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-12-05T12:24:52+00:00 org.opencontainers.image.created=2023-12-05T12:24:52+00:00
# Tue, 12 Dec 2023 12:49:29 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:d519a3a2a796a075e4e40e5c4a1513aa8db8f8fdf009662bf6858f0149143b28`  
		Last Modified: Wed, 13 Dec 2023 10:49:05 GMT  
		Size: 26.0 MB (25974768 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:92a1e7d71d662fea3176db34f01e2afb22468596910909062e42889cb2be6766`  
		Last Modified: Mon, 18 Dec 2023 19:59:02 GMT  
		Size: 36.7 MB (36736504 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d28fe55da162ade1eb87e2a8e5383c00e22edf99c2e9c1f861f35bb42281cdd2`  
		Last Modified: Mon, 18 Dec 2023 19:59:01 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:763ff03f781408581c158b36cbaabb08084f15719491190e4d1a0178688ea1af`  
		Last Modified: Mon, 18 Dec 2023 20:00:06 GMT  
		Size: 363.6 MB (363595954 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73e6080b79db201b78a9f1499a15560bee1ead79dae310acc08d41f9290aab22`  
		Last Modified: Mon, 18 Dec 2023 19:59:56 GMT  
		Size: 377.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70ec27b3e010a35ca3ae47a54c0c74d658732caf84c6dcc70d9e980170467a9e`  
		Last Modified: Mon, 18 Dec 2023 19:59:56 GMT  
		Size: 275.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f7fcb35737917972d4681a08acade07b83888badd66f22b9624ea452b1e991c3`  
		Last Modified: Mon, 18 Dec 2023 19:59:56 GMT  
		Size: 471.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f2515a6be9a79f59c9566f5317225e36e1bcc180fce88cc33e23982a2e059f0c`  
		Last Modified: Mon, 18 Dec 2023 19:59:57 GMT  
		Size: 276.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db0334396271f019408d440d907d6b1d8a8d88adf9faf1a9716278ff13cc9a8b`  
		Last Modified: Mon, 18 Dec 2023 19:59:57 GMT  
		Size: 827.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a2e20ebe92786ad0673efda66170ca76ee31ef8b81ab4eed26aeaad5b3fbdfc`  
		Last Modified: Mon, 18 Dec 2023 19:59:57 GMT  
		Size: 1.8 MB (1844765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b6463a73bcc880680060e5e7f9a12b8b4aefdfd09007be757af8cabcc2e5caf`  
		Last Modified: Mon, 18 Dec 2023 19:59:58 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `logstash:7.17.16` - unknown; unknown

```console
$ docker pull logstash@sha256:bea08338d34323b0e4097cff57bfb59352b4c3b672af921240c9548914497227
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2705711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4bb68aedeb5395bd12ccbb27a6130d8310542a05f8cf0f87c727c1cd74c6c53`

```dockerfile
```

-	Layers:
	-	`sha256:30dbb673facae481ed3d31e45475149fc89b00e089dc3059d90bfdacf302bc09`  
		Last Modified: Mon, 18 Dec 2023 19:59:56 GMT  
		Size: 2.7 MB (2673699 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:92abafc051904fcf46bbdbd53611db70acb224d076124f633e8535f8903e31fd`  
		Last Modified: Mon, 18 Dec 2023 19:59:56 GMT  
		Size: 32.0 KB (32012 bytes)  
		MIME: application/vnd.in-toto+json

## `logstash:8.11.2`

```console
$ docker pull logstash@sha256:8bdb3dd3806fbc8404c70ce0cb6f124918a8ae05983a16045fc60b8d877d32eb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `logstash:8.11.2` - linux; amd64

```console
$ docker pull logstash@sha256:de0b0e4e49f36872cf8e56298f0f3a171b058aa63fd0331982e300e26e414e31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.1 MB (426125568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f086cdeef5e2d496535426e77f01971cddc99f8aa72f7acf40fa7f1a5b3b53`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Thu, 07 Dec 2023 12:34:16 GMT
ARG RELEASE
# Thu, 07 Dec 2023 12:34:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 07 Dec 2023 12:34:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 07 Dec 2023 12:34:16 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 07 Dec 2023 12:34:16 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Thu, 07 Dec 2023 12:34:16 GMT
CMD ["/bin/bash"]
# Thu, 07 Dec 2023 12:34:16 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN curl -Lo - https://artifacts.elastic.co/downloads/logstash/logstash-8.11.2-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.11.2 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
WORKDIR /usr/share/logstash
# Thu, 07 Dec 2023 12:34:16 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 07 Dec 2023 12:34:16 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Dec 2023 12:34:16 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY config/log4j2.properties config/ # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Thu, 07 Dec 2023 12:34:16 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
USER 1000
# Thu, 07 Dec 2023 12:34:16 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Thu, 07 Dec 2023 12:34:16 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.11.2 org.opencontainers.image.version=8.11.2 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-12-05T12:30:34+00:00 org.opencontainers.image.created=2023-12-05T12:30:34+00:00
# Thu, 07 Dec 2023 12:34:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:527f5363b98e562da03d2e0bbf86fd7c34f487bffd9b27a3cf0a9afea2f0ee1f`  
		Last Modified: Wed, 13 Dec 2023 10:48:59 GMT  
		Size: 27.5 MB (27512774 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:543e98561526fda3befdacdbf5ff0dd8b1e5f9025f9215ac70ca9961d8d41a67`  
		Last Modified: Sat, 16 Dec 2023 10:49:56 GMT  
		Size: 46.2 MB (46236418 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:763bbf3dfb824d729a8f784ae8dd99a4579f8c794d05972945d1521d03cc571e`  
		Last Modified: Sat, 16 Dec 2023 10:49:54 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7bcbcd5d9fe9e1ecefacc653ed3d541b9737ada55a436418d5a41c06fb87013b`  
		Last Modified: Sat, 16 Dec 2023 10:50:03 GMT  
		Size: 350.5 MB (350524324 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a60185bc5810485cf6b79573f7bf4248012c71bc29f664b049f0603124104e2`  
		Last Modified: Sat, 16 Dec 2023 10:49:54 GMT  
		Size: 377.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a809c91b00f4a206bd3967cc1f7541e2fcda853eba1a5cef7b6a3aba64f070c`  
		Last Modified: Sat, 16 Dec 2023 10:49:55 GMT  
		Size: 275.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19989780c2ff2e732391d7326dec3a2ef7291987a7d477714e6af96a66a093c8`  
		Last Modified: Sat, 16 Dec 2023 10:49:55 GMT  
		Size: 470.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f9bef1982ecb9f79d304cdc4f77fea46e2a298636749781c495618cb17b42be7`  
		Last Modified: Sat, 16 Dec 2023 10:49:56 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59473bc4eb8a2f7aa9002565174a44a3329e8953af22a02db808ce4f16a57b13`  
		Last Modified: Sat, 16 Dec 2023 10:49:57 GMT  
		Size: 276.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e44e1aa40c898aef002c7cd3f2f02f4f3176f2e3e3bf41915ae8a54c66a69512`  
		Last Modified: Sat, 16 Dec 2023 10:49:57 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d1394d810477ae5b0d54beba2689364fb0f792e43bf61ce869e094b796c9b35c`  
		Last Modified: Sat, 16 Dec 2023 10:49:58 GMT  
		Size: 1.8 MB (1844956 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67c3d37eb4a8e0125a884630c23f75d38010568205b682689df1fe2fb2d22868`  
		Last Modified: Sat, 16 Dec 2023 10:49:58 GMT  
		Size: 712.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `logstash:8.11.2` - unknown; unknown

```console
$ docker pull logstash@sha256:819f6b49b11d926808afb65dfa950fc26e1ecf75e7134d302f9e7713a9e73df8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2834595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b1c9c3d4916b115dd2994bdd17fcff249c6593135369017b8784393f2d2ac80`

```dockerfile
```

-	Layers:
	-	`sha256:9070d07e2e81082e70086c5c2fa0d9c8451bec54c86129db50c25b1517acd9c9`  
		Last Modified: Sat, 16 Dec 2023 10:49:55 GMT  
		Size: 2.8 MB (2799896 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3119511e8522151956a21118205ad6da260fa5397ecdf477db35977adc59e0d0`  
		Last Modified: Sat, 16 Dec 2023 10:49:54 GMT  
		Size: 34.7 KB (34699 bytes)  
		MIME: application/vnd.in-toto+json

### `logstash:8.11.2` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:b868b0780ef40e75d86f70611e9380cf53c2cebf2ff04cbb8c7fa56b48cdef1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.9 MB (413903176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1c9700b3c526f11beb9436ad7207cfa2c84cce8d312f84d29eb02fbec6de20b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Thu, 07 Dec 2023 12:34:16 GMT
ARG RELEASE
# Thu, 07 Dec 2023 12:34:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 07 Dec 2023 12:34:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 07 Dec 2023 12:34:16 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 07 Dec 2023 12:34:16 GMT
ADD file:9ec8b7bbb2fbc8c90f1f24e19ab22130e03be1cc4727459e1265d2ed652377a1 in / 
# Thu, 07 Dec 2023 12:34:16 GMT
CMD ["/bin/bash"]
# Thu, 07 Dec 2023 12:34:16 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN curl -Lo - https://artifacts.elastic.co/downloads/logstash/logstash-8.11.2-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.11.2 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
WORKDIR /usr/share/logstash
# Thu, 07 Dec 2023 12:34:16 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 07 Dec 2023 12:34:16 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 07 Dec 2023 12:34:16 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY config/log4j2.properties config/ # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Thu, 07 Dec 2023 12:34:16 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Thu, 07 Dec 2023 12:34:16 GMT
USER 1000
# Thu, 07 Dec 2023 12:34:16 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Thu, 07 Dec 2023 12:34:16 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.11.2 org.opencontainers.image.version=8.11.2 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-12-05T12:30:34+00:00 org.opencontainers.image.created=2023-12-05T12:30:34+00:00
# Thu, 07 Dec 2023 12:34:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:d519a3a2a796a075e4e40e5c4a1513aa8db8f8fdf009662bf6858f0149143b28`  
		Last Modified: Wed, 13 Dec 2023 10:49:05 GMT  
		Size: 26.0 MB (25974768 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:92a1e7d71d662fea3176db34f01e2afb22468596910909062e42889cb2be6766`  
		Last Modified: Mon, 18 Dec 2023 19:59:02 GMT  
		Size: 36.7 MB (36736504 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d28fe55da162ade1eb87e2a8e5383c00e22edf99c2e9c1f861f35bb42281cdd2`  
		Last Modified: Mon, 18 Dec 2023 19:59:01 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc2801d83d065317eca4830cb6367d3df894be0ba34103624e3e173f064c21a`  
		Last Modified: Mon, 18 Dec 2023 19:59:38 GMT  
		Size: 349.3 MB (349339834 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a3c18d16c00a9e87d2920d14bcc29f37fae8eea62610b1dcba351635062f02d`  
		Last Modified: Mon, 18 Dec 2023 19:59:31 GMT  
		Size: 378.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e9f6960bcb42a7dfebd7a56b2384a49e97ab885b9dad887b3ef4c4c3caa23bad`  
		Last Modified: Mon, 18 Dec 2023 19:59:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbe5657d1421d9ccabd8f99dcd12d57c2a8e2158c5269dc468eba337ec3303ff`  
		Last Modified: Mon, 18 Dec 2023 19:59:31 GMT  
		Size: 473.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce52fc36bee71f89504e31480a44f8d2df4376c2414b9fbe9af757e54511b5b6`  
		Last Modified: Mon, 18 Dec 2023 19:59:31 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eee4daeb148561e470c22722241374b9c4409cad1eb38600b98c74c8cdc01c29`  
		Last Modified: Mon, 18 Dec 2023 19:59:32 GMT  
		Size: 279.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de234fda40e4e5a5f2929389795faddfe22d4088f63c4657bf50a514c98d24bb`  
		Last Modified: Mon, 18 Dec 2023 19:59:32 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e462ad0a793d906ba6dec2138d5b20a59bf002aa3d3060e421d109b605c39bc`  
		Last Modified: Mon, 18 Dec 2023 19:59:33 GMT  
		Size: 1.8 MB (1844956 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:87806073249c6c952d8ad1e1abe6cc3072e0091c845fe891984b658595979b21`  
		Last Modified: Mon, 18 Dec 2023 19:59:33 GMT  
		Size: 713.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `logstash:8.11.2` - unknown; unknown

```console
$ docker pull logstash@sha256:c05620eb25177b58c3825b9855fcd9198583e54783ce7252223c05e94147a47f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2834770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfb99cdb1c88b745d5290ffffa78dd98f88a9d8ec5faf9fdecdd96c126602397`

```dockerfile
```

-	Layers:
	-	`sha256:fb66b03dfb355df038bace8c3775ca24420861cc36184c6d63eb14c54a8e90c4`  
		Last Modified: Mon, 18 Dec 2023 19:59:31 GMT  
		Size: 2.8 MB (2800229 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:32baf6bde323445ee22c7870f47a52cd4b9fe7a7b4d6fb6de781da83aeaf8b5f`  
		Last Modified: Mon, 18 Dec 2023 19:59:30 GMT  
		Size: 34.5 KB (34541 bytes)  
		MIME: application/vnd.in-toto+json

## `logstash:8.11.3`

```console
$ docker pull logstash@sha256:9ac3570f9be8a0923f216d3b41704cfa84453d8f0a043330343260bd6ea6fab4
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `logstash:8.11.3` - linux; amd64

```console
$ docker pull logstash@sha256:af928335fc3e94fa8b58570ea4d9d1760d0976579ea2ce51cfc6e3374245308f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.5 MB (428516099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97f65931a6d5987b992a1caaed093f3486dcc107eb5845e380b007594b3747b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 12 Dec 2023 13:07:20 GMT
ARG RELEASE
# Tue, 12 Dec 2023 13:07:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 13:07:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 13:07:20 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 12 Dec 2023 13:07:20 GMT
ADD file:5696198fbfd4074852bdee76ffd84da75da8de76727cef4f0cdd265f7bee6b76 in / 
# Tue, 12 Dec 2023 13:07:20 GMT
CMD ["/bin/bash"]
# Tue, 12 Dec 2023 13:07:20 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN curl -Lo - https://artifacts.elastic.co/downloads/logstash/logstash-8.11.3-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.11.3 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
WORKDIR /usr/share/logstash
# Tue, 12 Dec 2023 13:07:20 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Dec 2023 13:07:20 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2023 13:07:20 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY config/log4j2.properties config/ # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 12 Dec 2023 13:07:20 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
USER 1000
# Tue, 12 Dec 2023 13:07:20 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 12 Dec 2023 13:07:20 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.11.3 org.opencontainers.image.version=8.11.3 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-12-07T19:18:05+00:00 org.opencontainers.image.created=2023-12-07T19:18:05+00:00
# Tue, 12 Dec 2023 13:07:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:527f5363b98e562da03d2e0bbf86fd7c34f487bffd9b27a3cf0a9afea2f0ee1f`  
		Last Modified: Wed, 13 Dec 2023 10:48:59 GMT  
		Size: 27.5 MB (27512774 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e860362dda24bb73b9812e1ba87c995fbd2dcf115d1870a5016161497c44d3b7`  
		Last Modified: Sat, 16 Dec 2023 10:49:51 GMT  
		Size: 46.2 MB (46236364 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9d965837ac0cffddd2a209ec27a69500c9a50752a72a9c0e72bf2e2ac71d954`  
		Last Modified: Sat, 16 Dec 2023 10:49:50 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d08fd165304e4d79f08c527e0660b9451357def6367e4a9608eb439e026c342`  
		Last Modified: Sat, 16 Dec 2023 10:49:56 GMT  
		Size: 352.9 MB (352914899 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:812625dcebb88332e22dd76162ea063dd5afd32eea6570651f868c3d3ca8bd43`  
		Last Modified: Sat, 16 Dec 2023 10:49:50 GMT  
		Size: 381.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa2615151308f1edd9f54ba93a48ad9229f8d58c58b82c34d8158d764bb11343`  
		Last Modified: Sat, 16 Dec 2023 10:49:51 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:191fc48743106554f0e8df902cb4d05169b4d26debc62a6d7145586a5421a9af`  
		Last Modified: Sat, 16 Dec 2023 10:49:50 GMT  
		Size: 473.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:182d2c952bd8e74ed568d0e515ff0f65a007e86f2b05548ba4481aa952fc267c`  
		Last Modified: Sat, 16 Dec 2023 10:49:51 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7bdbeef45ae1afc651980f434989688da2af980d7ea28485f5d0307274bb562c`  
		Last Modified: Sat, 16 Dec 2023 10:49:52 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc28c82e972a03fdba8ae8d04c0155f12968651d990a03d69570ffef874f7944`  
		Last Modified: Sat, 16 Dec 2023 10:49:52 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d07034579b035959365698298bf0378330d67bf83e4116224783c2b6e37d2dae`  
		Last Modified: Sat, 16 Dec 2023 10:49:52 GMT  
		Size: 1.8 MB (1844951 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2023bec0b2c02ddbed8c4fd520a7757ed53826f98b015b40d625cff39c7796d8`  
		Last Modified: Sat, 16 Dec 2023 10:49:53 GMT  
		Size: 711.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `logstash:8.11.3` - unknown; unknown

```console
$ docker pull logstash@sha256:e7f9d7a1301a548cb090361859c58c08ac6d531bed37ffceebc8b6aedf6d1679
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2831339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da91743bd47c6d195d3f3fc6686f7e6ed1071441ff69d295e0f149dd214cf45`

```dockerfile
```

-	Layers:
	-	`sha256:0eb8be3c997531ad5c14416bc8030056e5b1a3d100ebde0d4efd102fed10ab19`  
		Last Modified: Sat, 16 Dec 2023 10:49:50 GMT  
		Size: 2.8 MB (2796640 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d5b408a28fbad40a9608adf51153a1555947d97c4d0269851a4c654434adfec0`  
		Last Modified: Sat, 16 Dec 2023 10:49:50 GMT  
		Size: 34.7 KB (34699 bytes)  
		MIME: application/vnd.in-toto+json

### `logstash:8.11.3` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:9c1864a36cdd9715da02778188082097604cd391b7dc181543ae02773676fdbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.3 MB (416292598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef37300452cc0f4f77f3340fa4e3d631632e7256827fcfc3d020841b4e7527d5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 12 Dec 2023 13:07:20 GMT
ARG RELEASE
# Tue, 12 Dec 2023 13:07:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Dec 2023 13:07:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Dec 2023 13:07:20 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 12 Dec 2023 13:07:20 GMT
ADD file:9ec8b7bbb2fbc8c90f1f24e19ab22130e03be1cc4727459e1265d2ed652377a1 in / 
# Tue, 12 Dec 2023 13:07:20 GMT
CMD ["/bin/bash"]
# Tue, 12 Dec 2023 13:07:20 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN curl -Lo - https://artifacts.elastic.co/downloads/logstash/logstash-8.11.3-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.11.3 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
WORKDIR /usr/share/logstash
# Tue, 12 Dec 2023 13:07:20 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 12 Dec 2023 13:07:20 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Dec 2023 13:07:20 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY config/log4j2.properties config/ # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 12 Dec 2023 13:07:20 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 12 Dec 2023 13:07:20 GMT
USER 1000
# Tue, 12 Dec 2023 13:07:20 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 12 Dec 2023 13:07:20 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.11.3 org.opencontainers.image.version=8.11.3 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-12-07T19:18:05+00:00 org.opencontainers.image.created=2023-12-07T19:18:05+00:00
# Tue, 12 Dec 2023 13:07:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:d519a3a2a796a075e4e40e5c4a1513aa8db8f8fdf009662bf6858f0149143b28`  
		Last Modified: Wed, 13 Dec 2023 10:49:05 GMT  
		Size: 26.0 MB (25974768 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:92a1e7d71d662fea3176db34f01e2afb22468596910909062e42889cb2be6766`  
		Last Modified: Mon, 18 Dec 2023 19:59:02 GMT  
		Size: 36.7 MB (36736504 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d28fe55da162ade1eb87e2a8e5383c00e22edf99c2e9c1f861f35bb42281cdd2`  
		Last Modified: Mon, 18 Dec 2023 19:59:01 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c90c2809c8d1f41f2933e73506320c9b4bdd7040f6c2b3cfb50ba08c228740e`  
		Last Modified: Mon, 18 Dec 2023 19:59:10 GMT  
		Size: 351.7 MB (351729245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a604438b3916c7760a2e132d650a411f50996650d44bee74a3b1469651a625ad`  
		Last Modified: Mon, 18 Dec 2023 19:59:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2eb4d8d35e1b3dd6ddbcbdb6d1eef6a4aafd7f4b838efaf4e78f5861b9f1733`  
		Last Modified: Mon, 18 Dec 2023 19:59:02 GMT  
		Size: 279.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:46498d614f628cdb3a95306b9aeae4a28a7e1be79c8f4082576cb86bed407cdf`  
		Last Modified: Mon, 18 Dec 2023 19:59:02 GMT  
		Size: 476.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a773a0aa4f33bade95f7813105c885805c1c0506b6fd7dc5413cc36e06e66f8`  
		Last Modified: Mon, 18 Dec 2023 19:59:03 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17bc71ff54658535ac15120fdb7d4fac753fcc23228dcd098743c28b23bc2b69`  
		Last Modified: Mon, 18 Dec 2023 19:59:04 GMT  
		Size: 279.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:877b55cd8930b66a341e1487f07622d4361c30b9125cbec65dd0759efc94af8f`  
		Last Modified: Mon, 18 Dec 2023 19:59:04 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:10f57afd138c55d7ba70ff906dcf45e73481ace79d3d65b78d84a301d576b041`  
		Last Modified: Mon, 18 Dec 2023 19:59:05 GMT  
		Size: 1.8 MB (1844950 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d945665cf6fc5399385b995bb790efe1077b3d17833fe16f7301627cda89fff`  
		Last Modified: Mon, 18 Dec 2023 19:59:05 GMT  
		Size: 713.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `logstash:8.11.3` - unknown; unknown

```console
$ docker pull logstash@sha256:099b3fc482c611830a5dde116417923a55f1635ed82b638ba651e09eb615b99a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2831515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896a83ccf2ed40dc09d4ec55bb5ab081c0229bcb857796b88edb3c09ded45c29`

```dockerfile
```

-	Layers:
	-	`sha256:bf4a3c9abb0a36fb52da98a42d3c15452691d179ce17b41fe5050691d7f09fab`  
		Last Modified: Mon, 18 Dec 2023 19:59:01 GMT  
		Size: 2.8 MB (2796973 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c42ca490c54276f2d43bb4607f662d6bef3beb03a6ae8a315401cd901c7eeca5`  
		Last Modified: Mon, 18 Dec 2023 19:59:01 GMT  
		Size: 34.5 KB (34542 bytes)  
		MIME: application/vnd.in-toto+json
