<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.14`](#elasticsearch71714)
-	[`elasticsearch:8.11.0`](#elasticsearch8110)

## `elasticsearch:7.17.14`

```console
$ docker pull elasticsearch@sha256:574515ab039108e3f1a18bdc7ec19246a4c0bba72bf71cc3846d42f020073b79
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `elasticsearch:7.17.14` - linux; amd64

```console
$ docker pull elasticsearch@sha256:25f569f57081755530e8103ba5e1916ca1ffa4cb7b9148455b3466bb1e3acd26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.8 MB (397826736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63bea68e170705752d386e2f360713e71333b7df9383bf77facddfaafb214953`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

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
# Thu, 05 Oct 2023 22:22:24 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Thu, 05 Oct 2023 22:22:25 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Thu, 05 Oct 2023 22:22:25 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 05 Oct 2023 22:22:25 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 05 Oct 2023 22:22:41 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Thu, 05 Oct 2023 22:22:41 GMT
COPY /bin/tini /bin/tini # buildkit
# Thu, 05 Oct 2023 22:22:41 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 22:22:41 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Thu, 05 Oct 2023 22:22:42 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Thu, 05 Oct 2023 22:22:42 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 05 Oct 2023 22:22:43 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 05 Oct 2023 22:22:43 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Thu, 05 Oct 2023 22:22:43 GMT
LABEL org.label-schema.build-date=2023-10-05T22:17:33.780167078Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=774e3bfa4d52e2834e4d9d8d669d77e4e5c1017f org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.14 org.opencontainers.image.created=2023-10-05T22:17:33.780167078Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=774e3bfa4d52e2834e4d9d8d669d77e4e5c1017f org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.14
# Thu, 05 Oct 2023 22:22:43 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 05 Oct 2023 22:22:43 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:f9175e7b73a4b948b4c5db289cbeeb1d8511aee675255978036e76ffeda560be`  
		Last Modified: Mon, 07 Aug 2023 21:55:17 GMT  
		Size: 31.8 MB (31795971 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5554e1a3574b1a18e1e4bb8ad0ee4dd6471fe33efa73abc39bdb8d9f26df4aa5`  
		Last Modified: Tue, 10 Oct 2023 09:01:43 GMT  
		Size: 15.8 MB (15770658 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa31645a5670143fcaedf39689006a7b5ca9c0efbb08cfc4083219b8b2ffea94`  
		Last Modified: Tue, 10 Oct 2023 09:01:42 GMT  
		Size: 4.5 KB (4512 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89732bc7504122601f40269fc9ddfb70982e633ea9caf641ae45736f2846b004`  
		Last Modified: Sat, 26 Jan 2019 16:40:00 GMT  
		Size: 39.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:abcb33a8db97260b1f5f77687a4582307813448130bc2144cc06c418ffd2dc49`  
		Last Modified: Tue, 10 Oct 2023 09:02:11 GMT  
		Size: 349.9 MB (349916616 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfaf05422aaa7b8190ef948de40f088c7de96cc23cc5805ee9da6434f0649d12`  
		Last Modified: Tue, 10 Oct 2023 09:01:42 GMT  
		Size: 10.2 KB (10154 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6080ea97dfc51155d81b3335dc23c7d416e0236a91459b04ff74376114cd884b`  
		Last Modified: Tue, 10 Oct 2023 09:01:43 GMT  
		Size: 2.2 KB (2156 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f85837b82c46c512ea976ba33d6d6e988bd6cce4a4dd5789c3d351cd8a3650ca`  
		Last Modified: Tue, 10 Oct 2023 09:01:43 GMT  
		Size: 211.3 KB (211289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2dc4537d05c67aeced0013cc941403c36b7855adf6517ca2cf1dfc7318dbdbb6`  
		Last Modified: Tue, 10 Oct 2023 09:01:44 GMT  
		Size: 421.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:453482f77361336152d142cd407921f28cfb254ab33b1d248d735a3dcf6e1e7a`  
		Last Modified: Tue, 10 Oct 2023 09:01:45 GMT  
		Size: 114.9 KB (114920 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:7.17.14` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:a35095c1a34996113a365dd690794e55d85dabdc6e55c7466ea6c2639be9d212
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2073577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f18c0e6af4371ebbd51c32829db92e08e72b8ae6db17b6a9f6fa2c82e4dad29`

```dockerfile
```

-	Layers:
	-	`sha256:deacc7924d4e2a0214f187bc34505ba2c4c14d9d2076b5620cddf924042f44f9`  
		Last Modified: Thu, 09 Nov 2023 22:19:50 GMT  
		Size: 2.1 MB (2066531 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d06bd2fad9f20e284f01355560066bb636ff71b7ba78fa110c36cb1fb7e8e59`  
		Last Modified: Thu, 09 Nov 2023 22:19:50 GMT  
		Size: 7.0 KB (7046 bytes)  
		MIME: application/vnd.in-toto+json

### `elasticsearch:7.17.14` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:d33109631317496a23ecc6fe58f6a9501433157f13c26b69f50dd46948ef0dc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.8 MB (391753521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fc9fd861ebb65b1c3974e67ffaf503a8e0e905dad32a47b1e4616911ddf1625`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

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
# Thu, 05 Oct 2023 22:24:00 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Thu, 05 Oct 2023 22:24:02 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Thu, 05 Oct 2023 22:24:02 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 05 Oct 2023 22:24:02 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 05 Oct 2023 22:24:04 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Thu, 05 Oct 2023 22:24:04 GMT
COPY /bin/tini /bin/tini # buildkit
# Thu, 05 Oct 2023 22:24:04 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 Oct 2023 22:24:05 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Thu, 05 Oct 2023 22:24:05 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Thu, 05 Oct 2023 22:24:05 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 05 Oct 2023 22:24:06 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 05 Oct 2023 22:24:06 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Thu, 05 Oct 2023 22:24:06 GMT
LABEL org.label-schema.build-date=2023-10-05T22:17:33.780167078Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=774e3bfa4d52e2834e4d9d8d669d77e4e5c1017f org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.14 org.opencontainers.image.created=2023-10-05T22:17:33.780167078Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=774e3bfa4d52e2834e4d9d8d669d77e4e5c1017f org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.14
# Thu, 05 Oct 2023 22:24:06 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 05 Oct 2023 22:24:06 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:e61e4aa6ecf06d84f177710ed7a16ba36429af08286de7aa5a485fdcedaac1f7`  
		Last Modified: Thu, 17 Aug 2023 10:22:08 GMT  
		Size: 29.9 MB (29915840 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5769763037ebcd15fde62217b602bc4abdcb7821639fe6d748180c46abb20e97`  
		Last Modified: Tue, 10 Oct 2023 09:01:44 GMT  
		Size: 14.2 MB (14213381 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4efa310c2be754f6f5f5a7b9f4e74cc7ec1f6d82e086a1a21a9d964c68143305`  
		Last Modified: Tue, 10 Oct 2023 09:01:42 GMT  
		Size: 4.5 KB (4541 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89732bc7504122601f40269fc9ddfb70982e633ea9caf641ae45736f2846b004`  
		Last Modified: Sat, 26 Jan 2019 16:40:00 GMT  
		Size: 39.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:abc4e05cd98d246c674f763523145790311128acdab4022b024be45d195066d4`  
		Last Modified: Tue, 10 Oct 2023 09:01:59 GMT  
		Size: 347.3 MB (347289156 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3126aacc4def6755895c98ff634db573c2c923382e22a01d306c514a0f45cb47`  
		Last Modified: Tue, 10 Oct 2023 09:01:42 GMT  
		Size: 9.8 KB (9756 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa2e68d1e2f79cacb6bb31c5132beac0c193109ab1b7610f08b83520cdcddb2d`  
		Last Modified: Tue, 10 Oct 2023 09:01:44 GMT  
		Size: 2.2 KB (2156 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7eb2273899d5909c4599c62d71d58e07ace932099fd7bc04046b9bc16c3b15d6`  
		Last Modified: Tue, 10 Oct 2023 09:01:44 GMT  
		Size: 203.2 KB (203168 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73effe027f666465e021f7ff92954e0454480c24cf4795129ad982c3846c5272`  
		Last Modified: Tue, 10 Oct 2023 09:01:45 GMT  
		Size: 424.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5d158c05b3198b448d758aae60d155e9f91b9641f3193f1b39c0b2e83bed7669`  
		Last Modified: Tue, 10 Oct 2023 09:01:45 GMT  
		Size: 115.1 KB (115060 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:7.17.14` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:fad4c134ace65dc819474f34c608f61201e5ec76cb1710892b991e24b242196a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2073902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46703196d4e7b959233b8b7c4147bd506491ba532ecce5492e49d3bd1c6e283f`

```dockerfile
```

-	Layers:
	-	`sha256:8bcc2efbb7b1e3419b4ff4d7ae4ee6e9e14bda7a5dc6b9988e0f90d652055fb3`  
		Last Modified: Thu, 09 Nov 2023 22:30:25 GMT  
		Size: 2.1 MB (2066854 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c333947ab6d04a5f5ce0159e676425fb3e3da30ea5be20c3d72f36a88bd43d60`  
		Last Modified: Thu, 09 Nov 2023 22:30:24 GMT  
		Size: 7.0 KB (7048 bytes)  
		MIME: application/vnd.in-toto+json

## `elasticsearch:8.11.0`

```console
$ docker pull elasticsearch@sha256:2cadca6c21de5802b085f25532bba11cb893589b64ca8c94d62ac69eec923fad
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 3
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8

### `elasticsearch:8.11.0` - linux; amd64

```console
$ docker pull elasticsearch@sha256:16c4a2652c83a992e245ca3b88c01bfe518cbbcd6a14dca2eb9a92856ad6b560
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **740.2 MB (740208871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f03b6ec0c6f6d9a844550d1b3689e868e11850ac4e668e8583490c96baca8f1`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

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
# Sat, 04 Nov 2023 10:11:35 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Sat, 04 Nov 2023 10:11:36 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Sat, 04 Nov 2023 10:11:36 GMT
ENV ELASTIC_CONTAINER=true
# Sat, 04 Nov 2023 10:11:36 GMT
WORKDIR /usr/share/elasticsearch
# Sat, 04 Nov 2023 10:11:58 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Sat, 04 Nov 2023 10:11:58 GMT
COPY /bin/tini /bin/tini # buildkit
# Sat, 04 Nov 2023 10:11:58 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 10:11:58 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Sat, 04 Nov 2023 10:12:05 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Sat, 04 Nov 2023 10:12:05 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Sat, 04 Nov 2023 10:12:07 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Sat, 04 Nov 2023 10:12:07 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Sat, 04 Nov 2023 10:12:07 GMT
LABEL org.label-schema.build-date=2023-11-04T10:04:57.184859352Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=d9ec3fa628c7b0ba3d25692e277ba26814820b20 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.11.0 org.opencontainers.image.created=2023-11-04T10:04:57.184859352Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=d9ec3fa628c7b0ba3d25692e277ba26814820b20 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.0
# Sat, 04 Nov 2023 10:12:07 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Sat, 04 Nov 2023 10:12:07 GMT
CMD ["eswrapper"]
# Sat, 04 Nov 2023 10:12:07 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:70db4e7a2af7f73b7cef95301fc20fbedcfe68e5fb874e2cfba0b5ae41a066ca`  
		Last Modified: Wed, 25 Oct 2023 11:40:40 GMT  
		Size: 31.8 MB (31790746 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:84c497127d4d140073d7beed630e7adbe42369c449a60f4ba6edfcb9de2b2b23`  
		Last Modified: Tue, 07 Nov 2023 14:58:36 GMT  
		Size: 8.4 MB (8370631 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69a4900fd2ef7800018d95d3add5afc573566dda8c0d313a802d37764fc18709`  
		Last Modified: Tue, 07 Nov 2023 14:58:35 GMT  
		Size: 4.5 KB (4539 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89732bc7504122601f40269fc9ddfb70982e633ea9caf641ae45736f2846b004`  
		Last Modified: Sat, 26 Jan 2019 16:40:00 GMT  
		Size: 39.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f8b03cec5ab020d0f8bcf2e319272ff00e2a987aafee6f76d7d8f4146d40820`  
		Last Modified: Tue, 07 Nov 2023 14:59:14 GMT  
		Size: 699.7 MB (699704720 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d1ab6296a7fb2f087db5f286c59af46a674cc8f9924edad45af441206806e4b4`  
		Last Modified: Tue, 07 Nov 2023 14:58:36 GMT  
		Size: 10.2 KB (10153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c20737c529206e2ddb438aa42e20b6f49f8c42f0f08d694aa143fd345f31cfc`  
		Last Modified: Tue, 07 Nov 2023 14:58:38 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:93eb87cc64de15a48de3c1ea95779b34ddd22a8ca773a8be2b683ef72f7ce791`  
		Last Modified: Tue, 07 Nov 2023 14:58:38 GMT  
		Size: 211.0 KB (210977 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f0b2409f2858b94ed49aac8105ee5e94888e65a7f9dc333aa368209e11f13af`  
		Last Modified: Tue, 07 Nov 2023 14:58:38 GMT  
		Size: 422.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:737c82307a380a04f10cbdc08004d268c67edd00cd24b8726d3283663df0260d`  
		Last Modified: Tue, 07 Nov 2023 14:58:39 GMT  
		Size: 114.8 KB (114842 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `elasticsearch:8.11.0` - unknown; unknown

```console
$ docker pull elasticsearch@sha256:f6dea30e2b80be22248c09d15cb02f14c735d22a278c54b13f8ecfb28b2b720f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 MB (2342621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c959784e6d9caff9dfd1f58666c697da1b64d24bb6ffaf6cd02643d6e09f99d`

```dockerfile
```

-	Layers:
	-	`sha256:d3fbb512d34dbb96a1bdfc258e8440765bee10f44e54747048337e1b22ac055b`  
		Last Modified: Thu, 09 Nov 2023 22:20:35 GMT  
		Size: 2.3 MB (2335583 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:36265a2e05a1f0fed78e720055562c27d140b514c2b5e351e026d0ae6f7fa43b`  
		Last Modified: Thu, 09 Nov 2023 22:20:34 GMT  
		Size: 7.0 KB (7038 bytes)  
		MIME: application/vnd.in-toto+json

### `elasticsearch:8.11.0` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:b59dfd735d101120bb6cb57230a04ce7c06fb328e7a743f9c93a64f418b3b264
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **452.0 MB (451992726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6435e9be51cc0e5ba8b6746892bae1cacf974262a08857b1c8d4a0241b85fee1`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

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
# Sat, 04 Nov 2023 10:12:39 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Sat, 04 Nov 2023 10:12:43 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Sat, 04 Nov 2023 10:12:43 GMT
ENV ELASTIC_CONTAINER=true
# Sat, 04 Nov 2023 10:12:43 GMT
WORKDIR /usr/share/elasticsearch
# Sat, 04 Nov 2023 10:12:48 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Sat, 04 Nov 2023 10:12:48 GMT
COPY /bin/tini /bin/tini # buildkit
# Sat, 04 Nov 2023 10:12:48 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Nov 2023 10:12:48 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Sat, 04 Nov 2023 10:12:52 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Sat, 04 Nov 2023 10:12:52 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Sat, 04 Nov 2023 10:12:54 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Sat, 04 Nov 2023 10:12:54 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Sat, 04 Nov 2023 10:12:54 GMT
LABEL org.label-schema.build-date=2023-11-04T10:04:57.184859352Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=d9ec3fa628c7b0ba3d25692e277ba26814820b20 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.11.0 org.opencontainers.image.created=2023-11-04T10:04:57.184859352Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=d9ec3fa628c7b0ba3d25692e277ba26814820b20 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.11.0
# Sat, 04 Nov 2023 10:12:54 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Sat, 04 Nov 2023 10:12:54 GMT
CMD ["eswrapper"]
# Sat, 04 Nov 2023 10:12:54 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b7fce9281e3afe428ea22b2d0da41999a20290ba20993fdf2d336733b323bf`  
		Last Modified: Tue, 07 Nov 2023 23:42:43 GMT  
		Size: 7.3 MB (7330723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1098896b92da1cfd88f11c251a1f0f10d59be1cc8ccde2dde821411eee84944e`  
		Last Modified: Tue, 07 Nov 2023 23:42:42 GMT  
		Size: 4.4 KB (4356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4112cc587f28c9849a6b4d06446fbc0bead1e0b0a12f5d4a2cc0da61af1bf09e`  
		Last Modified: Tue, 07 Nov 2023 23:43:03 GMT  
		Size: 417.2 MB (417151732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ccd21d2d57c1dc3964f65983aa45b2a8e27e89e5d9e811e0ff28e5c802ce1c`  
		Last Modified: Tue, 07 Nov 2023 23:42:39 GMT  
		Size: 9.1 KB (9098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f00d26bc538e2b7ac5aec6408335fe3e07701d3ecf79e005d1b07b571c6080`  
		Last Modified: Tue, 07 Nov 2023 23:42:39 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a81a8d5c2aad8e7b8b1cd30146764bd94c3844aec6158edc4370771dc95220`  
		Last Modified: Tue, 07 Nov 2023 23:42:39 GMT  
		Size: 185.9 KB (185902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c1431ac2e95f1addcb9cc00cdcae71cc3976acaa41aaf4e6a1dc37ddf86bf0`  
		Last Modified: Tue, 07 Nov 2023 23:42:39 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7241b5cb1d4aad2ef0ecc1678f40ac77a8876c63b28c6f6f1d5a5dca6e8e3526`  
		Last Modified: Tue, 07 Nov 2023 23:42:43 GMT  
		Size: 109.2 KB (109244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
