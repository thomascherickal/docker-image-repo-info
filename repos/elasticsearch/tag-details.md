<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `elasticsearch`

-	[`elasticsearch:7.17.7`](#elasticsearch7177)
-	[`elasticsearch:8.5.1`](#elasticsearch851)

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

## `elasticsearch:8.5.1`

```console
$ docker pull elasticsearch@sha256:42b0e010a68cdbf951f273a4cc2320924d0873a6e13da7988c362f2f2e619f26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `elasticsearch:8.5.1` - linux; amd64

```console
$ docker pull elasticsearch@sha256:82560db72e740db62d5c172b7aee8837887f6e22b7f6dc022ab11028906c29b8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **623.7 MB (623727942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4620cd27bd0baf642c43f315363cc605c83d2f685b0a81842ee8e748730825`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Thu, 10 Nov 2022 01:14:38 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Thu, 10 Nov 2022 01:14:38 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Thu, 10 Nov 2022 01:14:39 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 10 Nov 2022 01:14:39 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 10 Nov 2022 01:14:55 GMT
COPY --chown=0:0dir:a98978f141efd1d551b3e600fab272aa0c4d52ef2c496c193d1455b03707399f in /usr/share/elasticsearch 
# Thu, 10 Nov 2022 01:14:56 GMT
COPY --chown=0:0file:fcc427e6b1b34164533c7d80cf8bba68e6f09d5c7d442ca055586359d7076e62 in /bin/tini 
# Thu, 10 Nov 2022 01:14:56 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 01:14:56 GMT
COPY file:480ac78aea3a6b2b78f3489c03400c7b30d7129a2955fcf04b47c6666f033929 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Nov 2022 01:14:57 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Thu, 10 Nov 2022 01:14:57 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Thu, 10 Nov 2022 01:14:58 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Thu, 10 Nov 2022 01:14:58 GMT
EXPOSE 9200 9300
# Thu, 10 Nov 2022 01:14:58 GMT
LABEL org.label-schema.build-date=2022-11-10T01:11:48.960945694Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=c1310c45fc534583afe2c1c03046491efba2bba2 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.5.1 org.opencontainers.image.created=2022-11-10T01:11:48.960945694Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=c1310c45fc534583afe2c1c03046491efba2bba2 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.5.1
# Thu, 10 Nov 2022 01:14:58 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 01:14:58 GMT
CMD ["eswrapper"]
# Thu, 10 Nov 2022 01:14:58 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965e7f7759554cb5e19077823ad8c79353fea41dfa0387d776de064b50e75dc3`  
		Last Modified: Wed, 16 Nov 2022 04:52:30 GMT  
		Size: 7.5 MB (7487483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b7f2b20b8059de98d44df22af47d1a3e5fbd2b9572fe80466da32b56c5d9f8`  
		Last Modified: Wed, 16 Nov 2022 04:52:29 GMT  
		Size: 4.3 KB (4340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01164aa77a22e3003f85ede54138f09471b42685fa4abbf1e9f9a93242eab0aa`  
		Last Modified: Wed, 16 Nov 2022 04:53:20 GMT  
		Size: 587.4 MB (587352329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af1ff287ecd4997f976fd8102abb4ac0b5363bcb5d24e4c2e59fbf05951f8a2`  
		Last Modified: Wed, 16 Nov 2022 04:52:29 GMT  
		Size: 9.5 KB (9529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e38c4483f8add36fb39bcecc02b485142bb3f85fd342883ad81a3e1e4c4a342`  
		Last Modified: Wed, 16 Nov 2022 04:52:27 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9cb0f94a822ffef79b71840f7ec131fc43b349bd3fc2006c8f7bb6906ab57b`  
		Last Modified: Wed, 16 Nov 2022 04:52:27 GMT  
		Size: 191.9 KB (191874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e00cd6fa2168a17e1f6bc477eb1624618f128dd0b78df22b875fa8110e354f`  
		Last Modified: Wed, 16 Nov 2022 04:52:27 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80b815049dde495eab58bbc07d035f4ad9bd097402b23de009c07e286cb9a1e`  
		Last Modified: Wed, 16 Nov 2022 04:52:27 GMT  
		Size: 102.4 KB (102420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elasticsearch:8.5.1` - linux; arm64 variant v8

```console
$ docker pull elasticsearch@sha256:99571e76b4ba7719366bb41e21794edfc8419c0b5cf63e318203a34e5b5db7b7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.1 MB (419111915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a178ff33421001fa6dad339dc2438162a298a3d5c37f69c10fbc7596bd1e198f`
-	Entrypoint: `["\/bin\/tini","--","\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["eswrapper"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Thu, 10 Nov 2022 01:16:20 GMT
RUN yes no | dpkg-reconfigure dash &&     for iter in 1 2 3 4 5 6 7 8 9 10; do       export DEBIAN_FRONTEND=noninteractive &&       apt-get update &&       apt-get upgrade -y &&       apt-get install -y --no-install-recommends         ca-certificates curl netcat p11-kit unzip zip  &&       apt-get clean &&       rm -rf /var/lib/apt/lists/* &&       exit_code=0 && break ||         exit_code=$? && echo "apt-get error: retry $iter in 10s" && sleep 10;     done;     exit $exit_code
# Thu, 10 Nov 2022 01:16:21 GMT
RUN groupadd -g 1000 elasticsearch &&     adduser --uid 1000 --gid 1000 --home /usr/share/elasticsearch elasticsearch &&     adduser elasticsearch root &&     chown -R 0:0 /usr/share/elasticsearch
# Thu, 10 Nov 2022 01:16:21 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 10 Nov 2022 01:16:21 GMT
WORKDIR /usr/share/elasticsearch
# Thu, 10 Nov 2022 01:16:27 GMT
COPY --chown=0:0dir:be72150d3d4e1b2ee41eb1739f5f6a7fa05a961394906186fc5f9a7b3fa070bf in /usr/share/elasticsearch 
# Thu, 10 Nov 2022 01:16:31 GMT
COPY --chown=0:0file:caaa172ee884dfa2de4269dce2215a63f709c6ea183f02cb82e252b7753b9772 in /bin/tini 
# Thu, 10 Nov 2022 01:16:31 GMT
ENV PATH=/usr/share/elasticsearch/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Nov 2022 01:16:31 GMT
COPY file:480ac78aea3a6b2b78f3489c03400c7b30d7129a2955fcf04b47c6666f033929 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Nov 2022 01:16:32 GMT
RUN chmod g=u /etc/passwd &&     chmod 0555 /usr/local/bin/docker-entrypoint.sh &&     find / -xdev -perm -4000 -exec chmod ug-s {} + &&     chmod 0775 /usr/share/elasticsearch &&     chown elasticsearch bin config config/jvm.options.d data logs plugins
# Thu, 10 Nov 2022 01:16:32 GMT
COPY file:12a03e8b4b92c72f58aeb5fcc5d8c6ce94ffb52fa4e13b04e23229fa535fedc0 in /etc/ca-certificates/update.d/docker-openjdk 
# Thu, 10 Nov 2022 01:16:33 GMT
RUN /etc/ca-certificates/update.d/docker-openjdk
# Thu, 10 Nov 2022 01:16:33 GMT
EXPOSE 9200 9300
# Thu, 10 Nov 2022 01:16:33 GMT
LABEL org.label-schema.build-date=2022-11-10T01:13:39.654260785Z org.label-schema.license=Elastic-License-2.0 org.label-schema.name=Elasticsearch org.label-schema.schema-version=1.0 org.label-schema.url=https://www.elastic.co/products/elasticsearch org.label-schema.usage=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.label-schema.vcs-ref=c1310c45fc534583afe2c1c03046491efba2bba2 org.label-schema.vcs-url=https://github.com/elastic/elasticsearch org.label-schema.vendor=Elastic org.label-schema.version=8.5.1 org.opencontainers.image.created=2022-11-10T01:13:39.654260785Z org.opencontainers.image.documentation=https://www.elastic.co/guide/en/elasticsearch/reference/index.html org.opencontainers.image.licenses=Elastic-License-2.0 org.opencontainers.image.revision=c1310c45fc534583afe2c1c03046491efba2bba2 org.opencontainers.image.source=https://github.com/elastic/elasticsearch org.opencontainers.image.title=Elasticsearch org.opencontainers.image.url=https://www.elastic.co/products/elasticsearch org.opencontainers.image.vendor=Elastic org.opencontainers.image.version=8.5.1
# Thu, 10 Nov 2022 01:16:33 GMT
ENTRYPOINT ["/bin/tini" "--" "/usr/local/bin/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 01:16:34 GMT
CMD ["eswrapper"]
# Thu, 10 Nov 2022 01:16:34 GMT
USER elasticsearch:root
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcb8dce094ed1437ea24b71aaca4138c1479bf78450c27b1a6d6340b001ea22`  
		Last Modified: Wed, 16 Nov 2022 19:42:29 GMT  
		Size: 7.3 MB (7312879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eccd95358444b26589a549e5abdc7fe09d4a91ace0627e3cb16d41aedd3244a`  
		Last Modified: Wed, 16 Nov 2022 19:42:28 GMT  
		Size: 4.4 KB (4383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd68f4540811abdcac9e080f2adcc41b7be6f2191d70d7e7704366323b16a66`  
		Last Modified: Wed, 16 Nov 2022 19:42:49 GMT  
		Size: 384.3 MB (384299123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d1efa60a1d176af65db3b185cced8add99eebdeb81a3496df59d4d84e48fa0`  
		Last Modified: Wed, 16 Nov 2022 19:42:26 GMT  
		Size: 9.1 KB (9096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b985a6ae22c6cc0fcb3371f64772801c74357264a13207ddde207f3eba68d8a`  
		Last Modified: Wed, 16 Nov 2022 19:42:26 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca8fe546cfe9db4e2ebda8fefb9a6d1f6b159f6e68989b71ca97d50fdb9ac4d`  
		Last Modified: Wed, 16 Nov 2022 19:42:26 GMT  
		Size: 185.9 KB (185886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fb9375d16632ba13fbb89a9e50873b6a58a6b3da522e4bac3d286e149d7025`  
		Last Modified: Wed, 16 Nov 2022 19:42:26 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d76143362bd4ea5960d71a7281317af87f6ca7f69bb8dd6b8d8620cdd7702`  
		Last Modified: Wed, 16 Nov 2022 19:42:30 GMT  
		Size: 102.4 KB (102417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
