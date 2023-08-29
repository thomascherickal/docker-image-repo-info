<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.11`](#elasticsearch71711)
-	[`elasticsearch:7.17.12`](#elasticsearch71712)
-	[`elasticsearch:8.8.2`](#elasticsearch882)
-	[`elasticsearch:8.9.0`](#elasticsearch890)
-	[`elasticsearch:8.9.1`](#elasticsearch891)

## `elasticsearch:7.17.11`

**does not exist** (yet?)

## `elasticsearch:7.17.12`

```console
$ docker pull elasticsearch@sha256:295a3f67e74f5d30d597d742b0d2387340543fd9ee4b090c822130f9b461bff0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.17.12` - linux; amd64

```console
$ docker pull elasticsearch@sha256:09de980aef66b2c879c9f2bae02244aa9526d0ca15d3385ba88ee6d3b1c22557
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.3 MB (356274906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e12f24d547f7a416587396303fcae7f8228e75ebc3a5b970a79cedd91256fe1c`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

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
# Thu, 20 Jul 2023 05:37:59 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Thu, 20 Jul 2023 05:38:01 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Thu, 20 Jul 2023 05:38:02 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 20 Jul 2023 05:38:02 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 20 Jul 2023 05:38:20 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Thu, 20 Jul 2023 05:38:20 GMT
COPY /bin/tini /bin/tini # buildkit
# Thu, 20 Jul 2023 05:38:20 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Jul 2023 05:38:20 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Thu, 20 Jul 2023 05:38:23 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Thu, 20 Jul 2023 05:38:23 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 20 Jul 2023 05:38:24 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 20 Jul 2023 05:38:24 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Thu, 20 Jul 2023 05:38:24 GMT
LABEL org.label-schema.build-date=2023-07-20T05:33:33.690180787Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=e3b0c3d3c5c130e1dc6d567d6baef1c73eeb2059 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.12 org.opencontainers.image.created=2023-07-20T05:33:33.690180787Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=e3b0c3d3c5c130e1dc6d567d6baef1c73eeb2059 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.12
# Thu, 20 Jul 2023 05:38:24 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 20 Jul 2023 05:38:24 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f730e53da950f6ea7615ef96104ca2bee6e39f40923de90efc7fb6253c331d`  
		Last Modified: Wed, 02 Aug 2023 09:29:31 GMT  
		Size: 7.5 MB (7509902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00937b28d0ae005e91309a7e36c428adda3d0e8733063e101457dd45166682a4`  
		Last Modified: Wed, 02 Aug 2023 09:29:27 GMT  
		Size: 4.3 KB (4335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef31d9d48f767a2235bec564c378f53ac24e8b180ca436b213cbf0c9ccbca3bf`  
		Last Modified: Wed, 02 Aug 2023 09:30:58 GMT  
		Size: 319.9 MB (319867331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3302e7ae92d0fbcbda4f72b2920ebf046f58d4193033e0793110eed12633445c`  
		Last Modified: Wed, 02 Aug 2023 09:29:26 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39533148ce3716a5e8b954faa016fa4267ef73026f3f242af059ae22c28b09ed`  
		Last Modified: Wed, 02 Aug 2023 09:29:24 GMT  
		Size: 2.0 KB (1982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4873b68789259978b99abadf4fe9c2a714e589d0c600800a032475524d768410`  
		Last Modified: Wed, 02 Aug 2023 09:29:25 GMT  
		Size: 192.1 KB (192139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834621cdc73669366c4942ef04f5646054c5c41e846ebdebe6cf9a64a8bfb578`  
		Last Modified: Wed, 02 Aug 2023 09:29:24 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d765e9a19285f1e7deb1b963b605078e6fae9fd909297b4c30fd90b3f846965`  
		Last Modified: Wed, 02 Aug 2023 09:29:24 GMT  
		Size: 109.2 KB (109237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.17.12` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:2e59a6dbd274364fcd6945312141f4648cbd4645463ae4281c46efd82975e6bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.8 MB (352778423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ed8ceb6348c4f73b902a2586aa0a5bfa1739d82407273ce7f136a7ae6eb225`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

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
# Thu, 20 Jul 2023 05:39:14 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Thu, 20 Jul 2023 05:39:17 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Thu, 20 Jul 2023 05:39:17 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 20 Jul 2023 05:39:17 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 20 Jul 2023 05:39:22 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Thu, 20 Jul 2023 05:39:22 GMT
COPY /bin/tini /bin/tini # buildkit
# Thu, 20 Jul 2023 05:39:22 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 20 Jul 2023 05:39:22 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Thu, 20 Jul 2023 05:39:23 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Thu, 20 Jul 2023 05:39:23 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 20 Jul 2023 05:39:24 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 20 Jul 2023 05:39:24 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Thu, 20 Jul 2023 05:39:24 GMT
LABEL org.label-schema.build-date=2023-07-20T05:33:33.690180787Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=e3b0c3d3c5c130e1dc6d567d6baef1c73eeb2059 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.12 org.opencontainers.image.created=2023-07-20T05:33:33.690180787Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=e3b0c3d3c5c130e1dc6d567d6baef1c73eeb2059 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.12
# Thu, 20 Jul 2023 05:39:24 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 20 Jul 2023 05:39:24 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d8d2cecec7d4e8f9ce26b6a574f1031d908649763016604433586e4376ee9d`  
		Last Modified: Fri, 11 Aug 2023 19:12:58 GMT  
		Size: 7.3 MB (7330984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048c45513239d3be0c22fdc0f75f705fc0af9d74afc459046dbe7b5320d24d30`  
		Last Modified: Fri, 11 Aug 2023 19:12:56 GMT  
		Size: 4.4 KB (4359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243ee9770d7627c968b35cfafd61a4daea728eef9ac053107d5d5c093ac6c49d`  
		Last Modified: Fri, 11 Aug 2023 19:13:15 GMT  
		Size: 317.9 MB (317937825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40158c56b2f278021639b5aea4e35c96709024daa9327c807343ab7a7194152`  
		Last Modified: Fri, 11 Aug 2023 19:12:56 GMT  
		Size: 9.1 KB (9095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ef765ef9a494b1a9b2c133615628522c7ad6bc0bd842e512b7e69967043f7b`  
		Last Modified: Fri, 11 Aug 2023 19:12:56 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ee292f98e0d3c8fb3fe1adcef0175ca1fc3e4eee647e8cf5f788c7ef1ee894`  
		Last Modified: Fri, 11 Aug 2023 19:12:55 GMT  
		Size: 186.2 KB (186162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4ea39f4d4a8fc7e013276e2d62dac62dfa093e11e90341d599d768d63f3a64`  
		Last Modified: Fri, 11 Aug 2023 19:12:54 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c16b2b3cfdf718cb3f978dd395fa545c3f75ada989723405a04e0a99affd5e`  
		Last Modified: Fri, 11 Aug 2023 19:12:54 GMT  
		Size: 109.2 KB (109246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:8.8.2`

**does not exist** (yet?)

## `elasticsearch:8.9.0`

**does not exist** (yet?)

## `elasticsearch:8.9.1`

```console
$ docker pull elasticsearch@sha256:767f3d4fbc45c757bf167ac4dbafd05a6502bc2521a604d3a25c26b246fb36b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.9.1` - linux; amd64

```console
$ docker pull elasticsearch@sha256:f553b6c7f05abc35e8997f375644857b868dcc4370fe42fdd3f2a074bc9c075c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **649.4 MB (649381965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a61551b302003765c449a9530f5d07713b04182c8f8f3dccd35870303935add`
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
# Thu, 10 Aug 2023 05:08:42 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Thu, 10 Aug 2023 05:08:43 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Thu, 10 Aug 2023 05:08:43 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 10 Aug 2023 05:08:43 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 10 Aug 2023 05:09:05 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Thu, 10 Aug 2023 05:09:05 GMT
COPY /bin/tini /bin/tini # buildkit
# Thu, 10 Aug 2023 05:09:05 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Aug 2023 05:09:05 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Thu, 10 Aug 2023 05:09:06 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Thu, 10 Aug 2023 05:09:06 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 10 Aug 2023 05:09:09 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 10 Aug 2023 05:09:09 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Thu, 10 Aug 2023 05:09:09 GMT
LABEL org.label-schema.build-date=2023-08-10T05:02:32.517455352Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=a813d015ef1826148d9d389bd1c0d781c6e349f0 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.9.1 org.opencontainers.image.created=2023-08-10T05:02:32.517455352Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=a813d015ef1826148d9d389bd1c0d781c6e349f0 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.9.1
# Thu, 10 Aug 2023 05:09:09 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 10 Aug 2023 05:09:09 GMT
CMD ["eswrapper"]
# Thu, 10 Aug 2023 05:09:09 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e136a4bb2ac2045dacc9775e92adb15a9189da6e413de8f09f9f04096e6a2`  
		Last Modified: Tue, 22 Aug 2023 03:00:31 GMT  
		Size: 7.5 MB (7509952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7152b76747e43beb8edde587195c26f6e8d67ebd919f59ab1cbf98139147835b`  
		Last Modified: Tue, 22 Aug 2023 03:00:22 GMT  
		Size: 4.3 KB (4332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8013ece6ebe8a883c60f71fcef310e4fd6d866219fec353e345923a2ce90751`  
		Last Modified: Tue, 22 Aug 2023 03:01:12 GMT  
		Size: 613.0 MB (612974218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849477e03c16efeae31da371596d63c919e0ef03689bcc3e0a88a061af37365c`  
		Last Modified: Tue, 22 Aug 2023 03:00:21 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d088e0be5d68b28f2a15a56188eb5ba4cffe0b81a9f92ead66b9047d2214d6dd`  
		Last Modified: Tue, 22 Aug 2023 03:00:16 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fade93157f3c6af355865d8842d7ed9f75595cc0c487f1933efd2b79b8738f`  
		Last Modified: Tue, 22 Aug 2023 03:00:17 GMT  
		Size: 191.9 KB (191860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7486b389bb9cfb1071683b48eef58fe462fd7a8dd5158788c0a61ac568d78e29`  
		Last Modified: Tue, 22 Aug 2023 03:00:16 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c48a6f0a873607ebf277a4cbcc2b91657d63ce74759d12ef2769f92a666e935`  
		Last Modified: Tue, 22 Aug 2023 03:00:17 GMT  
		Size: 109.2 KB (109240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.9.1` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:88073c594d4991fb73bf663c40d8b6b5e1604655a6d5775408d97a500d6b66de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **442.7 MB (442650837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:180d266daa33362dde05444f275d8803a7b9dc43d27ae57dd55dc3f574ace1a4`
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
# Thu, 10 Aug 2023 05:09:49 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Thu, 10 Aug 2023 05:09:52 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Thu, 10 Aug 2023 05:09:52 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 10 Aug 2023 05:09:52 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 10 Aug 2023 05:09:55 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Thu, 10 Aug 2023 05:09:56 GMT
COPY /bin/tini /bin/tini # buildkit
# Thu, 10 Aug 2023 05:09:56 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Aug 2023 05:09:56 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Thu, 10 Aug 2023 05:09:56 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Thu, 10 Aug 2023 05:09:56 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 10 Aug 2023 05:09:58 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Thu, 10 Aug 2023 05:09:58 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Thu, 10 Aug 2023 05:09:58 GMT
LABEL org.label-schema.build-date=2023-08-10T05:02:32.517455352Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=a813d015ef1826148d9d389bd1c0d781c6e349f0 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.9.1 org.opencontainers.image.created=2023-08-10T05:02:32.517455352Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=a813d015ef1826148d9d389bd1c0d781c6e349f0 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.9.1
# Thu, 10 Aug 2023 05:09:58 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 10 Aug 2023 05:09:58 GMT
CMD ["eswrapper"]
# Thu, 10 Aug 2023 05:09:58 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a7aa74f5917a2e171f248ab4ba4a9b17415615d12c4beaa4df0b761ad7a305`  
		Last Modified: Wed, 23 Aug 2023 23:47:12 GMT  
		Size: 7.3 MB (7331589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e25ec58a64fb7ac615c80677c9dd5c13adb868ed210607266248d2f4bdf434`  
		Last Modified: Wed, 23 Aug 2023 23:47:11 GMT  
		Size: 4.3 KB (4350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b70c394c55d6956f8da7990a54d48ed778c942bdc6c52bfe631a02abbe79766`  
		Last Modified: Wed, 23 Aug 2023 23:47:33 GMT  
		Size: 407.8 MB (407807926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6c88cf13a97892a263710d369d78bf795d90ae66f738406ea26b5d7c40eeda`  
		Last Modified: Wed, 23 Aug 2023 23:47:08 GMT  
		Size: 9.1 KB (9096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d18493ceb72af7b5f735023b09cb0e55d05ec1e9f7cf40be8c29844a0eb779`  
		Last Modified: Wed, 23 Aug 2023 23:47:09 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e25530749bd39b9b0937b4243abc778961bce94456f7dcb0bfa9ec3bb35f172`  
		Last Modified: Wed, 23 Aug 2023 23:47:09 GMT  
		Size: 185.9 KB (185892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e749de4d29cc57bda3ded4bf4d4b55dde96063f42273f81059d85740d68988a5`  
		Last Modified: Wed, 23 Aug 2023 23:47:08 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ebbc569dcfd1b7fdeea7c7f0e30dd801227e8e932ed9a9368aff3565faefef`  
		Last Modified: Wed, 23 Aug 2023 23:47:10 GMT  
		Size: 109.2 KB (109236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
