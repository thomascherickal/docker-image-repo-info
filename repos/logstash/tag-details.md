<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:7.17.16`](#logstash71716)
-	[`logstash:8.11.2`](#logstash8112)
-	[`logstash:8.11.3`](#logstash8113)

## `logstash:7.17.16`

```console
$ docker pull logstash@sha256:3e55610105f90416de30aca8ffdd767cd48185dfbf73df2a69d0b45d98e5e812
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
$ docker pull logstash@sha256:3c7893c93002e50310c5acf7e4b2983079b891c7e4d3adf246742b8641c6062f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.9 MB (433917486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ea72410b1c8cf671b08f81e0d0734da54d7c0cfed50c503394cf8c2934d130b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
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
	-	`sha256:dae58cbd668a05adbb25fa9970bfa041b807c2c537b86caa4ab74f77cfac02df`  
		Last Modified: Tue, 28 Nov 2023 05:37:25 GMT  
		Size: 26.0 MB (25975507 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:483023149b3e363410a4efa610382d9c1895c71ab225b1e3aeb1f58abbe3d12d`  
		Last Modified: Tue, 12 Dec 2023 17:43:18 GMT  
		Size: 42.5 MB (42496582 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97cb2de4e64897810ce7b16621b7ce7c9e83e9fcc5599d663460bc239058b036`  
		Last Modified: Tue, 12 Dec 2023 17:43:15 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2086a6382fdeb8710207fdb04b13c7c09acbedaaf88f3df1879a95f5c3cea565`  
		Last Modified: Thu, 14 Dec 2023 20:12:37 GMT  
		Size: 363.6 MB (363596021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e7fc2a73197dafd060a0b3b7619c1f3e711b02322609ed18fff7afaa062d3d3`  
		Last Modified: Thu, 14 Dec 2023 20:12:30 GMT  
		Size: 382.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f633f517c2366bef438309b7389ad8d821f351049f5f55d3e1f8e8ce8f77491a`  
		Last Modified: Thu, 14 Dec 2023 20:12:30 GMT  
		Size: 280.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf23d8b2254b754b8574ac5d934b117f2589eed8783289eaecfe08cc42bc111a`  
		Last Modified: Thu, 14 Dec 2023 20:12:30 GMT  
		Size: 476.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b5d6774bb58633b73bee0321f6a6763109c8e0b960231ed7da1143019f0bb3bb`  
		Last Modified: Thu, 14 Dec 2023 20:12:31 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4090904a81160ab5c863d9db5ed52a4c2bbc9446b8bf349ba49aedd752231876`  
		Last Modified: Thu, 14 Dec 2023 20:12:31 GMT  
		Size: 829.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b4ed7989161619758c4ac6a9b88ac4c980ee81942740394c0b0828ceeb80037`  
		Last Modified: Thu, 14 Dec 2023 20:12:32 GMT  
		Size: 1.8 MB (1844766 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4622af1cdcd1ad1fa574aff2ce1ae2f642d84f63c9968b911e0735acb0d75352`  
		Last Modified: Thu, 14 Dec 2023 20:12:32 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `logstash:7.17.16` - unknown; unknown

```console
$ docker pull logstash@sha256:62109d774139f1d5fd87be017c8f501c4055353d8f65d7a5e54616f90d0d623c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2705711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eaa3597438d4503bb6be7f1701de35cb320849525824ab71cedfe21968d46ab`

```dockerfile
```

-	Layers:
	-	`sha256:f42858484f101c5e24ae864a4c3c494ab17307b126300f4e0acdf26a4754aab9`  
		Last Modified: Thu, 14 Dec 2023 20:12:30 GMT  
		Size: 2.7 MB (2673699 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9f40c7e65737392e0cb3c519ca403bfc1b9332258c78a6794546dfefc5713825`  
		Last Modified: Thu, 14 Dec 2023 20:12:30 GMT  
		Size: 32.0 KB (32012 bytes)  
		MIME: application/vnd.in-toto+json

## `logstash:8.11.2`

```console
$ docker pull logstash@sha256:afc9186bf503d4858f0f72e79b8ae5b563d76058c87914892ef02dd6e9e3571f
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
$ docker pull logstash@sha256:034f9cfffcd468f72deea927ee0d7865c1fe078a03b11dfdf7593b0195d9146b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.7 MB (419663568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4aebc00cd8b407cb256130d221d04aadca01a468f6c1e1dcb8524a25064e101`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
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
	-	`sha256:dae58cbd668a05adbb25fa9970bfa041b807c2c537b86caa4ab74f77cfac02df`  
		Last Modified: Tue, 28 Nov 2023 05:37:25 GMT  
		Size: 26.0 MB (25975507 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:483023149b3e363410a4efa610382d9c1895c71ab225b1e3aeb1f58abbe3d12d`  
		Last Modified: Tue, 12 Dec 2023 17:43:18 GMT  
		Size: 42.5 MB (42496582 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97cb2de4e64897810ce7b16621b7ce7c9e83e9fcc5599d663460bc239058b036`  
		Last Modified: Tue, 12 Dec 2023 17:43:15 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d2940e9675cc166deaabc968796424a5dddc67a63631e4e3108fe406031d838`  
		Last Modified: Thu, 14 Dec 2023 20:11:27 GMT  
		Size: 349.3 MB (349339413 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61dce82e32df43c373acc6597452e7b088511fd3e25a9f576abf19876a58d384`  
		Last Modified: Thu, 14 Dec 2023 20:11:18 GMT  
		Size: 378.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:23aa5993b12bec24e35a11dce53ac03c0983a65c9cc6a83763e09f2cf76ecb62`  
		Last Modified: Thu, 14 Dec 2023 20:11:18 GMT  
		Size: 276.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6aae14061e17100ceaa71115597eb771c2b1f597a7ac6c653de8df53a08781ff`  
		Last Modified: Thu, 14 Dec 2023 20:11:18 GMT  
		Size: 471.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:24c37af170d2b17d6ec0bb26bcacc883ab05a30fe6a053099b8415c1ae14901a`  
		Last Modified: Thu, 14 Dec 2023 20:11:19 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e92b81871162e7472a406b2eee18aed95f0918488c0e3428b1fe26df0851807e`  
		Last Modified: Thu, 14 Dec 2023 20:11:19 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:233d39a7f43e1030cf62ff58b257bc2a2ca0d85f4142f6c856f34483997ab1d9`  
		Last Modified: Thu, 14 Dec 2023 20:11:19 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f84adbe17068ac59d3977fe362d037b24073c27c16fa405df657d2bbd2ead5b`  
		Last Modified: Thu, 14 Dec 2023 20:11:20 GMT  
		Size: 1.8 MB (1844955 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c3280d62a08c5c2e9f03f8f3e431e0e3f3834d7d77ad942900a54bfd0e66c39`  
		Last Modified: Thu, 14 Dec 2023 20:11:20 GMT  
		Size: 711.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `logstash:8.11.2` - unknown; unknown

```console
$ docker pull logstash@sha256:a2d90645fb905894f1173dcfbce64633969affe9d7e36786b7bed80b7656dab7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2834769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ec08b445ebbd13688f04f291a71baa745807fdd748c37b50166f0fbc1a99a59`

```dockerfile
```

-	Layers:
	-	`sha256:9f306e3d02da7db4163e267e5f010fb18da4d70531c7c084dc5b3a93bf0b9089`  
		Last Modified: Thu, 14 Dec 2023 20:11:19 GMT  
		Size: 2.8 MB (2800229 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bcba072ec261f297154b9e8155222daaa79aa2fcb2a2158816130b480d55f43b`  
		Last Modified: Thu, 14 Dec 2023 20:11:18 GMT  
		Size: 34.5 KB (34540 bytes)  
		MIME: application/vnd.in-toto+json

## `logstash:8.11.3`

```console
$ docker pull logstash@sha256:bc7739a1190e819eca175561efe019d260b8ea598334e1f024bde7cc948428cf
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
$ docker pull logstash@sha256:d7007e6fe7cd6b973feb7bb4fd5cbe3281a1a44941f02ac1367a738926ee3beb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.1 MB (422053703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9fba0f63519f9b5af1a5e959584029274e5c857788dfb5cd2f9329f6ff097d1`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
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
	-	`sha256:dae58cbd668a05adbb25fa9970bfa041b807c2c537b86caa4ab74f77cfac02df`  
		Last Modified: Tue, 28 Nov 2023 05:37:25 GMT  
		Size: 26.0 MB (25975507 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:483023149b3e363410a4efa610382d9c1895c71ab225b1e3aeb1f58abbe3d12d`  
		Last Modified: Tue, 12 Dec 2023 17:43:18 GMT  
		Size: 42.5 MB (42496582 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97cb2de4e64897810ce7b16621b7ce7c9e83e9fcc5599d663460bc239058b036`  
		Last Modified: Tue, 12 Dec 2023 17:43:15 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:229c8f20624824f07558822e35ce497a57ee6a8cd8848c58ddd3948670149ec2`  
		Last Modified: Thu, 14 Dec 2023 19:59:12 GMT  
		Size: 351.7 MB (351729537 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc9246513b637a4ecd7f593d289f8bee5d6275a8dd44c9f22ae8474f40810524`  
		Last Modified: Thu, 14 Dec 2023 19:59:04 GMT  
		Size: 381.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:60741e70fd2a3e31df5a35b95269fcfa540e9d81686e2b385c5d5aa19284ba0b`  
		Last Modified: Thu, 14 Dec 2023 19:59:04 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:02b2437fec7dea5b5fcf0edaa736394f54c75a4183fbbbe1c5dc4e8e8b91e414`  
		Last Modified: Thu, 14 Dec 2023 19:59:04 GMT  
		Size: 476.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4d889c32ddbf6bf4dfe9905d9bf016a5423a25697b80fbcdf86e6b67938820ed`  
		Last Modified: Thu, 14 Dec 2023 19:59:05 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f825a5ce7589c5a3b5cbe2a7d265323c7734cd4edaa9a453c8b99af54ab27b2d`  
		Last Modified: Thu, 14 Dec 2023 19:59:05 GMT  
		Size: 279.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b2a2507bcbbb6c588dafb91a16eb9df7bc2f507569d6b9b64e5139ab256b03f`  
		Last Modified: Thu, 14 Dec 2023 19:59:05 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0478def58651d86055a555971c4e72b55991963108d4397cf5727399e11d3c3`  
		Last Modified: Thu, 14 Dec 2023 19:59:07 GMT  
		Size: 1.8 MB (1844953 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:24a9e29c8c4e7d948b84d2510f02f67d650b7f34d200b9894232096529077262`  
		Last Modified: Thu, 14 Dec 2023 19:59:07 GMT  
		Size: 710.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `logstash:8.11.3` - unknown; unknown

```console
$ docker pull logstash@sha256:47382f920604306a8a633a4eed9f28507f23869073f5754bcf865f90cda86d78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2831515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:148fd7dd8c445d51d30f037a55c7a20d16050369f578362e7f1354e3f1513cea`

```dockerfile
```

-	Layers:
	-	`sha256:82c5fbd474b522bbca5a1190da400c8aed18b87a7dba43d91f38fe2844eceee9`  
		Last Modified: Thu, 14 Dec 2023 19:59:04 GMT  
		Size: 2.8 MB (2796973 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3640b5120cc84a2988445504b6e70db1668dfcdae189044a76efde75423b2be3`  
		Last Modified: Thu, 14 Dec 2023 19:59:04 GMT  
		Size: 34.5 KB (34542 bytes)  
		MIME: application/vnd.in-toto+json
