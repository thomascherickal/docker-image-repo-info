<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.13`](#elasticsearch71713)
-	[`elasticsearch:8.9.2`](#elasticsearch892)

## `elasticsearch:7.17.13`

```console
$ docker pull elasticsearch@sha256:7a32c0bd5399222dfe7bb85327b4c05226b46027288ea266193e2193ef076b14
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.17.13` - linux; amd64

```console
$ docker pull elasticsearch@sha256:30934b143cf90326c5c909a1b2b5d0180f0ee345c053ea4cc4d24e7aa59ebad6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.3 MB (356332117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e5e531872826103bdf8eb271ce46d6a3046bf80c81d04d3f0f9b4727871f674`
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
# Thu, 31 Aug 2023 17:37:50 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Thu, 31 Aug 2023 17:37:52 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Thu, 31 Aug 2023 17:37:52 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 31 Aug 2023 17:37:52 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 31 Aug 2023 17:38:09 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Thu, 31 Aug 2023 17:38:09 GMT
COPY /bin/tini /bin/tini # buildkit
# Thu, 31 Aug 2023 17:38:09 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 17:38:09 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Thu, 31 Aug 2023 17:38:09 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Thu, 31 Aug 2023 17:38:10 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 31 Aug 2023 17:38:11 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 31 Aug 2023 17:38:11 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Thu, 31 Aug 2023 17:38:11 GMT
LABEL org.label-schema.build-date=2023-08-31T17:33:19.958690787Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=2b211dbb8bfdecaf7f5b44d356bdfe54b1050c13 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.13 org.opencontainers.image.created=2023-08-31T17:33:19.958690787Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=2b211dbb8bfdecaf7f5b44d356bdfe54b1050c13 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.13
# Thu, 31 Aug 2023 17:38:11 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 31 Aug 2023 17:38:11 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3338394bb482b95c33f794fe78a80c1208116a2939740f288577a6c903dbae82`  
		Last Modified: Fri, 08 Sep 2023 04:18:50 GMT  
		Size: 7.5 MB (7509892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b9c4941f7456d2f00a407a07b2a716178bd46e688c0f276b32d0f2a4e5ccf6`  
		Last Modified: Fri, 08 Sep 2023 04:18:48 GMT  
		Size: 4.3 KB (4328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90209b0ac7c7749d6ae27ac103b3d63144a3483b7a76652451d5d9140f92218a`  
		Last Modified: Fri, 08 Sep 2023 04:19:22 GMT  
		Size: 319.9 MB (319923887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6d1afbb72b48a28e37b5456338e989e53e17d020048e3d9980f0f4cf6330d2`  
		Last Modified: Fri, 08 Sep 2023 04:18:48 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690601a2b955e10d190c722d78fe6bbca42f62398f700ffb98909c2b91081b16`  
		Last Modified: Fri, 08 Sep 2023 04:18:45 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3b6afc4d162ec6e26e2c3e13e600e497e25c4f31a4d99d992ae6849c94d54`  
		Last Modified: Fri, 08 Sep 2023 04:18:45 GMT  
		Size: 192.1 KB (192140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee478770ef53ced28bdc4126fbe26cacb2e15664938000db1b8ed4175d206356`  
		Last Modified: Fri, 08 Sep 2023 04:18:45 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2384b3ff12859f6f7562dae8f6237b1824ed10b1ad161ce3c5eb9cb2ee50eb2`  
		Last Modified: Fri, 08 Sep 2023 04:18:45 GMT  
		Size: 109.2 KB (109247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.17.13` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:4bf5bc03b5d7e7c8ded9b75fa0bd4915dcfee9564cc87eab988231ce127a976f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.8 MB (352840815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a7cbb2f76ed247ee322dc3984b964b379128ea9824d1d6c9497bba16de05b7f`
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
# Thu, 31 Aug 2023 17:39:08 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Thu, 31 Aug 2023 17:39:10 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Thu, 31 Aug 2023 17:39:10 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 31 Aug 2023 17:39:10 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 31 Aug 2023 17:39:13 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Thu, 31 Aug 2023 17:39:13 GMT
COPY /bin/tini /bin/tini # buildkit
# Thu, 31 Aug 2023 17:39:13 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 17:39:13 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Thu, 31 Aug 2023 17:39:14 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Thu, 31 Aug 2023 17:39:14 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 31 Aug 2023 17:39:15 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 31 Aug 2023 17:39:15 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Thu, 31 Aug 2023 17:39:15 GMT
LABEL org.label-schema.build-date=2023-08-31T17:33:19.958690787Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=2b211dbb8bfdecaf7f5b44d356bdfe54b1050c13 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.13 org.opencontainers.image.created=2023-08-31T17:33:19.958690787Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=2b211dbb8bfdecaf7f5b44d356bdfe54b1050c13 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.13
# Thu, 31 Aug 2023 17:39:15 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 31 Aug 2023 17:39:15 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6c870f81713b73262b8749ea43efda6d46d2f7c4c00e2cff8bca8e8c8ac1fe`  
		Last Modified: Thu, 07 Sep 2023 23:36:41 GMT  
		Size: 7.3 MB (7331515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286da3bbb43a9beb9521fbf38b9af9e1c68ec20564b22b1c2eb9197a838f1a80`  
		Last Modified: Thu, 07 Sep 2023 23:36:40 GMT  
		Size: 4.4 KB (4351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da8774595b83e69d2fed8d8eb3a5650ec0730c50bd18bc176c5bd594daab8a5`  
		Last Modified: Thu, 07 Sep 2023 23:37:01 GMT  
		Size: 318.0 MB (317997416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fb8fd5d0389f7160b7d97a898edcd63024477c7320bd992af5af6e59f0d325`  
		Last Modified: Thu, 07 Sep 2023 23:36:38 GMT  
		Size: 9.1 KB (9101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7094b424a4fcbec80d5c76e30b50d83203b1cec1b3ecb3aa4ec161b66012a648`  
		Last Modified: Thu, 07 Sep 2023 23:36:38 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aef9dc948bd773773407291ec534a537fe4d09f7de6bfd61e69c0532e818a47`  
		Last Modified: Thu, 07 Sep 2023 23:36:38 GMT  
		Size: 186.2 KB (186175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52483b14584715fe36ca156fadc4d15e4003355d99dbc4c4ccdc36b7e1fdc188`  
		Last Modified: Thu, 07 Sep 2023 23:36:38 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105ed2ec6e831e3252f06d971ea53a644e81f0716c283618fb8c57a576c01501`  
		Last Modified: Thu, 07 Sep 2023 23:36:38 GMT  
		Size: 109.2 KB (109244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:8.9.2`

```console
$ docker pull elasticsearch@sha256:38082e945768e8e98fc0d828c810baf0b63d58ddc9059db2a62e4c293e44e817
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.9.2` - linux; amd64

```console
$ docker pull elasticsearch@sha256:25e0ad0c0e7b7897e964367e7954f8130446ee8ae512765b4d7f91acf673f8cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **649.4 MB (649382012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cccb6ce650c498b355019121a35e5ba17c61cf1a8f0e58d469c2b765de52e89f`
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
# Thu, 31 Aug 2023 02:49:25 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Thu, 31 Aug 2023 02:49:26 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Thu, 31 Aug 2023 02:49:26 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 31 Aug 2023 02:49:26 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 31 Aug 2023 02:49:43 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Thu, 31 Aug 2023 02:49:43 GMT
COPY /bin/tini /bin/tini # buildkit
# Thu, 31 Aug 2023 02:49:43 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 02:49:43 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Thu, 31 Aug 2023 02:49:45 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Thu, 31 Aug 2023 02:49:45 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 31 Aug 2023 02:49:45 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 31 Aug 2023 02:49:45 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Thu, 31 Aug 2023 02:49:45 GMT
LABEL org.label-schema.build-date=2023-08-31T02:43:14.210479707Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=e8179018838f55b8820685f92e245abef3bddc0f org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.9.2 org.opencontainers.image.created=2023-08-31T02:43:14.210479707Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=e8179018838f55b8820685f92e245abef3bddc0f org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.9.2
# Thu, 31 Aug 2023 02:49:45 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 31 Aug 2023 02:49:45 GMT
CMD ["eswrapper"]
# Thu, 31 Aug 2023 02:49:45 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04adb7909f5278a73a0687d2e86fbc246dc486bbeff1f06cd7c540559d0e1dc3`  
		Last Modified: Fri, 08 Sep 2023 05:18:09 GMT  
		Size: 7.5 MB (7509974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee481ddf31334d8e46875a32c95175496be2e0eeffeeb30e5846df2a63a9a471`  
		Last Modified: Fri, 08 Sep 2023 05:18:07 GMT  
		Size: 4.3 KB (4339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f7280337e1fedc00c4def9d07f4b46384d6014956f53dca36b9248fd7b73f5`  
		Last Modified: Fri, 08 Sep 2023 05:18:58 GMT  
		Size: 613.0 MB (612974226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a46f8f0c0914aba9805b12ff25ba26122eb44b09c9c2cd4a1fa94aa06e1489e`  
		Last Modified: Fri, 08 Sep 2023 05:18:05 GMT  
		Size: 9.5 KB (9531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a552db92036c846d2139b4621c95a7adc05156c4a105a40dd1ae0eecbd3ced47`  
		Last Modified: Fri, 08 Sep 2023 05:18:05 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bacce6024cc8de84f134888bb4ac232e988806b5c00741bc78db3d4acdb525`  
		Last Modified: Fri, 08 Sep 2023 05:18:05 GMT  
		Size: 191.9 KB (191869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284757fa4ceffdeb0d9833a9f8048b4e98a79375091c8737be00fd71636b49c9`  
		Last Modified: Fri, 08 Sep 2023 05:18:05 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efae4bf9712ff75052c2c31a8615abe31903d66bb209d42e69c4b1f4a0300237`  
		Last Modified: Fri, 08 Sep 2023 05:18:05 GMT  
		Size: 109.2 KB (109240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.9.2` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:baa6fcf2ff89afdd4fc172e4502c252e8e39c3d3b80383c8ff8e31150373fd41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **442.7 MB (442651606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d590ac737663c10454922da5bfec9c81efa90b4e082ecb43055a8068587d60eb`
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
# Thu, 31 Aug 2023 02:50:24 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Thu, 31 Aug 2023 02:50:27 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Thu, 31 Aug 2023 02:50:27 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 31 Aug 2023 02:50:27 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 31 Aug 2023 02:50:31 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Thu, 31 Aug 2023 02:50:31 GMT
COPY /bin/tini /bin/tini # buildkit
# Thu, 31 Aug 2023 02:50:31 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 31 Aug 2023 02:50:31 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Thu, 31 Aug 2023 02:50:33 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Thu, 31 Aug 2023 02:50:34 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 31 Aug 2023 02:50:36 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 31 Aug 2023 02:50:36 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Thu, 31 Aug 2023 02:50:36 GMT
LABEL org.label-schema.build-date=2023-08-31T02:43:14.210479707Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=e8179018838f55b8820685f92e245abef3bddc0f org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.9.2 org.opencontainers.image.created=2023-08-31T02:43:14.210479707Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=e8179018838f55b8820685f92e245abef3bddc0f org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.9.2
# Thu, 31 Aug 2023 02:50:36 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 31 Aug 2023 02:50:36 GMT
CMD ["eswrapper"]
# Thu, 31 Aug 2023 02:50:36 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c788e962643467c75e5788a6e2c5c94a737b12b8293e7c20daf7e540fb309422`  
		Last Modified: Thu, 07 Sep 2023 23:36:10 GMT  
		Size: 7.3 MB (7331609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c76694d00528c637ebd45c4b70d916de9fe456965df57f613e43427cb1b887`  
		Last Modified: Thu, 07 Sep 2023 23:36:09 GMT  
		Size: 4.4 KB (4356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9020d2452aa3efac0c3babb32176560b4473b3f60a53bc3cf309ce4ed6d811`  
		Last Modified: Thu, 07 Sep 2023 23:36:31 GMT  
		Size: 407.8 MB (407808647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c754b80930aae6bbdcfc6920d136f80605a5310fb05fe0c914aa096ff844c61`  
		Last Modified: Thu, 07 Sep 2023 23:36:06 GMT  
		Size: 9.1 KB (9099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ed4842606ebd1d7deed4121bd77c6ee386bbe58f562f7ceb5ad6ad51368396`  
		Last Modified: Thu, 07 Sep 2023 23:36:06 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6a5c3cd69a7b2fae7d43a0bce44005f5bd9bad108f27830a680acbc55dd2d`  
		Last Modified: Thu, 07 Sep 2023 23:36:07 GMT  
		Size: 185.9 KB (185900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a915126bc3aa024566ae63ac1ee247bf91ec781db6de5f01b08eb28607506e`  
		Last Modified: Thu, 07 Sep 2023 23:36:06 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee22a2924a098058e713d0d7152716e7ab81222d64384abe48f17dd4de867a1`  
		Last Modified: Thu, 07 Sep 2023 23:36:07 GMT  
		Size: 109.2 KB (109242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
