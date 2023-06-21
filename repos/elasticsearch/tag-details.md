<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.10`](#elasticsearch71710)
-	[`elasticsearch:8.8.1`](#elasticsearch881)

## `elasticsearch:7.17.10`

```console
$ docker pull elasticsearch@sha256:43b9e781ebb2bd731ea3966bb816edce947e34965676046b3c0f8c17318cee72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.17.10` - linux; amd64

```console
$ docker pull elasticsearch@sha256:81facec55eceeb7bebeed80af49eb9a05fce77709b231210f343ac8b9599098e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.1 MB (355054430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a305059888ba801d416b5c586108895e4f650557856a19572d3f815b160e1d38`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Sun, 23 Apr 2023 05:37:54 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Sun, 23 Apr 2023 05:37:55 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Sun, 23 Apr 2023 05:37:55 GMT
ENV ELASTIC_CONTAINER=true
# Sun, 23 Apr 2023 05:37:55 GMT
WORKDIR /usr/share/elasticsearch
# Sun, 23 Apr 2023 05:38:12 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Sun, 23 Apr 2023 05:38:12 GMT
COPY /bin/tini /bin/tini # buildkit
# Sun, 23 Apr 2023 05:38:12 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 23 Apr 2023 05:38:12 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Sun, 23 Apr 2023 05:38:13 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Sun, 23 Apr 2023 05:38:13 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Sun, 23 Apr 2023 05:38:14 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Sun, 23 Apr 2023 05:38:14 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Sun, 23 Apr 2023 05:38:14 GMT
LABEL org.label-schema.build-date=2023-04-23T05:33:18.138275597Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=fecd68e3150eda0c307ab9a9d7557f5d5fd71349 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.10 org.opencontainers.image.created=2023-04-23T05:33:18.138275597Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=fecd68e3150eda0c307ab9a9d7557f5d5fd71349 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.10
# Sun, 23 Apr 2023 05:38:14 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Sun, 23 Apr 2023 05:38:14 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12bd77ba010a976d7845656c4f0cf9affa73cb9ad95aa165e7d799e422051ee`  
		Last Modified: Tue, 02 May 2023 23:55:47 GMT  
		Size: 7.5 MB (7488523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1301fe510917887796b5e67371d1ed9ef8e58e416aa142ac2de6f4bdf754bbd2`  
		Last Modified: Tue, 02 May 2023 23:55:46 GMT  
		Size: 4.3 KB (4341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b84f24899a89b9d0bc4a1bde480e2b09c7ddd4d6657906225c3358734cfef27`  
		Last Modified: Tue, 02 May 2023 23:56:08 GMT  
		Size: 318.7 MB (318678941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80def0a7fa7350415c940a42467e8591b2cbf41c5204802b78e1d1150d8f5ee6`  
		Last Modified: Tue, 02 May 2023 23:55:44 GMT  
		Size: 9.5 KB (9526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b893bbb622cfc6c32cd4699db7907f835390ee9b308a3bb3ffa4460bd4a940`  
		Last Modified: Tue, 02 May 2023 23:55:44 GMT  
		Size: 2.0 KB (1980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb7875ab0d20d1c37f3a1085dc1e27554a71f4912d32c1baf2b3f077054c533`  
		Last Modified: Tue, 02 May 2023 23:55:44 GMT  
		Size: 192.1 KB (192127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ed52a5c81982d65b4b0984ddb103751082a0ac40c34290d65c2cdcd62010f4`  
		Last Modified: Tue, 02 May 2023 23:55:44 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6942c0cf53a513a300fcd5bd7013634d1ddd1820c2fe5207d88da2682f5ef2`  
		Last Modified: Tue, 02 May 2023 23:55:44 GMT  
		Size: 100.0 KB (99988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.17.10` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:9e3e732ae247a773ddb753abebbdf2094b2cccc74229761e270e47a9398afad7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.6 MB (351588685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02ab30907c1ff1e1a46678a04e3986b0e0c1fed4069b9c0585e649562318ae1`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Sun, 23 Apr 2023 05:38:58 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Sun, 23 Apr 2023 05:39:00 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Sun, 23 Apr 2023 05:39:00 GMT
ENV ELASTIC_CONTAINER=true
# Sun, 23 Apr 2023 05:39:00 GMT
WORKDIR /usr/share/elasticsearch
# Sun, 23 Apr 2023 05:39:04 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Sun, 23 Apr 2023 05:39:05 GMT
COPY /bin/tini /bin/tini # buildkit
# Sun, 23 Apr 2023 05:39:05 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 23 Apr 2023 05:39:05 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Sun, 23 Apr 2023 05:39:05 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Sun, 23 Apr 2023 05:39:05 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Sun, 23 Apr 2023 05:39:06 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Sun, 23 Apr 2023 05:39:06 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Sun, 23 Apr 2023 05:39:06 GMT
LABEL org.label-schema.build-date=2023-04-23T05:33:18.138275597Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=fecd68e3150eda0c307ab9a9d7557f5d5fd71349 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.10 org.opencontainers.image.created=2023-04-23T05:33:18.138275597Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=fecd68e3150eda0c307ab9a9d7557f5d5fd71349 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.10
# Sun, 23 Apr 2023 05:39:06 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Sun, 23 Apr 2023 05:39:06 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feca59924f0d86cf80613044e81bb351de559728b0da8a28d2ca2955333ee540`  
		Last Modified: Wed, 03 May 2023 00:21:29 GMT  
		Size: 7.3 MB (7309587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8d3e68fe0c3228a2c728ef6416e688266d4ac9ef13c8e4c24067e2903013e7`  
		Last Modified: Wed, 03 May 2023 00:21:28 GMT  
		Size: 4.4 KB (4358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046ebafbe7304d40fd0e6f552a9ee289fda050205f15f529fc06423fa0a1f7e2`  
		Last Modified: Wed, 03 May 2023 00:22:02 GMT  
		Size: 316.8 MB (316780680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf7ce3fa8665187fe0d08aa4e6511fd263eb0c23d633ae01315b714cd79098e`  
		Last Modified: Wed, 03 May 2023 00:21:26 GMT  
		Size: 9.1 KB (9093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0625aa8000c2aab2dcc14e5ed7f2f09c8e046d91c0f93434673563de0d4564d`  
		Last Modified: Wed, 03 May 2023 00:21:26 GMT  
		Size: 2.0 KB (1982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4048d8522fed75b092aff3b1d344939e073b97c33662ad9fb320830bfa1dc5e4`  
		Last Modified: Wed, 03 May 2023 00:21:26 GMT  
		Size: 186.2 KB (186162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03345f934121cb9b8051453128be9c8cbca5dd9b13dd4608424c221ebd6c3b9`  
		Last Modified: Wed, 03 May 2023 00:21:26 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffd0f00782dcf135cef9f641cf729c91315da45477bf364da5f0b0621446242`  
		Last Modified: Wed, 03 May 2023 00:21:26 GMT  
		Size: 100.0 KB (99985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:8.8.1`

```console
$ docker pull elasticsearch@sha256:e31753d052509353f99be86892bf5c65a070805aadbb295d1b3128163061ea68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.8.1` - linux; amd64

```console
$ docker pull elasticsearch@sha256:c6268f420d8d15de1e5212b322b86acabf1690640920d26ed405db96b68eb673
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **643.0 MB (643049199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8552a239ee1e62b3bc7d1ab3d7537b33ec2b9b7931ccf65f4283962fbfa092cc`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Mon, 05 Jun 2023 21:39:21 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Mon, 05 Jun 2023 21:39:23 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Mon, 05 Jun 2023 21:39:23 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 05 Jun 2023 21:39:23 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 05 Jun 2023 21:39:50 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Mon, 05 Jun 2023 21:39:51 GMT
COPY /bin/tini /bin/tini # buildkit
# Mon, 05 Jun 2023 21:39:51 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Jun 2023 21:39:51 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Mon, 05 Jun 2023 21:39:52 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Mon, 05 Jun 2023 21:39:52 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 05 Jun 2023 21:39:53 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 05 Jun 2023 21:39:53 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Mon, 05 Jun 2023 21:39:53 GMT
LABEL org.label-schema.build-date=2023-06-05T21:32:25.188464208Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=f8edfccba429b6477927a7c1ce1bc6729521305e org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.8.1 org.opencontainers.image.created=2023-06-05T21:32:25.188464208Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=f8edfccba429b6477927a7c1ce1bc6729521305e org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.8.1
# Mon, 05 Jun 2023 21:39:53 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 05 Jun 2023 21:39:53 GMT
CMD ["eswrapper"]
# Mon, 05 Jun 2023 21:39:53 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be80ab3482c783c18390a4e7025b9f275f0accfd4260cf05df9472b3d751a8c8`  
		Last Modified: Fri, 09 Jun 2023 06:05:46 GMT  
		Size: 10.2 MB (10234350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d8cdf4255b130324eab09f8157c3a7e979f68880f0fb3ad27a3fdb4c90a5e1`  
		Last Modified: Fri, 09 Jun 2023 06:05:45 GMT  
		Size: 4.3 KB (4342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d156df27c7a2107146409802adc7daed10bcae57d8271305bde9d6a4f488031a`  
		Last Modified: Fri, 09 Jun 2023 06:06:35 GMT  
		Size: 603.9 MB (603919140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f70a6c0a491e77c9904144f1114e839fa1a21889da252e7cd47b1c63ecfec08`  
		Last Modified: Fri, 09 Jun 2023 06:05:44 GMT  
		Size: 9.5 KB (9530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d022c77db7212d953bd3d9059474527fda18cb411283e6df3a5fe30f9e6da55`  
		Last Modified: Fri, 09 Jun 2023 06:05:43 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b139178bd8216d72df81e68bdf003caac33b8f210850f67cf77fc7ac89c4289a`  
		Last Modified: Fri, 09 Jun 2023 06:05:43 GMT  
		Size: 191.9 KB (191869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1ebbdcf04297196b949aa4549b5b27707e9239354d1e33a379c5394e36f0e5`  
		Last Modified: Fri, 09 Jun 2023 06:05:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d5ce1e1e82f76b644b800a8d77a4fa7c17ca7919b0bc38eff05d387d6d4175`  
		Last Modified: Fri, 09 Jun 2023 06:05:42 GMT  
		Size: 109.2 KB (109242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.8.1` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:605d9197817e3a5991aab6e89f555d518d80d88681b33463adc64db6e06cb33b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **436.3 MB (436303952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e80ec76da7dc35ec13d2294b51ccbe0f977e3dad172032710279258b6df2d038`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Mon, 05 Jun 2023 21:39:50 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Mon, 05 Jun 2023 21:39:53 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Mon, 05 Jun 2023 21:39:53 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 05 Jun 2023 21:39:53 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 05 Jun 2023 21:40:00 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Mon, 05 Jun 2023 21:40:00 GMT
COPY /bin/tini /bin/tini # buildkit
# Mon, 05 Jun 2023 21:40:00 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Jun 2023 21:40:00 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Mon, 05 Jun 2023 21:40:11 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Mon, 05 Jun 2023 21:40:14 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 05 Jun 2023 21:40:17 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Mon, 05 Jun 2023 21:40:17 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Mon, 05 Jun 2023 21:40:17 GMT
LABEL org.label-schema.build-date=2023-06-05T21:32:25.188464208Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=f8edfccba429b6477927a7c1ce1bc6729521305e org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.8.1 org.opencontainers.image.created=2023-06-05T21:32:25.188464208Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=f8edfccba429b6477927a7c1ce1bc6729521305e org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.8.1
# Mon, 05 Jun 2023 21:40:17 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 05 Jun 2023 21:40:17 GMT
CMD ["eswrapper"]
# Mon, 05 Jun 2023 21:40:17 GMT
USER 1000:0
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7779814f25c50f37a3db37ef6f59b54e5aa125064216136e0a68c10b011c73c`  
		Last Modified: Wed, 21 Jun 2023 20:36:19 GMT  
		Size: 10.0 MB (10000644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa27bb7ecb9b3cea9985f4e97ccba78f10d7bd2e785d1464cb90defc92825dfd`  
		Last Modified: Wed, 21 Jun 2023 20:36:17 GMT  
		Size: 4.4 KB (4359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a087a6579ed9d51e72f7f53ddf0f747f9d8ca941bcb42faed2990125d7de76`  
		Last Modified: Wed, 21 Jun 2023 20:36:39 GMT  
		Size: 398.8 MB (398796140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5ce013d4813eb01e6408be5d332c9896ee3f004155d3cbcfa6311357c257c9`  
		Last Modified: Wed, 21 Jun 2023 20:36:15 GMT  
		Size: 9.1 KB (9097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13f5fac5998e325d718b2ce72063401d286f40c5384814c1e15c612ddd3a2a5`  
		Last Modified: Wed, 21 Jun 2023 20:36:15 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fb2a62763a801a5eaef678cfd0fa4a07810b4d860ba74a799fb81da09db46a`  
		Last Modified: Wed, 21 Jun 2023 20:36:15 GMT  
		Size: 185.9 KB (185905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1239c6c87a6e5580b9421321d4faa5fb1e9e499c38282ed972efa31635a9d83a`  
		Last Modified: Wed, 21 Jun 2023 20:36:15 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b939cf93d53ead2b33cd5ad616a72eb8a0df7b9b0642af82d0505f052e8eb34`  
		Last Modified: Wed, 21 Jun 2023 20:36:19 GMT  
		Size: 109.2 KB (109246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
