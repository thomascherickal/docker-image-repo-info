<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:7.17.7`](#logstash7177)
-	[`logstash:8.5.0`](#logstash850)

## `logstash:7.17.7`

```console
$ docker pull logstash@sha256:93030161613312c65d84fb2ace25654badbb935604a545df91d2e93e28511bca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:7.17.7` - linux; amd64

```console
$ docker pull logstash@sha256:c23d8a62e603410c34028f910e6361a5413c5268cab04a6da8eb77a7dbcacb28
```

-	Docker Version: 20.10.18
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.5 MB (437519025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf8838e621a60b70f9d48554bcde253215e1b8b6f2e0f886202d84f07a5f73d7`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Thu, 13 Oct 2022 14:17:46 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Thu, 13 Oct 2022 14:17:47 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Thu, 13 Oct 2022 14:18:10 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.7-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.7 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Thu, 13 Oct 2022 14:18:13 GMT
WORKDIR /usr/share/logstash
# Thu, 13 Oct 2022 14:18:13 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 13 Oct 2022 14:18:13 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Oct 2022 14:18:13 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Thu, 13 Oct 2022 14:18:13 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Thu, 13 Oct 2022 14:18:13 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Thu, 13 Oct 2022 14:18:14 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Thu, 13 Oct 2022 14:18:14 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Thu, 13 Oct 2022 14:18:14 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Thu, 13 Oct 2022 14:18:14 GMT
ADD file:fa0b17daaf7e42274e538ba9365a74fea034f24924e0f813a39f5fa2e120e58c in /usr/local/bin/ 
# Thu, 13 Oct 2022 14:18:14 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Thu, 13 Oct 2022 14:18:15 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Thu, 13 Oct 2022 14:18:15 GMT
USER 1000
# Thu, 13 Oct 2022 14:18:15 GMT
EXPOSE 5044 9600
# Thu, 13 Oct 2022 14:18:15 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.7 org.opencontainers.image.version=7.17.7 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-10-13T13:24:55+00:00 org.opencontainers.image.created=2022-10-13T13:24:55+00:00
# Thu, 13 Oct 2022 14:18:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9a59914a229d8ae3e7ec7972d333a5f74aba0794a4154157f238ed4d847d70`  
		Last Modified: Wed, 26 Oct 2022 22:15:28 GMT  
		Size: 40.4 MB (40425249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b31ddf2ac4ed36ead677552e16519abf881155e7a9d81ad499aa533d6ece43e`  
		Last Modified: Wed, 26 Oct 2022 22:15:20 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162661d00d0869f2d10d158ab7cef44edc1323842d733b182465f2c508be93c3`  
		Last Modified: Wed, 26 Oct 2022 22:16:02 GMT  
		Size: 366.7 MB (366742521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706a1bf2d5e328d5e3c881a7d7d93b84c189525e9496a0231432605c5f7704db`  
		Last Modified: Wed, 26 Oct 2022 22:15:19 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741874f127b93c45780a633eceacac11ca8a53f282fb079a699fad63ea342068`  
		Last Modified: Wed, 26 Oct 2022 22:15:17 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03492354dd29643862ad76a2f876ff4466a6077fdbdbda9abc21ceb3b9c1cfc`  
		Last Modified: Wed, 26 Oct 2022 22:15:15 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5245bb90f80984f5c07f4b871ce265847bdd42892ee112ebae6b2ba3bf1096d`  
		Last Modified: Wed, 26 Oct 2022 22:15:14 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05103a3b7940af5e8174754a5f53d97b0dffe102aa39231e83724a00a65eee0d`  
		Last Modified: Wed, 26 Oct 2022 22:15:13 GMT  
		Size: 2.9 KB (2856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815ba6161ff764e95c9b924a0e57d3b5aa18680625a09fb7b1f415552cd3f7fa`  
		Last Modified: Wed, 26 Oct 2022 22:15:13 GMT  
		Size: 1.8 MB (1769694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7777f80b5df45d533f8fd71aabbaec6e9e69ba8cc62a0fbbdf05a89fa4ea52cc`  
		Last Modified: Wed, 26 Oct 2022 22:15:09 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7777f80b5df45d533f8fd71aabbaec6e9e69ba8cc62a0fbbdf05a89fa4ea52cc`  
		Last Modified: Wed, 26 Oct 2022 22:15:09 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:7.17.7` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:4281307b1f2fc77683ffa5f96376d45786f7a8776276792c78a9c2ceba7aa3f5
```

-	Docker Version: 20.10.18
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.9 MB (426896160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:018639fbc67183aa904f93bdb8e6746b3b406415bc75ae7cc90e29497e768e54`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Thu, 13 Oct 2022 13:39:23 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Thu, 13 Oct 2022 13:39:24 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Thu, 13 Oct 2022 13:39:41 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.7-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.7 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Thu, 13 Oct 2022 13:39:45 GMT
WORKDIR /usr/share/logstash
# Thu, 13 Oct 2022 13:39:45 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 13 Oct 2022 13:39:45 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 13 Oct 2022 13:39:45 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Thu, 13 Oct 2022 13:39:46 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Thu, 13 Oct 2022 13:39:46 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Thu, 13 Oct 2022 13:39:46 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Thu, 13 Oct 2022 13:39:46 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Thu, 13 Oct 2022 13:39:46 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Thu, 13 Oct 2022 13:39:46 GMT
ADD file:969bb191a8e9eeea9a2d6de82b8c4da2699144646e4913f47a776d17895433c4 in /usr/local/bin/ 
# Thu, 13 Oct 2022 13:39:47 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Thu, 13 Oct 2022 13:39:47 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Thu, 13 Oct 2022 13:39:47 GMT
USER 1000
# Thu, 13 Oct 2022 13:39:47 GMT
EXPOSE 5044 9600
# Thu, 13 Oct 2022 13:39:47 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.7 org.opencontainers.image.version=7.17.7 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-10-13T13:26:27+00:00 org.opencontainers.image.created=2022-10-13T13:26:27+00:00
# Thu, 13 Oct 2022 13:39:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c515b444af642edb8348969e482dd217ab61e162a62a4415b10f65b7b88fc58d`  
		Last Modified: Wed, 26 Oct 2022 20:31:16 GMT  
		Size: 34.5 MB (34545828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ab6351ec5a253dc95d89d1b48f98590a838dfdaca194fe85986585d78fa2b`  
		Last Modified: Wed, 26 Oct 2022 20:31:12 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a48741a584df72385b298226915e9a2ddbd8f7cb158f31861ed49d39b889eb`  
		Last Modified: Wed, 26 Oct 2022 20:31:35 GMT  
		Size: 363.5 MB (363502230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b17eeae75bed8bcce84fddcd9feb4031bc9692e0cf0a6c5bd13eaaae49b9fe`  
		Last Modified: Wed, 26 Oct 2022 20:31:12 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f011bd72ec002bc253d60c27bcb0db8cf35bcbb1b8de3163c2c7e7387187116`  
		Last Modified: Wed, 26 Oct 2022 20:31:12 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7947c840491836acd7612ef6642dc79dbcc8ec20936b8a9e14768e250d194dd`  
		Last Modified: Wed, 26 Oct 2022 20:31:10 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd905caa31f3996de53be00582a9f64b04ac13598a353d68f56e52a30691290`  
		Last Modified: Wed, 26 Oct 2022 20:31:10 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f26018ec7fd1889e89d899a75e6fdfb5d5a489951ab4e246fb27cb810edf1a`  
		Last Modified: Wed, 26 Oct 2022 20:31:10 GMT  
		Size: 2.8 KB (2849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e79f73b76442bc7bc79bb303b61788984297866ddccc14288e2e2bb2bcb7d8`  
		Last Modified: Wed, 26 Oct 2022 20:31:10 GMT  
		Size: 1.6 MB (1649383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15538e66358de9dfd77e68364776e22f9db4fc9510a0f3e18c8342b64d119273`  
		Last Modified: Wed, 26 Oct 2022 20:31:10 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15538e66358de9dfd77e68364776e22f9db4fc9510a0f3e18c8342b64d119273`  
		Last Modified: Wed, 26 Oct 2022 20:31:10 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:8.5.0`

```console
$ docker pull logstash@sha256:3b285f2133d78630d6366ba8e074d27b6352b759d908bb4334e52ec36c028a6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:8.5.0` - linux; amd64

```console
$ docker pull logstash@sha256:0dab3a9c94c0a1ac59897245da3e90366a9448127ce7569c255f5dd847c8aa4e
```

-	Docker Version: 20.10.16
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.1 MB (415144816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df0e328413e11084e22f419a873ae22e079b9072c6e5e912faf78d85b8785caf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Mon, 24 Oct 2022 17:50:42 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Mon, 24 Oct 2022 17:50:43 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Mon, 24 Oct 2022 17:51:06 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.5.0-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.5.0 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash
# Mon, 24 Oct 2022 17:51:09 GMT
WORKDIR /usr/share/logstash
# Mon, 24 Oct 2022 17:51:09 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 24 Oct 2022 17:51:09 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Oct 2022 17:51:10 GMT
COPY file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Mon, 24 Oct 2022 17:51:10 GMT
COPY file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Mon, 24 Oct 2022 17:51:10 GMT
COPY file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Mon, 24 Oct 2022 17:51:10 GMT
COPY file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Mon, 24 Oct 2022 17:51:10 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Mon, 24 Oct 2022 17:51:11 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Mon, 24 Oct 2022 17:51:11 GMT
COPY file:e900d2f1e4d24464d0910b807f0dd51edeff4b07e7ad5d84f9440dcfef0c5f6a in /usr/local/bin/ 
# Mon, 24 Oct 2022 17:51:11 GMT
COPY file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Mon, 24 Oct 2022 17:51:11 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Mon, 24 Oct 2022 17:51:11 GMT
USER 1000
# Mon, 24 Oct 2022 17:51:12 GMT
EXPOSE 5044 9600
# Mon, 24 Oct 2022 17:51:12 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.5.0 org.opencontainers.image.version=8.5.0 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-10-24T16:56:24Z org.opencontainers.image.created=2022-10-24T16:56:24Z
# Mon, 24 Oct 2022 17:51:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b102e8c1a1c3e5d4770f59846606434450effe18e03896cb26949276675b2f81`  
		Last Modified: Wed, 02 Nov 2022 13:35:47 GMT  
		Size: 42.9 MB (42876301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497564fa21361004daa0fc8657b6fb35974bcb9ae5166f9ac91c6353bcc6c1b7`  
		Last Modified: Wed, 02 Nov 2022 13:35:41 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fecfa36ca903198cea7a31f06e1856a43b7c20aec0373e72e799ba1de4eed51`  
		Last Modified: Wed, 02 Nov 2022 13:36:09 GMT  
		Size: 341.9 MB (341917260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53775651d8fd681a305cc5714d4a38d4872a470b0819d59f5f6b97b4f43309b`  
		Last Modified: Wed, 02 Nov 2022 13:35:39 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309aff6ab18bf5febbbd26ee290eebcb810ac0e6c5c0f78503bf8ea962b6e737`  
		Last Modified: Wed, 02 Nov 2022 13:35:39 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec74142c06cc9c5e299a7d7728e44baea6b946bf10cd22ae530fb14ba303ea98`  
		Last Modified: Wed, 02 Nov 2022 13:35:39 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac009607a86424e5319058b87f8f956c6805fa8a7982c3b74aa4b400a5919fa6`  
		Last Modified: Wed, 02 Nov 2022 13:35:39 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15d45abc4057ed4735dc2586bab709ea116b3b7685ffcd7935ed576dfe494ef`  
		Last Modified: Wed, 02 Nov 2022 13:35:36 GMT  
		Size: 2.7 KB (2719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f240ae687cee03d3d51d26dc2dad49cdf14a72c47d2229842bac48234b967bb`  
		Last Modified: Wed, 02 Nov 2022 13:35:37 GMT  
		Size: 1.8 MB (1769822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f274def3db6324825b336625764292340a31236a9cb8540b0a0f8f5e150b833`  
		Last Modified: Wed, 02 Nov 2022 13:35:36 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f274def3db6324825b336625764292340a31236a9cb8540b0a0f8f5e150b833`  
		Last Modified: Wed, 02 Nov 2022 13:35:36 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:8.5.0` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:eb0942510ba5e9cfb7c6f7192859f1a11bfdb91e474f5bb4f6c87402ac32ac3c
```

-	Docker Version: 20.10.20
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.3 MB (406335769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36da5e77eaa35b0c8119ea9b906db4dc977fe189823e62d78a955e54df2ea7f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Mon, 24 Oct 2022 17:13:39 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Mon, 24 Oct 2022 17:13:40 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Mon, 24 Oct 2022 17:13:58 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.5.0-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.5.0 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash
# Mon, 24 Oct 2022 17:13:59 GMT
WORKDIR /usr/share/logstash
# Mon, 24 Oct 2022 17:13:59 GMT
ENV ELASTIC_CONTAINER=true
# Mon, 24 Oct 2022 17:13:59 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 24 Oct 2022 17:14:00 GMT
COPY file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Mon, 24 Oct 2022 17:14:00 GMT
COPY file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Mon, 24 Oct 2022 17:14:00 GMT
COPY file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Mon, 24 Oct 2022 17:14:00 GMT
COPY file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Mon, 24 Oct 2022 17:14:00 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Mon, 24 Oct 2022 17:14:00 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Mon, 24 Oct 2022 17:14:00 GMT
COPY file:198c6e4b2866a58ec73ab4b7a1f4e00c313b5231ab00b1c3bac13d0c8dd2f8eb in /usr/local/bin/ 
# Mon, 24 Oct 2022 17:14:01 GMT
COPY file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Mon, 24 Oct 2022 17:14:01 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Mon, 24 Oct 2022 17:14:01 GMT
USER 1000
# Mon, 24 Oct 2022 17:14:01 GMT
EXPOSE 5044 9600
# Mon, 24 Oct 2022 17:14:01 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.5.0 org.opencontainers.image.version=8.5.0 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-10-24T16:58:08+00:00 org.opencontainers.image.created=2022-10-24T16:58:08+00:00
# Mon, 24 Oct 2022 17:14:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83db47fdd306cd0fde02d1e40d6d18f68e757793c23f4b1ae7977028ec0f3ee1`  
		Last Modified: Wed, 02 Nov 2022 18:41:58 GMT  
		Size: 36.8 MB (36800759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b754250493fe73956996f6db29b970cf7edf741c21b205b00ae901c7ed543e`  
		Last Modified: Wed, 02 Nov 2022 18:41:54 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b147479debfcc82d829036e7c66b9b7f7e3af5855895ad5b06e177b341f375`  
		Last Modified: Wed, 02 Nov 2022 18:42:16 GMT  
		Size: 340.7 MB (340686800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555f2537c9e2d2727bb461c81c1b9ae186619c20955f1f3cb8ea6e84de430156`  
		Last Modified: Wed, 02 Nov 2022 18:41:54 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3587bf345bd6331dd94e3af47806bcff0d074030dfbaaa54c0b257fa15572a`  
		Last Modified: Wed, 02 Nov 2022 18:41:54 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2776e7c7852d7c954ffa3920c4f272532014d6d169eb29bb938fde1e19901957`  
		Last Modified: Wed, 02 Nov 2022 18:41:52 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524ebb1c5a852c978a1b2f37a7afa148ef2c82fff838fd55293528bf6f3a2101`  
		Last Modified: Wed, 02 Nov 2022 18:41:51 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dc9e6b92b31ce0d48cc90c7df333d1cd844c8df4f4c0bd29dbb2688867b0cf`  
		Last Modified: Wed, 02 Nov 2022 18:41:52 GMT  
		Size: 2.7 KB (2718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1405a7274b859ee5a5aa2d64893c62fe149a9aa179aaa3796c1672a3d8cbd9`  
		Last Modified: Wed, 02 Nov 2022 18:41:52 GMT  
		Size: 1.6 MB (1649610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3043eb5634220be3742f5a42412229015483e17932e8c4110bcc44a4b7b44b45`  
		Last Modified: Wed, 02 Nov 2022 18:41:51 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3043eb5634220be3742f5a42412229015483e17932e8c4110bcc44a4b7b44b45`  
		Last Modified: Wed, 02 Nov 2022 18:41:51 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
