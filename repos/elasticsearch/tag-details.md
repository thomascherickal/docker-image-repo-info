<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.13`](#elasticsearch71713)
-	[`elasticsearch:8.10.2`](#elasticsearch8102)

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

## `elasticsearch:8.10.2`

```console
$ docker pull elasticsearch@sha256:53efb4ba72e1c71c8223ee8d8de6537e8d992ad6cc8fcdf5dd944be93b6ab814
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.10.2` - linux; amd64

```console
$ docker pull elasticsearch@sha256:7aae8ab0a532acddfd9781476e0233c0a304cddce87264ce2e7f881c70ffdd42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **650.8 MB (650795727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb20157f1390e5b7c638973436fbe1f7ea995106b445aac3630de0839d112ecb`
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
# Tue, 19 Sep 2023 08:22:52 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Tue, 19 Sep 2023 08:22:53 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Tue, 19 Sep 2023 08:22:53 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 19 Sep 2023 08:22:53 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 19 Sep 2023 08:23:10 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Tue, 19 Sep 2023 08:23:11 GMT
COPY /bin/tini /bin/tini # buildkit
# Tue, 19 Sep 2023 08:23:11 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Sep 2023 08:23:11 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Tue, 19 Sep 2023 08:23:12 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Tue, 19 Sep 2023 08:23:12 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 19 Sep 2023 08:23:13 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 19 Sep 2023 08:23:13 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Tue, 19 Sep 2023 08:23:13 GMT
LABEL org.label-schema.build-date=2023-09-19T08:16:24.564900370Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=6d20dd8ce62365be9b1aca96427de4622e970e9e org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.10.2 org.opencontainers.image.created=2023-09-19T08:16:24.564900370Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=6d20dd8ce62365be9b1aca96427de4622e970e9e org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.10.2
# Tue, 19 Sep 2023 08:23:13 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 19 Sep 2023 08:23:13 GMT
CMD ["eswrapper"]
# Tue, 19 Sep 2023 08:23:13 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086f659de354d8a87c8a82511781cdf4abf99c085c170840235feaa24aa0439e`  
		Last Modified: Fri, 22 Sep 2023 01:05:13 GMT  
		Size: 7.5 MB (7510049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de879b95239d77e3be0eb37ba3cf86f657924b369b3bd099bb6d296905d26be5`  
		Last Modified: Fri, 22 Sep 2023 01:05:12 GMT  
		Size: 4.3 KB (4343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb521e57fd91553c3b205b4f7b9dde65337dcc33b65f73c435651e20e9e3d2f5`  
		Last Modified: Fri, 22 Sep 2023 01:06:04 GMT  
		Size: 614.4 MB (614387866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0c0034a9820ce687cd0595fdfbefec6efc22f78dc2a16e3f6e8726b743f0e0`  
		Last Modified: Fri, 22 Sep 2023 01:05:10 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c197fd61adc0a750b7efa3ab4c3627e260a13ce15dfcf32e306729760e7ba91`  
		Last Modified: Fri, 22 Sep 2023 01:05:10 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacfdbd7575a807bfbe22ed0e0baccf08b7719550b9fbd1f8dadc5871b55a10f`  
		Last Modified: Fri, 22 Sep 2023 01:05:10 GMT  
		Size: 191.9 KB (191870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b95a46968f83ea515318a7b4087ae77cf7023ff43b8972a71e8a8966487e5`  
		Last Modified: Fri, 22 Sep 2023 01:05:10 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e862dcba76375f19605069ebb08ddfcfeefb5c917e6973c533892ae6d545e8e`  
		Last Modified: Fri, 22 Sep 2023 01:05:10 GMT  
		Size: 109.2 KB (109238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.10.2` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:44b497e3b7639cad53a0f130688af91caff22fb385f016e1b060afe208dd7c2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.1 MB (444053831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23c2475f409b6cd3a2d8611bd7240fef51025830b550e059b10f0d4ca8f5f3b8`
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
# Tue, 19 Sep 2023 08:23:53 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Tue, 19 Sep 2023 08:23:57 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Tue, 19 Sep 2023 08:23:57 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 19 Sep 2023 08:23:57 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 19 Sep 2023 08:24:04 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Tue, 19 Sep 2023 08:24:04 GMT
COPY /bin/tini /bin/tini # buildkit
# Tue, 19 Sep 2023 08:24:04 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 19 Sep 2023 08:24:04 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Tue, 19 Sep 2023 08:24:05 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Tue, 19 Sep 2023 08:24:05 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 19 Sep 2023 08:24:07 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 19 Sep 2023 08:24:07 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Tue, 19 Sep 2023 08:24:07 GMT
LABEL org.label-schema.build-date=2023-09-19T08:16:24.564900370Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=6d20dd8ce62365be9b1aca96427de4622e970e9e org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.10.2 org.opencontainers.image.created=2023-09-19T08:16:24.564900370Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=6d20dd8ce62365be9b1aca96427de4622e970e9e org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.10.2
# Tue, 19 Sep 2023 08:24:07 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 19 Sep 2023 08:24:07 GMT
CMD ["eswrapper"]
# Tue, 19 Sep 2023 08:24:07 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f8802f612d8f458c3669c3b3c14e15aed7d1d96632b5eeb2617727deb72e71`  
		Last Modified: Fri, 22 Sep 2023 01:25:06 GMT  
		Size: 7.3 MB (7331672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0343a1851d8c8e40a7d82b2e292b8bf6c917a974ae16574bcdccdf6e04a3b7`  
		Last Modified: Fri, 22 Sep 2023 01:25:05 GMT  
		Size: 4.4 KB (4357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32130303ef74d6aa5100ebda27da7490381977342210fbd403523118199167c1`  
		Last Modified: Fri, 22 Sep 2023 01:25:27 GMT  
		Size: 409.2 MB (409210821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb37481f72caa4017ca2357c729b67af8991e70b0ffad4c3865eb3122eba8202`  
		Last Modified: Fri, 22 Sep 2023 01:25:03 GMT  
		Size: 9.1 KB (9095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6f3de1727f7bdd4bed707beda93c0e7d263f2d14441cb74cd43c3c8f6e0c93`  
		Last Modified: Fri, 22 Sep 2023 01:25:03 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1d7e9761133aabdbdbd8bcc7bc26d00b2a24da57252a81d464b0ad2cd328e6`  
		Last Modified: Fri, 22 Sep 2023 01:25:03 GMT  
		Size: 185.9 KB (185895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e863819dd2a34c49162fbbdcd44da261a557e47c8a80c6cc009ea219eb352d3c`  
		Last Modified: Fri, 22 Sep 2023 01:25:03 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabbd90021b43cf1cb28fa940506a5da4c32300f01f5ea025c2b4f9cfc68cf1d`  
		Last Modified: Fri, 22 Sep 2023 01:25:03 GMT  
		Size: 109.2 KB (109239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
