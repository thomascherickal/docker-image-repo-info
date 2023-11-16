<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:7.17.15`](#logstash71715)
-	[`logstash:8.11.1`](#logstash8111)

## `logstash:7.17.15`

```console
$ docker pull logstash@sha256:6f27b139f4596e2d5dd0770a16dea4887bd7c50d4ce59ec3b3668b950c589828
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `logstash:7.17.15` - linux; amd64

```console
$ docker pull logstash@sha256:168daa053382d3cf35daefbc18fb3f2754a9c81c43f5c1bbdf80696b6f2797c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.1 MB (484134580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbbb30f0bc7d4c5344d23ba638d3e2ef63ad7d1fb2187a7cb250177e777b8e7`
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
# Tue, 10 Oct 2023 17:36:44 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Tue, 10 Oct 2023 17:36:44 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Tue, 10 Oct 2023 17:36:54 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.15-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.15 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash # buildkit
# Tue, 10 Oct 2023 17:36:54 GMT
WORKDIR /usr/share/logstash
# Tue, 10 Oct 2023 17:36:54 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 10 Oct 2023 17:36:54 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 10 Oct 2023 17:36:54 GMT
ADD config/pipelines.yml config/pipelines.yml # buildkit
# Tue, 10 Oct 2023 17:36:54 GMT
ADD config/logstash-full.yml config/logstash.yml # buildkit
# Tue, 10 Oct 2023 17:36:54 GMT
ADD config/log4j2.properties config/ # buildkit
# Tue, 10 Oct 2023 17:36:54 GMT
ADD pipeline/default.conf pipeline/logstash.conf # buildkit
# Tue, 10 Oct 2023 17:36:54 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Tue, 10 Oct 2023 17:36:54 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 10 Oct 2023 17:36:54 GMT
ADD env2yaml/env2yaml /usr/local/bin/ # buildkit
# Tue, 10 Oct 2023 17:36:54 GMT
ADD bin/docker-entrypoint /usr/local/bin/ # buildkit
# Tue, 10 Oct 2023 17:36:54 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Tue, 10 Oct 2023 17:36:54 GMT
USER 1000
# Tue, 10 Oct 2023 17:36:54 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Tue, 10 Oct 2023 17:36:54 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.15 org.opencontainers.image.version=7.17.15 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-10-10T17:27:06+00:00 org.opencontainers.image.created=2023-10-10T17:27:06+00:00
# Tue, 10 Oct 2023 17:36:54 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:f9175e7b73a4b948b4c5db289cbeeb1d8511aee675255978036e76ffeda560be`  
		Last Modified: Mon, 07 Aug 2023 21:55:17 GMT  
		Size: 31.8 MB (31795971 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:83ba9255ea2aad343648bfce8cedb7079e112b82eb5ef5fcb3b8b19fd90270ef`  
		Last Modified: Mon, 13 Nov 2023 18:04:34 GMT  
		Size: 55.1 MB (55136167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:705436fe590e46fb8189b17ac08352fe1eabf4dc3f1bdf414727f17a8d235654`  
		Last Modified: Mon, 13 Nov 2023 18:04:30 GMT  
		Size: 2.0 KB (2032 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fecdb2387d9514ddc6d1a62aa654835a75d17ae1c783fca40674f8629aa38e53`  
		Last Modified: Mon, 13 Nov 2023 18:04:42 GMT  
		Size: 395.2 MB (395247487 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89732bc7504122601f40269fc9ddfb70982e633ea9caf641ae45736f2846b004`  
		Last Modified: Sat, 26 Jan 2019 16:40:00 GMT  
		Size: 39.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce41a6cca7150d3d14b5399ab7ac67eccbd4f0ec8550b0ed9d0186cb6eff3d54`  
		Last Modified: Mon, 13 Nov 2023 18:04:30 GMT  
		Size: 401.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:11dfb55bc376e95df6e6e7fe87f10a49ad5b6be6b9b6ae108000ad38a638ead0`  
		Last Modified: Mon, 13 Nov 2023 18:04:32 GMT  
		Size: 296.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03495e4b508d64b04f81574b7e75b16563c1192e2fb5467d301d781b365812ba`  
		Last Modified: Mon, 13 Nov 2023 18:04:32 GMT  
		Size: 500.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47fd9ac414235fe90cc134b6011786b9be37b92b8459595ac6b3b2c0443e1417`  
		Last Modified: Mon, 13 Nov 2023 18:04:33 GMT  
		Size: 296.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8d86115a731fda7720afc093a8d9a25ba6db81271251178f8e281eafecd77ee0`  
		Last Modified: Mon, 13 Nov 2023 18:04:34 GMT  
		Size: 3.0 KB (3005 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ab26e9eb5b2014929b91e1f3403cafe5169defd7c92884259b268b6dc66556b`  
		Last Modified: Mon, 13 Nov 2023 18:04:35 GMT  
		Size: 1.9 MB (1947358 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5d91f872b892e3033a8cc9403bfb495143f37e433d1693c2c5c5478d3b78ba51`  
		Last Modified: Mon, 13 Nov 2023 18:04:35 GMT  
		Size: 514.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5d91f872b892e3033a8cc9403bfb495143f37e433d1693c2c5c5478d3b78ba51`  
		Last Modified: Mon, 13 Nov 2023 18:04:35 GMT  
		Size: 514.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `logstash:7.17.15` - unknown; unknown

```console
$ docker pull logstash@sha256:1fc891d6f12c3bfec7be2c651af3ca80617e07d4c1fd2cd063924bca12d99475
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 MB (2686905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77e1bd13a1ff50c059ce19e5978443d4435a4f00d928a382509e00c2c4451aea`

```dockerfile
```

-	Layers:
	-	`sha256:7c00e467f891a0d2fd06148da5f08986735ee1f9ff0f793bba67512638fb96d0`  
		Last Modified: Thu, 16 Nov 2023 01:20:28 GMT  
		Size: 2.7 MB (2678967 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4e311cbf19692f7df109cbdc47aa10ab71824d28122ac3eefae5c2fffaad344d`  
		Last Modified: Thu, 16 Nov 2023 01:20:27 GMT  
		Size: 7.9 KB (7938 bytes)  
		MIME: application/vnd.in-toto+json

## `logstash:8.11.1`

```console
$ docker pull logstash@sha256:c5355c121295d7380869df186de9b05d7fe1954302211e25ecb8af96c6fbc53b
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 2
	-	linux; amd64
	-	unknown; unknown

### `logstash:8.11.1` - linux; amd64

```console
$ docker pull logstash@sha256:9217b40ed71769101de0e7476f18f6c9f7f2be3989bd0ad312a2a8353f67183b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **460.0 MB (460018707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4482a4fdfada47597dfd616a737fba82d215553dcf765c7ddd905189c230d739`
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
# Sat, 11 Nov 2023 08:36:20 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code) # buildkit
# Sat, 11 Nov 2023 08:36:21 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash # buildkit
# Sat, 11 Nov 2023 08:36:30 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.11.1-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.11.1 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash # buildkit
# Sat, 11 Nov 2023 08:36:30 GMT
WORKDIR /usr/share/logstash
# Sat, 11 Nov 2023 08:36:30 GMT
ENV ELASTIC_CONTAINER=true
# Sat, 11 Nov 2023 08:36:30 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Nov 2023 08:36:30 GMT
COPY config/pipelines.yml config/pipelines.yml # buildkit
# Sat, 11 Nov 2023 08:36:30 GMT
COPY config/logstash-full.yml config/logstash.yml # buildkit
# Sat, 11 Nov 2023 08:36:30 GMT
COPY config/log4j2.properties config/ # buildkit
# Sat, 11 Nov 2023 08:36:30 GMT
COPY config/log4j2.file.properties config/ # buildkit
# Sat, 11 Nov 2023 08:36:30 GMT
COPY pipeline/default.conf pipeline/logstash.conf # buildkit
# Sat, 11 Nov 2023 08:36:30 GMT
RUN chown --recursive logstash:root config/ pipeline/ # buildkit
# Sat, 11 Nov 2023 08:36:30 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Sat, 11 Nov 2023 08:36:30 GMT
COPY env2yaml/env2yaml /usr/local/bin/ # buildkit
# Sat, 11 Nov 2023 08:36:30 GMT
COPY bin/docker-entrypoint /usr/local/bin/ # buildkit
# Sat, 11 Nov 2023 08:36:30 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint # buildkit
# Sat, 11 Nov 2023 08:36:30 GMT
USER 1000
# Sat, 11 Nov 2023 08:36:30 GMT
EXPOSE map[5044/tcp:{} 9600/tcp:{}]
# Sat, 11 Nov 2023 08:36:30 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.11.1 org.opencontainers.image.version=8.11.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2023-11-11T08:23:14+00:00 org.opencontainers.image.created=2023-11-11T08:23:14+00:00
# Sat, 11 Nov 2023 08:36:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:70db4e7a2af7f73b7cef95301fc20fbedcfe68e5fb874e2cfba0b5ae41a066ca`  
		Last Modified: Wed, 25 Oct 2023 11:40:40 GMT  
		Size: 31.8 MB (31790746 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:598118935314bc1e56ec60bf8aac967b2d0763d605dd5a42b2340ebb663c5bc6`  
		Last Modified: Mon, 13 Nov 2023 14:12:55 GMT  
		Size: 48.3 MB (48283281 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b3f9c3afc2f595e4ba1cf231b625f694df35276ef59e6c6d9701226d68711a4`  
		Last Modified: Mon, 13 Nov 2023 14:12:52 GMT  
		Size: 2.0 KB (2041 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e02795b6f169a879d82f4609c427b0dd95d939c7285d622ba39f882f6ea6b5a0`  
		Last Modified: Mon, 13 Nov 2023 14:13:05 GMT  
		Size: 378.0 MB (377985870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89732bc7504122601f40269fc9ddfb70982e633ea9caf641ae45736f2846b004`  
		Last Modified: Sat, 26 Jan 2019 16:40:00 GMT  
		Size: 39.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bad71d450f6d45ca090868b64d6fdfab5a371c5e113457e2bd0fe5614cfafc6d`  
		Last Modified: Mon, 13 Nov 2023 14:12:53 GMT  
		Size: 400.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac99c4e27b27daca90729e2d08629a77eaf8af06c23f48eef9293df615c109b4`  
		Last Modified: Mon, 13 Nov 2023 14:12:54 GMT  
		Size: 295.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:45a7c189991ce9f52de195064013887398f89ec7f2bcaff772f7944501099c5f`  
		Last Modified: Mon, 13 Nov 2023 14:12:55 GMT  
		Size: 499.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6d85b6e63ecfe3d979a1d9678da513c82550524af14eb68ad7034fe329f853cd`  
		Last Modified: Mon, 13 Nov 2023 14:12:56 GMT  
		Size: 1.7 KB (1686 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a2ca5cbdc643c57a4d116a7ced58b3872a85af9eee0c7a45ac822a56194e61c3`  
		Last Modified: Mon, 13 Nov 2023 14:12:56 GMT  
		Size: 296.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:137c420bd0fe4ac20cf3ad0d823a181d6652d19d4ead29e8c7033338efc3d87f`  
		Last Modified: Mon, 13 Nov 2023 14:12:57 GMT  
		Size: 4.1 KB (4124 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4dd658d818dc5967fa86497ef90ff34717ba07d9ebba374e718f8d47d1484735`  
		Last Modified: Mon, 13 Nov 2023 14:12:58 GMT  
		Size: 1.9 MB (1947942 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cdc8a8da7272c8c7bb56eee5a4e6b744a65c2ac9863d6cbd36d1a6144f0bbf7c`  
		Last Modified: Mon, 13 Nov 2023 14:12:58 GMT  
		Size: 744.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cdc8a8da7272c8c7bb56eee5a4e6b744a65c2ac9863d6cbd36d1a6144f0bbf7c`  
		Last Modified: Mon, 13 Nov 2023 14:12:58 GMT  
		Size: 744.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `logstash:8.11.1` - unknown; unknown

```console
$ docker pull logstash@sha256:7f6d1187a3e0f3af519514df1113c67e6f209f3427dee20684615fbc7b106180
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 MB (2819563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b6ebbb4df9c12261ae07399b1ee18e72c6a90ccb29f5ecb253cebe73bf9c2c8`

```dockerfile
```

-	Layers:
	-	`sha256:c86c2b9522d51ef9bca63fdc59036419631a44b331b8a801cf912a5b8557936f`  
		Last Modified: Thu, 16 Nov 2023 01:20:35 GMT  
		Size: 2.8 MB (2811309 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5cd9e3fdbb6d7dad8cbf7dcefbe17e6f89869cc88d4bfcc9e9cd8a1bab067863`  
		Last Modified: Thu, 16 Nov 2023 01:20:35 GMT  
		Size: 8.3 KB (8254 bytes)  
		MIME: application/vnd.in-toto+json
