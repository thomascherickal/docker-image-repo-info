<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.8`](#elasticsearch7178)
-	[`elasticsearch:8.6.1`](#elasticsearch861)

## `elasticsearch:7.17.8`

```console
$ docker pull elasticsearch@sha256:fdc73b3249c1936f7a277911d58bd10bdd5cf7aae07c1f4d285cf3b7bd18e503
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.17.8` - linux; amd64

```console
$ docker pull elasticsearch@sha256:d1b1c87fcd3e6039695f9e67052865ee85568d1be343e26326a6d3b73076b7c0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.1 MB (354138324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b4df3b1f757e99cb6cee3818f1b9da9a47855741ef06d8b495283d3ad6d9cf2`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Fri, 02 Dec 2022 17:38:29 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Fri, 02 Dec 2022 17:38:30 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Fri, 02 Dec 2022 17:38:30 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 02 Dec 2022 17:38:30 GMT
WORKDIR /usr/share/elasticsearch
# Fri, 02 Dec 2022 17:38:37 GMT
COPY --chown=0:0dir:15beec23a18e3cab272ee0479a77dc21f31bc10561c3eb72a1b84cf33eb522f6 in /usr/share/elasticsearch 
# Fri, 02 Dec 2022 17:38:39 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Fri, 02 Dec 2022 17:38:39 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Dec 2022 17:38:39 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Fri, 02 Dec 2022 17:38:40 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Fri, 02 Dec 2022 17:38:40 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Fri, 02 Dec 2022 17:38:41 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Fri, 02 Dec 2022 17:38:41 GMT
EXPOSE 9200 9300
# Fri, 02 Dec 2022 17:38:41 GMT
LABEL org.label-schema.build-date=2022-12-02T17:33:09.727072865Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=120eabe1c8a0cb2ae87cffc109a5b65d213e9df1 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.8 org.opencontainers.image.created=2022-12-02T17:33:09.727072865Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=120eabe1c8a0cb2ae87cffc109a5b65d213e9df1 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.8
# Fri, 02 Dec 2022 17:38:41 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Fri, 02 Dec 2022 17:38:41 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247f12a2b5fadf2435dffd0df6cffeee9128409e488ff855ba929842da14620`  
		Last Modified: Thu, 08 Dec 2022 19:22:06 GMT  
		Size: 8.7 MB (8686061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0495283e7099e4d6b1131aff25a580571b82c9d651aa943acb4134202894f67`  
		Last Modified: Thu, 08 Dec 2022 19:22:05 GMT  
		Size: 4.3 KB (4347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7e458ee5994c2382fa67ad3d971d6afd21943861275c2f508639430f61861e`  
		Last Modified: Thu, 08 Dec 2022 19:22:29 GMT  
		Size: 316.6 MB (316563617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ffe59d0e2690f7196442d2e5098637b854fb5b5908155355d3ed3219ecac53`  
		Last Modified: Thu, 08 Dec 2022 19:22:03 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab476f874bd0ed85446659b8d33f1e3362c295451579a01d3a9c34caeca103b`  
		Last Modified: Thu, 08 Dec 2022 19:22:03 GMT  
		Size: 2.0 KB (1981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20df4c47e643927cf82d269360a02b48f1da3c9f690a29973df36207ffa69ee`  
		Last Modified: Thu, 08 Dec 2022 19:22:03 GMT  
		Size: 192.1 KB (192138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef90b430ba5b81dd4918270805f86e347cea0011a15df8349bfd241e3fd8e2cb`  
		Last Modified: Thu, 08 Dec 2022 19:22:03 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f96f41bfec89084d3adfdf2bcd6f20547fb88df452fac9f241e909800e3d3d`  
		Last Modified: Thu, 08 Dec 2022 19:22:03 GMT  
		Size: 102.4 KB (102413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.17.8` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:abb19313e30d1e56f0c2e022cce8ba743215922483c9da5cca04c718e768493e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.0 MB (351011804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17e7a751ed4f0a3ecf2e6f7c0153dc516731336b150e8ed371c8ad6af087d958`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Fri, 02 Dec 2022 17:38:45 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Fri, 02 Dec 2022 17:38:48 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Fri, 02 Dec 2022 17:38:48 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 02 Dec 2022 17:38:48 GMT
WORKDIR /usr/share/elasticsearch
# Fri, 02 Dec 2022 17:38:50 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Fri, 02 Dec 2022 17:38:50 GMT
COPY /bin/tini /bin/tini # buildkit
# Fri, 02 Dec 2022 17:38:50 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Dec 2022 17:38:50 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Fri, 02 Dec 2022 17:38:50 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Fri, 02 Dec 2022 17:38:50 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Fri, 02 Dec 2022 17:38:51 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Fri, 02 Dec 2022 17:38:51 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Fri, 02 Dec 2022 17:38:51 GMT
LABEL org.label-schema.build-date=2022-12-02T17:33:09.727072865Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=120eabe1c8a0cb2ae87cffc109a5b65d213e9df1 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.8 org.opencontainers.image.created=2022-12-02T17:33:09.727072865Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=120eabe1c8a0cb2ae87cffc109a5b65d213e9df1 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.8
# Fri, 02 Dec 2022 17:38:51 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Fri, 02 Dec 2022 17:38:51 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e203ee7abb6500800d9319317105809a398b5be3e3d1130e2178a84b8630daf`  
		Last Modified: Thu, 08 Dec 2022 18:41:16 GMT  
		Size: 8.5 MB (8490726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33638d7e763d5519b298022ea49693b7d87681bf5f29c4f8ccb03eae2f588fc`  
		Last Modified: Thu, 08 Dec 2022 18:41:15 GMT  
		Size: 4.4 KB (4360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70884ade5b8f9939665241d36329788803d678288f787c0464b856c17190aa3`  
		Last Modified: Thu, 08 Dec 2022 18:41:34 GMT  
		Size: 315.0 MB (315020612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a951d1a6de13fb838fad0ad3a08d924e12b4e930ec79196ac19929d58284259c`  
		Last Modified: Thu, 08 Dec 2022 18:41:12 GMT  
		Size: 9.1 KB (9098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9133d822c8166cee37e725eb6556f1cc7f004a7462e03d021a3eade1e14d2b25`  
		Last Modified: Thu, 08 Dec 2022 18:41:12 GMT  
		Size: 2.0 KB (1985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7974d905102e90a77a5ed48be1c49b874b8da5ede1b49e6f194e4e698aeb7f6e`  
		Last Modified: Thu, 08 Dec 2022 18:41:12 GMT  
		Size: 186.2 KB (186165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1befb3933d86201a2a9b3228b65641fec16107722b97d2640fda01f606dd030`  
		Last Modified: Thu, 08 Dec 2022 18:41:12 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf543a5a7fee5a0fb6927ef68b3cfc8d8b79d54898e7dd332d1e20b70ab73624`  
		Last Modified: Thu, 08 Dec 2022 18:41:15 GMT  
		Size: 102.4 KB (102417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:8.6.1`

```console
$ docker pull elasticsearch@sha256:6242ee491ce3bbdb60543ae31e095630da00a413fa7d3885966a0642734bb69d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.6.1` - linux; amd64

```console
$ docker pull elasticsearch@sha256:c4a01d0a2a76e2d371ba66615d5878e3e676a6a44e940656683896789f40b75e
```

-	Docker Version: 20.10.22
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **624.9 MB (624866245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:704e34a98f9ad33b8407232e648c0b0eb39a3bc96373926db18a71f5aa32298f`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:21 GMT
ADD file:9d282119af0c42bc823c95b4192a3350cf2cad670622017356dd2e637762e425 in / 
# Fri, 09 Dec 2022 01:20:21 GMT
CMD ["bash"]
# Tue, 24 Jan 2023 21:51:01 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Tue, 24 Jan 2023 21:51:03 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Tue, 24 Jan 2023 21:51:03 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 24 Jan 2023 21:51:03 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 24 Jan 2023 21:51:17 GMT
COPY --chown=0:0dir:e28ddfbe4e96637ee1a1acbe45388bf0457b103d83bd0967c8c914a0512f3082 in /usr/share/elasticsearch 
# Tue, 24 Jan 2023 21:51:21 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Tue, 24 Jan 2023 21:51:21 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 21:51:21 GMT
COPY file:480ac78aea3a6b2b78f3489c03400c7b30d7129a2955fcf04b47c6666f033929 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 24 Jan 2023 21:51:22 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Tue, 24 Jan 2023 21:51:22 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Tue, 24 Jan 2023 21:51:23 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Tue, 24 Jan 2023 21:51:23 GMT
EXPOSE 9200 9300
# Tue, 24 Jan 2023 21:51:23 GMT
LABEL org.label-schema.build-date=2023-01-24T21:35:11.506992272Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=180c9830da956993e59e2cd70eb32b5e383ea42c org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.6.1 org.opencontainers.image.created=2023-01-24T21:35:11.506992272Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=180c9830da956993e59e2cd70eb32b5e383ea42c org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.6.1
# Tue, 24 Jan 2023 21:51:23 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 24 Jan 2023 21:51:23 GMT
CMD ["eswrapper"]
# Tue, 24 Jan 2023 21:51:23 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:846c0b181fff0c667d9444f8378e8fcfa13116da8d308bf21673f7e4bea8d580`  
		Last Modified: Thu, 08 Dec 2022 13:18:11 GMT  
		Size: 28.6 MB (28576882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8808e7b116d86a4da8b904a22bdee12c02f26eb26b0d46023cbd858e669c7679`  
		Last Modified: Fri, 27 Jan 2023 03:03:42 GMT  
		Size: 7.5 MB (7486120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1575487a3b14b2d359cc7100068b44063390c2578726d87ebb461bf667707fc9`  
		Last Modified: Fri, 27 Jan 2023 03:03:40 GMT  
		Size: 4.3 KB (4337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12eebc573f38d46992aaeca582964e7e7eb8874dd720bfe6eb82e07f9671808`  
		Last Modified: Fri, 27 Jan 2023 03:04:30 GMT  
		Size: 588.5 MB (588495392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2336bb55b75a660d39665c44f2d6a424323514d9a4e3ad98846161c7ab67183`  
		Last Modified: Fri, 27 Jan 2023 03:03:40 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2665f0ae7e1eef8e6dbc300412bbbc96ea6e121ab9de5f22e8d322fc44a9c26`  
		Last Modified: Fri, 27 Jan 2023 03:03:40 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765d657a2677188c712474404128cb295c96b8e0bb0ebefc88738031745c7061`  
		Last Modified: Fri, 27 Jan 2023 03:03:40 GMT  
		Size: 191.9 KB (191869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b66c25b220395fb17bfeebcc2e841661bad902d7ef8c88996fc91b9e3dfbe9`  
		Last Modified: Fri, 27 Jan 2023 03:03:38 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90d1b00a7353e98fa74e2cc0b9ca059a9767f0d576a883946eba4aabdbe071a`  
		Last Modified: Fri, 27 Jan 2023 03:03:38 GMT  
		Size: 100.0 KB (99985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.6.1` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:7616ae747f6139d498b6b2fdd7ce8eea2721be9f0911443be5a47c323d9193b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.2 MB (420247646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4209fba45d31ec23ff4089a63e0c61d44138377b9d4e0407595f8578f9aacf`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:50 GMT
ADD file:8cba976cb6ea226de769a768ee274e7679d34f923c93392f340680dc6696232e in / 
# Fri, 09 Dec 2022 01:46:50 GMT
CMD ["bash"]
# Tue, 24 Jan 2023 21:49:41 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code # buildkit
# Tue, 24 Jan 2023 21:49:48 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch # buildkit
# Tue, 24 Jan 2023 21:49:49 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 24 Jan 2023 21:49:49 GMT
WORKDIR /usr/share/elasticsearch
# Tue, 24 Jan 2023 21:50:11 GMT
COPY /usr/share/elasticsearch /usr/share/elasticsearch # buildkit
# Tue, 24 Jan 2023 21:50:11 GMT
COPY /bin/tini /bin/tini # buildkit
# Tue, 24 Jan 2023 21:50:11 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 24 Jan 2023 21:50:11 GMT
COPY bin/docker-entrypoint.sh /usr/local/bin/docker-entrypoint.sh # buildkit
# Tue, 24 Jan 2023 21:50:12 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins # buildkit
# Tue, 24 Jan 2023 21:50:12 GMT
COPY bin/docker-openjdk /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 24 Jan 2023 21:50:13 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk # buildkit
# Tue, 24 Jan 2023 21:50:13 GMT
EXPOSE map[9200/tcp:{} 9300/tcp:{}]
# Tue, 24 Jan 2023 21:50:13 GMT
LABEL org.label-schema.build-date=2023-01-24T21:35:11.506992272Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=180c9830da956993e59e2cd70eb32b5e383ea42c org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.6.1 org.opencontainers.image.created=2023-01-24T21:35:11.506992272Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=180c9830da956993e59e2cd70eb32b5e383ea42c org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.6.1
# Tue, 24 Jan 2023 21:50:13 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Tue, 24 Jan 2023 21:50:13 GMT
CMD ["eswrapper"]
# Tue, 24 Jan 2023 21:50:13 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:f04b4bbe15805316c8fda79beedd3b77e6b1ffcd0acf81226c3089e63f6bffeb`  
		Last Modified: Thu, 08 Dec 2022 15:28:02 GMT  
		Size: 27.2 MB (27193168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f825be296d963da2d39bcf9a9d1a0ff6634ba1e14e7fc2aa7eb211dc53413fe`  
		Last Modified: Wed, 01 Feb 2023 22:05:39 GMT  
		Size: 7.3 MB (7305871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a451ffab41d6df7995adac6fe7a8f7f05f392b1ecddb1bfcf10bfaa6f66838e`  
		Last Modified: Wed, 01 Feb 2023 22:05:37 GMT  
		Size: 4.4 KB (4361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2d7b82311048c3fb0fe92d1f0a9d6bcdf04ca06a710752c84a0c854d19f1bf`  
		Last Modified: Wed, 01 Feb 2023 22:05:58 GMT  
		Size: 385.4 MB (385447098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f636ddc069b8c468096c90966d0db1d27df7256a044d80ccc534b9d7ec0278fc`  
		Last Modified: Wed, 01 Feb 2023 22:05:35 GMT  
		Size: 9.1 KB (9094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e634d2b0d5c2300d7897b316a83d786b4000e6717691a800cf94a2d51dc0881`  
		Last Modified: Wed, 01 Feb 2023 22:05:35 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fadf00d4e1576917f9f926c63b23a0da65974f994a294b9998e071cea1cd4c`  
		Last Modified: Wed, 01 Feb 2023 22:05:35 GMT  
		Size: 185.9 KB (185896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c139e97bf357309f61490094b3d193f93d7de28d40b8cc8a17174b9924e17f54`  
		Last Modified: Wed, 01 Feb 2023 22:05:35 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c935817762c5abfbcd2c07fc983f3064411be8fe126198ca1cde85826ed4d3b4`  
		Last Modified: Wed, 01 Feb 2023 22:05:39 GMT  
		Size: 100.0 KB (99993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
