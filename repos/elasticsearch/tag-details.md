<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.7`](#elasticsearch7177)
-	[`elasticsearch:8.5.0`](#elasticsearch850)

## `elasticsearch:7.17.7`

```console
$ docker pull elasticsearch@sha256:bb22e1ef1707314b30020c84f29e25bc0aa80a50616a196526e38069fbd95c1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:7.17.7` - linux; amd64

```console
$ docker pull elasticsearch@sha256:8ee5c469f80e39b6cf508b543b72dcd19e83f093099f542cf271fa3dff06d5ae
```

-	Docker Version: 20.10.19
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.1 MB (353078094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec081739526313e5fcfdd125899c346a4e732fe3590bb5b2d6c6b1513bc71a35`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Mon, 17 Oct 2022 19:32:06 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Mon, 17 Oct 2022 19:32:07 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Mon, 17 Oct 2022 19:32:08 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 17 Oct 2022 19:32:08 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 17 Oct 2022 19:32:15 GMT
COPY --chown=0:0dir:cbfb429d0144d1d671bffc51c3db72ff6cc9f4f3e38b30203a3df484aea6b1e6 in /usr/share/elasticsearch 
# Mon, 17 Oct 2022 19:32:18 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Mon, 17 Oct 2022 19:32:18 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Oct 2022 19:32:18 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Mon, 17 Oct 2022 19:32:19 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Mon, 17 Oct 2022 19:32:19 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Mon, 17 Oct 2022 19:32:20 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Mon, 17 Oct 2022 19:32:20 GMT
EXPOSE 9200 9300
# Mon, 17 Oct 2022 19:32:20 GMT
LABEL org.label-schema.build-date=2022-10-17T19:29:41.425804264Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=78dcaaa8cee33438b91eca7f5c7f56a70fec9e80 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.7 org.opencontainers.image.created=2022-10-17T19:29:41.425804264Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=78dcaaa8cee33438b91eca7f5c7f56a70fec9e80 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.7
# Mon, 17 Oct 2022 19:32:21 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 17 Oct 2022 19:32:21 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38dd47397c9661cecd555176f20a2255247298ade13fa74b3f1346b74a944e5e`  
		Last Modified: Tue, 25 Oct 2022 11:51:53 GMT  
		Size: 7.8 MB (7835878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cc04abc7e0971e3ef90245210dc164413adda04cbbae2a76c3830a8acbf0f8`  
		Last Modified: Tue, 25 Oct 2022 11:51:45 GMT  
		Size: 4.3 KB (4335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5db66d71d32e2a4c3ee4b7613657672be060ed33fb49f2204ad42cfeaa9b6c`  
		Last Modified: Tue, 25 Oct 2022 11:52:30 GMT  
		Size: 316.4 MB (316356949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e314b07b4a41d4bd52199fa821cb4e58fe05b29e7724190207173205a7c55839`  
		Last Modified: Tue, 25 Oct 2022 11:51:45 GMT  
		Size: 9.5 KB (9529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cbe2363e681b91dc597e1d39f8175396b7db5817d44eeb3f76af8d3405d0ee`  
		Last Modified: Tue, 25 Oct 2022 11:51:45 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec6881665fbf286ae9fdae6f4e014d012f604017780726da41466b86cb9834d`  
		Last Modified: Tue, 25 Oct 2022 11:51:44 GMT  
		Size: 192.1 KB (192139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a24512c722108823662e4537da1a154001999c72c3edd40979891e716f6160`  
		Last Modified: Tue, 25 Oct 2022 11:51:44 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d802e5d0597d1b4b910c876478380ac9a936492ca10d24eb99729d1f8f231f`  
		Last Modified: Tue, 25 Oct 2022 11:51:44 GMT  
		Size: 102.4 KB (102421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:7.17.7` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:4e456210ad045e8c2e71fc757f46da9b8b035a589caa57f6b98da92f89547641
```

-	Docker Version: 20.10.19
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.9 MB (349948977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c7d96debc9d30e6f99e98641695c8b44fe2e75d1072aa566b57dc4eed34f09`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Mon, 17 Oct 2022 19:33:09 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Mon, 17 Oct 2022 19:33:10 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Mon, 17 Oct 2022 19:33:10 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 17 Oct 2022 19:33:10 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 17 Oct 2022 19:33:15 GMT
COPY --chown=0:0dir:442b2e05fbe59277941d1b1045e3ce4d8bc3d0f01530e6cba28d90f0376b9e99 in /usr/share/elasticsearch 
# Mon, 17 Oct 2022 19:33:19 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Mon, 17 Oct 2022 19:33:19 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 17 Oct 2022 19:33:19 GMT
COPY file:35bdfc6ad8079cb9cab605169a09ebfe8ce26cd4a9e4120efe12f418073a9bfb in /usr/local/bin/docker-entrypoint.sh 
# Mon, 17 Oct 2022 19:33:20 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Mon, 17 Oct 2022 19:33:20 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Mon, 17 Oct 2022 19:33:20 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Mon, 17 Oct 2022 19:33:20 GMT
EXPOSE 9200 9300
# Mon, 17 Oct 2022 19:33:20 GMT
LABEL org.label-schema.build-date=2022-10-17T19:31:01.853349037Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=78dcaaa8cee33438b91eca7f5c7f56a70fec9e80 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=7.17.7 org.opencontainers.image.created=2022-10-17T19:31:01.853349037Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=78dcaaa8cee33438b91eca7f5c7f56a70fec9e80 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=7.17.7
# Mon, 17 Oct 2022 19:33:21 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 17 Oct 2022 19:33:21 GMT
CMD ["eswrapper"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fb772f3aa0b7617c189a791b2626db6ca7a36379e6cd3af495f9e682f516a0`  
		Last Modified: Wed, 26 Oct 2022 20:23:16 GMT  
		Size: 7.7 MB (7654532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958897edaf7ac53f4443dd9fe18860d100d0f8ac7e9958ad2965cb597be92881`  
		Last Modified: Wed, 26 Oct 2022 20:23:15 GMT  
		Size: 4.4 KB (4363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08fedfc6594de363c61df1d412c4533e6ae78de3640bf2c8de9064446f28dcd`  
		Last Modified: Wed, 26 Oct 2022 20:23:35 GMT  
		Size: 314.8 MB (314798397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7564d3ff4f93c09c8c094b098b259b546ed7032074c9ba6ce3636354361b9277`  
		Last Modified: Wed, 26 Oct 2022 20:23:12 GMT  
		Size: 9.1 KB (9096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951a2253715ab74b864db039e653e96d381a03f938e1ace36fb6b8a0b089c651`  
		Last Modified: Wed, 26 Oct 2022 20:23:12 GMT  
		Size: 2.0 KB (1981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38386a5ad2f6acf32792485561084b4902d9bdce427d4485edc8bb0c4ecf1547`  
		Last Modified: Wed, 26 Oct 2022 20:23:13 GMT  
		Size: 186.2 KB (186159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176a4f233e2115c55ccb247c52ef765372a0d5372a870a9d6498461f2e634137`  
		Last Modified: Wed, 26 Oct 2022 20:23:13 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457203fd2aa311a6924dd7e9cad32897e48cf13c3be7c47d7ae49cd06dadfdc6`  
		Last Modified: Wed, 26 Oct 2022 20:23:17 GMT  
		Size: 102.4 KB (102418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `elasticsearch:8.5.0`

```console
$ docker pull elasticsearch@sha256:c60b67aacf91e62e0e65ab8f5003b8a57ae97d794d61e8afc256142aa8e23ad1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.5.0` - linux; amd64

```console
$ docker pull elasticsearch@sha256:41ae63c4178160a8bf6e952349d54b653252abf1e85b412ef52b0799254e81f2
```

-	Docker Version: 20.10.20
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **626.0 MB (626010149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65719a2cfaea8f638f7f179c916885b4e5cab8ff2246e7973798d044a19391bb`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Mon, 24 Oct 2022 20:26:59 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Mon, 24 Oct 2022 20:27:00 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Mon, 24 Oct 2022 20:27:01 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 24 Oct 2022 20:27:01 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 24 Oct 2022 20:27:17 GMT
COPY --chown=0:0dir:dcf8e9bd57d9aae5cbf367464c0748648988dd6ff6cb7c287d7d4355302baf07 in /usr/share/elasticsearch 
# Mon, 24 Oct 2022 20:27:21 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Mon, 24 Oct 2022 20:27:21 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Oct 2022 20:27:21 GMT
COPY file:480ac78aea3a6b2b78f3489c03400c7b30d7129a2955fcf04b47c6666f033929 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 24 Oct 2022 20:27:22 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Mon, 24 Oct 2022 20:27:23 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Mon, 24 Oct 2022 20:27:23 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Mon, 24 Oct 2022 20:27:24 GMT
EXPOSE 9200 9300
# Mon, 24 Oct 2022 20:27:24 GMT
LABEL org.label-schema.build-date=2022-10-24T20:23:55.503438230Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=c94b4700cda13820dad5aa74fae6db185ca5c304 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.5.0 org.opencontainers.image.created=2022-10-24T20:23:55.503438230Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=c94b4700cda13820dad5aa74fae6db185ca5c304 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.5.0
# Mon, 24 Oct 2022 20:27:24 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 24 Oct 2022 20:27:24 GMT
CMD ["eswrapper"]
# Mon, 24 Oct 2022 20:27:24 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecea2b9d6eb5987d841506a05b80cf5e6decd1cea184827c4c65e163cfe88942`  
		Last Modified: Wed, 02 Nov 2022 05:28:08 GMT  
		Size: 10.0 MB (10040405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92372eb67e7800c50811f6bdc1a8fe6565d74687d67231588fc93daf67906087`  
		Last Modified: Wed, 02 Nov 2022 05:28:06 GMT  
		Size: 4.3 KB (4332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35a2c3a38c0c1a86b2b00bc459f65d3dedfa2c1245972a1920704dcda15915a`  
		Last Modified: Wed, 02 Nov 2022 05:28:58 GMT  
		Size: 587.1 MB (587085018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cac206f55a29e84ad82467834477f18ac321a4c5f1b6b79d939a54c18cb92b7`  
		Last Modified: Wed, 02 Nov 2022 05:28:06 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e55d4524e9025e5360918df4cd192b360fbe1b240061601cb32275971136e5e`  
		Last Modified: Wed, 02 Nov 2022 05:28:04 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d42bd05aab9b0c66cde675322a8a76f961e0b246f92e64ebadaf69edee3ffa5`  
		Last Modified: Wed, 02 Nov 2022 05:28:04 GMT  
		Size: 191.9 KB (191866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383da80248ab7a252fbfc5b9ced1ed4829dafadcd3b27968bee27042dbc632e8`  
		Last Modified: Wed, 02 Nov 2022 05:28:04 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f8a730fccdbe85c48f00d9d27309be17086f000ac1a2e4c5200b4b810f152d`  
		Last Modified: Wed, 02 Nov 2022 05:28:04 GMT  
		Size: 102.4 KB (102417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.5.0` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:eb796d443e41caf59a4dd2afb6b4fd5bb7e993c3c14f6ddff63c9f55cfce08d9
```

-	Docker Version: 20.10.20
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **421.3 MB (421331034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84042ee74a2a8a370ea192b764328deade3ef2472c6544d890cd5a656b61e599`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Mon, 24 Oct 2022 20:28:12 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Mon, 24 Oct 2022 20:28:13 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Mon, 24 Oct 2022 20:28:13 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 24 Oct 2022 20:28:13 GMT
WORKDIR /usr/share/elasticsearch
# Mon, 24 Oct 2022 20:28:20 GMT
COPY --chown=0:0dir:723a745f6c671dcfbed7bb2a642df5616272849f7df069e2681d36424a150f7f in /usr/share/elasticsearch 
# Mon, 24 Oct 2022 20:28:24 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Mon, 24 Oct 2022 20:28:24 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Oct 2022 20:28:24 GMT
COPY file:480ac78aea3a6b2b78f3489c03400c7b30d7129a2955fcf04b47c6666f033929 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 24 Oct 2022 20:28:24 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Mon, 24 Oct 2022 20:28:25 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Mon, 24 Oct 2022 20:28:25 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Mon, 24 Oct 2022 20:28:25 GMT
EXPOSE 9200 9300
# Mon, 24 Oct 2022 20:28:25 GMT
LABEL org.label-schema.build-date=2022-10-24T20:25:49.679675868Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=c94b4700cda13820dad5aa74fae6db185ca5c304 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.5.0 org.opencontainers.image.created=2022-10-24T20:25:49.679675868Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=c94b4700cda13820dad5aa74fae6db185ca5c304 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.5.0
# Mon, 24 Oct 2022 20:28:26 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Mon, 24 Oct 2022 20:28:26 GMT
CMD ["eswrapper"]
# Mon, 24 Oct 2022 20:28:26 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d182be6bc44123c895dfe1d069d733a9467dc73a7760553189d66e77935a7bc6`  
		Last Modified: Wed, 02 Nov 2022 18:39:54 GMT  
		Size: 9.8 MB (9804100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd0440205402b2fc62bc736e2778380a250827244dbdc67d52de777cadbbb73`  
		Last Modified: Wed, 02 Nov 2022 18:39:53 GMT  
		Size: 4.4 KB (4379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a5f176eb6590d8c5d9ef4e9c7ac7ff08e01b7b4d2fe7fbde02471cf48014ec`  
		Last Modified: Wed, 02 Nov 2022 18:40:16 GMT  
		Size: 384.0 MB (384031397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd23582b34fea255614fff51cfb619cc759fb5290109f35378ad3a6850a7320`  
		Last Modified: Wed, 02 Nov 2022 18:39:50 GMT  
		Size: 9.1 KB (9094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bbace2345a597c58b7f3b24addf9abe4559ec5c6a0a56f497f9dcab7d1962d`  
		Last Modified: Wed, 02 Nov 2022 18:39:50 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb366b99b4b9a7676b1b4f2b1cb3bd6b565dc5ec66177a1cf7b672337adc6eb`  
		Last Modified: Wed, 02 Nov 2022 18:39:50 GMT  
		Size: 185.9 KB (185898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d9ecef21b3f8ac11d71eaa6888d6c1e85f1c19d2efaccd35320e208e23c237`  
		Last Modified: Wed, 02 Nov 2022 18:39:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b5901087f8d022883dbaadb846439cc97cd31a9ab2858571c3077ed306c31`  
		Last Modified: Wed, 02 Nov 2022 18:39:54 GMT  
		Size: 102.4 KB (102410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
