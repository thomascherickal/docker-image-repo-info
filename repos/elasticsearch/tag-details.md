<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.14`](#elasticsearch71714)
-	[`elasticsearch:8.10.4`](#elasticsearch8104)

## `elasticsearch:7.17.14`

```console
$ docker pull elasticsearch@sha256:2283a10121603e695e84313e8b794b310a1e2a9c458d3f165f20431a510423d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.17.14` - linux; amd64

```console
$ docker pull elasticsearch@sha256:c7b7c4f45b516ff5bf6abc95488338f1e56b9d2fd14e74a79d98e32d302f6be4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.4 MB (367415646 bytes)**  
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
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce03a8bcc73c8878a1bd2c63a68936e8f31bc3386f0cbcfb5beac6f7ef4726b6`  
		Last Modified: Sun, 15 Oct 2023 21:41:20 GMT  
		Size: 14.1 MB (14103913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a135dee158bbec26d1f8d60aff8bd3bca9d27f83db8df03f0a0f227af41735c`  
		Last Modified: Sun, 15 Oct 2023 21:41:18 GMT  
		Size: 4.3 KB (4339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6447c6580cc6bd881aa25fec3b8f90e5948a25313d8dd2918dc882253740cba6`  
		Last Modified: Sun, 15 Oct 2023 21:41:42 GMT  
		Size: 324.4 MB (324413388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d49beb0c9d2b18f4cb3e5fc248b83a9007992c538ec5535511c2a5ba1666941`  
		Last Modified: Sun, 15 Oct 2023 21:41:21 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a9cc20930a7d1fe1e7a3baacb9e620b0188428e5aa6efe317ed4170b2f5935`  
		Last Modified: Sun, 15 Oct 2023 21:41:17 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21f30d4808d368aa997e7aca2302faa3abf388e5c1d842ab20e72e278cf706f`  
		Last Modified: Sun, 15 Oct 2023 21:41:16 GMT  
		Size: 192.1 KB (192139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3bebd03fbb146490b4ab33b89e39b84152012a3ae2983a5e8622b6dd2d6d97`  
		Last Modified: Sun, 15 Oct 2023 21:41:16 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78556d8f50914c24306090f59b050ea9d57d32f6dec27189167744f649da3289`  
		Last Modified: Sun, 15 Oct 2023 21:41:15 GMT  
		Size: 109.2 KB (109243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.17.14` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:d0f7cf9064bbc124a765cfc4cae4897cca33eccdd2f00d6bb4e633fa7793a414
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.7 MB (362710792 bytes)**  
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
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1527c3d34f6dbcd2d497bb04cd79773b5470c9ee598bbe1f592495ff0c1f7d`  
		Last Modified: Thu, 02 Nov 2023 23:40:35 GMT  
		Size: 12.9 MB (12853835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6208089f8a98805e375a073eb608564601514f0219e8f69db14ca33f7e7d86a7`  
		Last Modified: Thu, 02 Nov 2023 23:40:33 GMT  
		Size: 4.4 KB (4357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf64e867920b9c94613a084b44db7fbe97e79859bc076992d9e8e2bd509a32c6`  
		Last Modified: Thu, 02 Nov 2023 23:40:52 GMT  
		Size: 322.3 MB (322345079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87076fbd4cb01c68c48b2fa981718ed64e1cc9e38e97102806fe7b728801642f`  
		Last Modified: Thu, 02 Nov 2023 23:40:31 GMT  
		Size: 9.1 KB (9098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c1393344f7f80e266e3e2e30a3682db05271224129b05afaebe4e1085c4474`  
		Last Modified: Thu, 02 Nov 2023 23:40:31 GMT  
		Size: 2.0 KB (1983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395bc23cbc3d289367e4e75dfed87d93be0b7b21120edd3d00bcc7747c6a6e6c`  
		Last Modified: Thu, 02 Nov 2023 23:40:31 GMT  
		Size: 186.2 KB (186163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7705b912b1248807b93bb078c794e0d254f908d516f1d0b6e7a11e17723391d2`  
		Last Modified: Thu, 02 Nov 2023 23:40:31 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb67150a47fb253abf189c118218a617eca7e5c20afe6670b391c71417815e7`  
		Last Modified: Thu, 02 Nov 2023 23:40:31 GMT  
		Size: 109.2 KB (109248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:8.10.4`

```console
$ docker pull elasticsearch@sha256:180a0b356c6d1b5ae49063aac79e7b0be4ff4b3394070be986a207e367235822
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.10.4` - linux; amd64

```console
$ docker pull elasticsearch@sha256:3084fdc165cd1239d199fc0fde82b8db6c6b4aba0715c9b945ac1af6884b47ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **661.9 MB (661876440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a14b77fb5e8fa57f80d23b8aab8972dfda263a3060f2553430d71e3fbcb1a4`
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
# Wed, 11 Oct 2023 22:11:04 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Wed, 11 Oct 2023 22:11:05 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Wed, 11 Oct 2023 22:11:05 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 11 Oct 2023 22:11:05 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 11 Oct 2023 22:11:36 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Wed, 11 Oct 2023 22:11:36 GMT
COPY /bin/tini /bin/tini # buildkit
# Wed, 11 Oct 2023 22:11:36 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:11:36 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Wed, 11 Oct 2023 22:11:37 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Wed, 11 Oct 2023 22:11:37 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Wed, 11 Oct 2023 22:11:38 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Wed, 11 Oct 2023 22:11:38 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Wed, 11 Oct 2023 22:11:38 GMT
LABEL org.label-schema.build-date=2023-10-11T22:04:35.506990650Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=b4a62ac808e886ff032700c391f45f1408b2538c org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.10.4 org.opencontainers.image.created=2023-10-11T22:04:35.506990650Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=b4a62ac808e886ff032700c391f45f1408b2538c org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.10.4
# Wed, 11 Oct 2023 22:11:38 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 22:11:38 GMT
CMD ["eswrapper"]
# Wed, 11 Oct 2023 22:11:38 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55683f03886b517ea2e1f90b6789d2f9cf1e37e297525cd56a7a9d0e7f046a28`  
		Last Modified: Tue, 17 Oct 2023 12:30:27 GMT  
		Size: 14.1 MB (14103620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8001bda6ed4564ca84e5de39b0b31a8c9fa120442ddee3aa1f5f834d9094e64f`  
		Last Modified: Tue, 17 Oct 2023 12:30:24 GMT  
		Size: 4.3 KB (4340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4972d9cd2d15c68c6605d4b32d5aa2bcf60748190d5a5321aba0088bcfd1bb`  
		Last Modified: Tue, 17 Oct 2023 12:31:26 GMT  
		Size: 618.9 MB (618875004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc98de9d3c273d6d817c6101faeab454359d003a600286960612a5abaed91e2`  
		Last Modified: Tue, 17 Oct 2023 12:30:22 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ab6623b7ddaa40703859bb51d839019b517961ba6aecc35792765053017616`  
		Last Modified: Tue, 17 Oct 2023 12:30:22 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a483bbf6ec8d8ab8d93acb5413445582b966a457edb046881c3a8e6431746091`  
		Last Modified: Tue, 17 Oct 2023 12:30:22 GMT  
		Size: 191.9 KB (191871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3681483de1da2d0f1a2d972e72221098e1ea92b14c49c91d139dbb6905bc2a`  
		Last Modified: Tue, 17 Oct 2023 12:30:21 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c089f82855866f0884e0d2691833405c8627c2a8c3b23257c002fb43b5ecaa`  
		Last Modified: Tue, 17 Oct 2023 12:30:21 GMT  
		Size: 109.2 KB (109240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.10.4` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:5adb2c2025632c04f61c3b00dfb76a308b8c899c31cae257586ef7187cda4f13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.0 MB (453952593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e277ee668b41c5c904a91b08b66d0e2d362b00d6c96a85f57a68624d28c01e77`
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
# Wed, 11 Oct 2023 22:12:35 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Wed, 11 Oct 2023 22:12:38 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Wed, 11 Oct 2023 22:12:38 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 11 Oct 2023 22:12:38 GMT
WORKDIR /usr/share/elasticsearch
# Wed, 11 Oct 2023 22:12:41 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Wed, 11 Oct 2023 22:12:41 GMT
COPY /bin/tini /bin/tini # buildkit
# Wed, 11 Oct 2023 22:12:41 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Oct 2023 22:12:41 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Wed, 11 Oct 2023 22:12:42 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Wed, 11 Oct 2023 22:12:42 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Wed, 11 Oct 2023 22:12:44 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Wed, 11 Oct 2023 22:12:44 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Wed, 11 Oct 2023 22:12:44 GMT
LABEL org.label-schema.build-date=2023-10-11T22:04:35.506990650Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=b4a62ac808e886ff032700c391f45f1408b2538c org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.10.4 org.opencontainers.image.created=2023-10-11T22:04:35.506990650Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=b4a62ac808e886ff032700c391f45f1408b2538c org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.10.4
# Wed, 11 Oct 2023 22:12:44 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Wed, 11 Oct 2023 22:12:44 GMT
CMD ["eswrapper"]
# Wed, 11 Oct 2023 22:12:44 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d95eb8231422a9f01413f2a8643a50d5b4f6d2110da904eb7e6fd9bea96aa29`  
		Last Modified: Thu, 02 Nov 2023 23:40:04 GMT  
		Size: 12.9 MB (12853544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f270fa135f5081e6163f3304e54c7b9dbbe39478e5d84198ecaef22f943c869d`  
		Last Modified: Thu, 02 Nov 2023 23:40:02 GMT  
		Size: 4.4 KB (4357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68654a7d9a6aa09e40d1c9a1a423fb520918cd4f3a2c6bf7cf7ce2d590a3049`  
		Last Modified: Thu, 02 Nov 2023 23:40:23 GMT  
		Size: 413.6 MB (413587686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab37834942f171839a99bd32fa0ca40d5aad810ebd4cd73d547081141521b3b`  
		Last Modified: Thu, 02 Nov 2023 23:39:59 GMT  
		Size: 9.1 KB (9097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5682219c29d5268b392af0a3bf7153605ce2d44f1f161f557901b99c9cbeda`  
		Last Modified: Thu, 02 Nov 2023 23:39:59 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cbc45dad72cdb5cd6fad14b3566846074c3613c2b62b25936f3d74029cb3ea`  
		Last Modified: Thu, 02 Nov 2023 23:39:59 GMT  
		Size: 185.9 KB (185906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eea32d954d5e82eaaaf7912750e11e747303fea6d5c775d40ab16afcf215602`  
		Last Modified: Thu, 02 Nov 2023 23:39:59 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c1fce5ba86ebc1c64ed5d99e1df644638cc814ebadd1d21f793accc66fbb70`  
		Last Modified: Thu, 02 Nov 2023 23:40:04 GMT  
		Size: 109.2 KB (109246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
