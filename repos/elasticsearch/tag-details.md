<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.8`](#elasticsearch7178)
-	[`elasticsearch:8.5.2`](#elasticsearch852)

## `elasticsearch:7.17.8`

**does not exist** (yet?)

## `elasticsearch:8.5.2`

```console
$ docker pull elasticsearch@sha256:9ee7fa5787c7372a91d1666c066d57096f293d08eeb029274a294e1dd4f860fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.5.2` - linux; amd64

```console
$ docker pull elasticsearch@sha256:6eb35fbe63877945c363e4bf19b262e0e568987097c0bee7f3229c69fc6bba07
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **623.7 MB (623729394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b19437f14a3b1f662d3e8db30c7eeed88f777314e9dc64be7767f146b2637a67`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Thu, 17 Nov 2022 21:20:35 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Thu, 17 Nov 2022 21:20:36 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Thu, 17 Nov 2022 21:20:36 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 17 Nov 2022 21:20:36 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 17 Nov 2022 21:20:51 GMT
COPY --chown=0:0dir:f108133d18e0681cd7e3b65a58bb4d437bb7acfa107e5504522dbe7ec4928327 in /usr/share/elasticsearch 
# Thu, 17 Nov 2022 21:20:55 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Thu, 17 Nov 2022 21:20:55 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Nov 2022 21:20:55 GMT
COPY file:480ac78aea3a6b2b78f3489c03400c7b30d7129a2955fcf04b47c6666f033929 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Nov 2022 21:20:56 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Thu, 17 Nov 2022 21:20:56 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Thu, 17 Nov 2022 21:20:56 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Thu, 17 Nov 2022 21:20:57 GMT
EXPOSE 9200 9300
# Thu, 17 Nov 2022 21:20:57 GMT
LABEL org.label-schema.build-date=2022-11-17T21:17:54.410437150Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=a846182fa16b4ebfcc89aa3c11a11fd5adf3de04 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.5.2 org.opencontainers.image.created=2022-11-17T21:17:54.410437150Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=a846182fa16b4ebfcc89aa3c11a11fd5adf3de04 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.5.2
# Thu, 17 Nov 2022 21:20:57 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 17 Nov 2022 21:20:57 GMT
CMD ["eswrapper"]
# Thu, 17 Nov 2022 21:20:57 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9233316d9dbf357944daebd5aae308fa78615d44b32d3aedf46ec8e762277d5f`  
		Last Modified: Wed, 23 Nov 2022 04:47:01 GMT  
		Size: 7.5 MB (7487571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc27906be4d3a5e49fe2978a29c0f76395265450e59c77c1f1bef36cbcb4602`  
		Last Modified: Wed, 23 Nov 2022 04:47:00 GMT  
		Size: 4.3 KB (4331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f0f50e5d47b1e5729b07f79991d71f0a4b37aa38a255a504838917b074b9cf`  
		Last Modified: Wed, 23 Nov 2022 04:47:49 GMT  
		Size: 587.4 MB (587353718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d069760f90418d3e61dac0a61737d162bbfbf109ab539a4089d26eda139773c8`  
		Last Modified: Wed, 23 Nov 2022 04:46:59 GMT  
		Size: 9.5 KB (9526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8e11fd7a9a7e9dad0ee7016e05b2be22c6695b4827237a04bb22c1d52babef`  
		Last Modified: Wed, 23 Nov 2022 04:46:58 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e687db3011a12e1b95f548114be3a6904c17ec34a3002fc1eea612eae0fdbf`  
		Last Modified: Wed, 23 Nov 2022 04:46:58 GMT  
		Size: 191.9 KB (191867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bd12c6dc1ea72e424e3d9a29c2b351139dd35b9a8b679cac3ffa0576890c20`  
		Last Modified: Wed, 23 Nov 2022 04:46:58 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b79bd3f53d9b4fa60e1f3faf83d90f2503587afc272cca137b5f57b309f5f3`  
		Last Modified: Wed, 23 Nov 2022 04:46:58 GMT  
		Size: 102.4 KB (102417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.5.2` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:8537e5cf133402803daf602197d1ca77a1af3e2580eca6ce4b5a35c612f682a2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.1 MB (419115283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3269deb053a47778f53aa0266b8b860ac2aa1a4aadf5584aff82718b1e27806`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Thu, 17 Nov 2022 21:22:22 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Thu, 17 Nov 2022 21:22:23 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Thu, 17 Nov 2022 21:22:23 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 17 Nov 2022 21:22:23 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 17 Nov 2022 21:22:29 GMT
COPY --chown=0:0dir:19ddff23ed3c3c2da79ab4025094a4fa79f97b7d9c186c9071d0fe025da395b9 in /usr/share/elasticsearch 
# Thu, 17 Nov 2022 21:22:33 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Thu, 17 Nov 2022 21:22:33 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Nov 2022 21:22:33 GMT
COPY file:480ac78aea3a6b2b78f3489c03400c7b30d7129a2955fcf04b47c6666f033929 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Nov 2022 21:22:34 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Thu, 17 Nov 2022 21:22:34 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Thu, 17 Nov 2022 21:22:35 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Thu, 17 Nov 2022 21:22:35 GMT
EXPOSE 9200 9300
# Thu, 17 Nov 2022 21:22:35 GMT
LABEL org.label-schema.build-date=2022-11-17T21:20:04.988417881Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=a846182fa16b4ebfcc89aa3c11a11fd5adf3de04 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.5.2 org.opencontainers.image.created=2022-11-17T21:20:04.988417881Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=a846182fa16b4ebfcc89aa3c11a11fd5adf3de04 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.5.2
# Thu, 17 Nov 2022 21:22:35 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 17 Nov 2022 21:22:35 GMT
CMD ["eswrapper"]
# Thu, 17 Nov 2022 21:22:35 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401c913bec1701f135a611dfc9ce27979d8d8a849a70f3872920cc4ffc14b5af`  
		Last Modified: Tue, 29 Nov 2022 01:47:08 GMT  
		Size: 7.3 MB (7312881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd29d12a258c235540b4ae20e2ea7d4f2a293d7620971ab18b8cb56f96a5bf7`  
		Last Modified: Tue, 29 Nov 2022 01:47:07 GMT  
		Size: 4.4 KB (4370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d714c768053971c5dcd76519b5e33714d13dd1ee4d00b80b9354b1e0f44d6a3e`  
		Last Modified: Tue, 29 Nov 2022 01:47:28 GMT  
		Size: 384.3 MB (384302496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b8ff0d5954a901daeb5ff4be8c1fbef05eecff22bad0ae4f4232b50aa812bc`  
		Last Modified: Tue, 29 Nov 2022 01:47:05 GMT  
		Size: 9.1 KB (9095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1552bec12dc190ea649cdf9e7bac23ba3def87ada2c2c56c37def1d566e0237`  
		Last Modified: Tue, 29 Nov 2022 01:47:05 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466c9ec2d3a13d99fe2ccbbf61b37aa1498e8989529e50790bad6da73e51c77c`  
		Last Modified: Tue, 29 Nov 2022 01:47:05 GMT  
		Size: 185.9 KB (185893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b03f5b382fea7a12f53a8d670f4350614f20371318f494be8e2582c6487eec`  
		Last Modified: Tue, 29 Nov 2022 01:47:05 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edcc9e88702f44544603c6da98077e7d92d840f83929b81d0d9d7a7eabed3e24`  
		Last Modified: Tue, 29 Nov 2022 01:47:06 GMT  
		Size: 102.4 KB (102417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
