<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:7.17.7`](#logstash7177)
-	[`logstash:8.5.2`](#logstash852)

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

## `logstash:8.5.2`

```console
$ docker pull logstash@sha256:368c58aec5ec75edb69e72bde8e540bc9727b3a39b23ab3b290d88cf216719f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:8.5.2` - linux; amd64

```console
$ docker pull logstash@sha256:93eba5d8682db20177b4f7b474d939ef8b46796c3e08b31d47ded17abc8c4f41
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.2 MB (413185997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7102f8c625d14e18dcea07419d0046be2c596c9edef0bb4e4b130dc51bd77ec`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 25 Oct 2022 01:53:34 GMT
ADD file:7633003155a1059419aa1a6756fafb6e4f419d65bff7feb7c945de1e29dccb1e in / 
# Tue, 25 Oct 2022 01:53:35 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 21:05:46 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Wed, 16 Nov 2022 21:05:47 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Wed, 16 Nov 2022 21:06:09 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.5.2-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.5.2 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash
# Wed, 16 Nov 2022 21:06:12 GMT
WORKDIR /usr/share/logstash
# Wed, 16 Nov 2022 21:06:13 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 16 Nov 2022 21:06:13 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 21:06:13 GMT
COPY file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Wed, 16 Nov 2022 21:06:13 GMT
COPY file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Wed, 16 Nov 2022 21:06:13 GMT
COPY file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Wed, 16 Nov 2022 21:06:13 GMT
COPY file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Wed, 16 Nov 2022 21:06:14 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Wed, 16 Nov 2022 21:06:14 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 16 Nov 2022 21:06:14 GMT
COPY file:2d39e1eff8ffafbab219bc3ddc26102e295829e559ae1314f59a12693923951c in /usr/local/bin/ 
# Wed, 16 Nov 2022 21:06:14 GMT
COPY file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Wed, 16 Nov 2022 21:06:14 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Wed, 16 Nov 2022 21:06:14 GMT
USER 1000
# Wed, 16 Nov 2022 21:06:15 GMT
EXPOSE 5044 9600
# Wed, 16 Nov 2022 21:06:15 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.5.2 org.opencontainers.image.version=8.5.2 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-11-16T20:48:12+00:00 org.opencontainers.image.created=2022-11-16T20:48:12+00:00
# Wed, 16 Nov 2022 21:06:15 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:eaead16dc43bb8811d4ff450935d607f9ba4baffda4fc110cc402fa43f601d83`  
		Last Modified: Fri, 21 Oct 2022 03:03:39 GMT  
		Size: 28.6 MB (28577834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98504f7fd0eb05abf8fa2bfa2ee8ac982faadee3e4e12a2d79670ac8dc926083`  
		Last Modified: Tue, 22 Nov 2022 19:22:39 GMT  
		Size: 40.6 MB (40625797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319b43422ffa2df9a31413a38f2b9acdd59d8c76ea91fb804106cc97c6019f3c`  
		Last Modified: Tue, 22 Nov 2022 19:22:09 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e313819e4f3ba9a4ad2f1cd17ca1a9336075bd84cd8bfc3aeb693aad79f23e1`  
		Last Modified: Tue, 22 Nov 2022 19:23:53 GMT  
		Size: 342.2 MB (342205404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea288f002f50515aa781411d05ad81c43b95c349ccb3dd66b160f48d9a7eeb34`  
		Last Modified: Tue, 22 Nov 2022 19:22:07 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a02cc7fdbaee561a21e89d9f12c8544869caede67797fc196398d0dcd4d6367`  
		Last Modified: Tue, 22 Nov 2022 19:22:07 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20234b6e73958a4f8716d5cfa7631cbec7bd585df378dbb17a0a7567318f4e0`  
		Last Modified: Tue, 22 Nov 2022 19:22:06 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dfb93d097085478cad0dc833e46c5e95afdd6f7ec8a2ab5cb09f2af329e54d`  
		Last Modified: Tue, 22 Nov 2022 19:22:04 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e6513c65a39733bc36c96ed2bb19ed6869a9180d915142d83d2de553af6c9c`  
		Last Modified: Tue, 22 Nov 2022 19:22:04 GMT  
		Size: 2.7 KB (2718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2459fa2d6538cca5a84efd6a6ee5355c9fa1cadfb4718fec18a468c8c5d6b2e`  
		Last Modified: Tue, 22 Nov 2022 19:22:05 GMT  
		Size: 1.8 MB (1770001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d1047a86e86b9c4c1740432f83a6df7b0cef60cbc9d23a354f28b66d894a66`  
		Last Modified: Tue, 22 Nov 2022 19:22:01 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d1047a86e86b9c4c1740432f83a6df7b0cef60cbc9d23a354f28b66d894a66`  
		Last Modified: Tue, 22 Nov 2022 19:22:01 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:8.5.2` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:659c06161ec7e8d5aca405ce56e892bcfa3c36dc25d43607e0865969bfcc5f01
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **404.3 MB (404306213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e0efa28c8656645f29d8994093d497a8def6de88431d323ba47ce4aa9923460`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 21:05:16 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Wed, 16 Nov 2022 21:05:16 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Wed, 16 Nov 2022 21:05:32 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.5.2-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.5.2 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash
# Wed, 16 Nov 2022 21:05:36 GMT
WORKDIR /usr/share/logstash
# Wed, 16 Nov 2022 21:05:36 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 16 Nov 2022 21:05:36 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Nov 2022 21:05:36 GMT
COPY file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Wed, 16 Nov 2022 21:05:36 GMT
COPY file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Wed, 16 Nov 2022 21:05:36 GMT
COPY file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Wed, 16 Nov 2022 21:05:36 GMT
COPY file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Wed, 16 Nov 2022 21:05:37 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Wed, 16 Nov 2022 21:05:37 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 16 Nov 2022 21:05:37 GMT
COPY file:b957ce48a2de40474174c778ad47ed8a8bb37d58c020d91507d11d3bf2ad62dd in /usr/local/bin/ 
# Wed, 16 Nov 2022 21:05:37 GMT
COPY file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Wed, 16 Nov 2022 21:05:37 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Wed, 16 Nov 2022 21:05:37 GMT
USER 1000
# Wed, 16 Nov 2022 21:05:37 GMT
EXPOSE 5044 9600
# Wed, 16 Nov 2022 21:05:37 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.5.2 org.opencontainers.image.version=8.5.2 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-11-16T20:49:53+00:00 org.opencontainers.image.created=2022-11-16T20:49:53+00:00
# Wed, 16 Nov 2022 21:05:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86018fa370fd3d0bc15a005f860e7cfec910ef0ad473b9398d3fa7a68487bfc`  
		Last Modified: Tue, 29 Nov 2022 01:52:34 GMT  
		Size: 34.5 MB (34468899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a339aa1cd8729f9009149d701a2d9ee5b1c72fc5da04e3496b1063270cb363e3`  
		Last Modified: Tue, 29 Nov 2022 01:52:30 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df7531c9b42c06f52347477d1230e6dc37397e698089bea801997a5ac8ea050`  
		Last Modified: Tue, 29 Nov 2022 01:52:51 GMT  
		Size: 341.0 MB (340984239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4824cc93d9fc2907c4f55a8fd906b1a87e07afe0e56bec89e053fc2ab184f80`  
		Last Modified: Tue, 29 Nov 2022 01:52:30 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a05abbdf0de46664d5d903edbbce054fc68605a87a95975d71ae2a78e90c921`  
		Last Modified: Tue, 29 Nov 2022 01:52:30 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddf86798fcbbac19c99349f4dbe7a0f534211cea7733c0285814b72f6a68fe3`  
		Last Modified: Tue, 29 Nov 2022 01:52:28 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2664460b5fdbff813ee5016bbdbc24b0b84a40fbb163f1dba1f7ad662d17759`  
		Last Modified: Tue, 29 Nov 2022 01:52:28 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b437651fb63013bab0ff4d7b452776415c052f45510b4fcabdec3eb608b707`  
		Last Modified: Tue, 29 Nov 2022 01:52:28 GMT  
		Size: 2.7 KB (2719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355ee7f92f45745c3495304eee3ae205dd403bbc68900123a09df0e4081427bb`  
		Last Modified: Tue, 29 Nov 2022 01:52:28 GMT  
		Size: 1.7 MB (1650082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4041ba1d7ca422dbd0a1e6706f59d9ba668aee7823b594b78015c6f32a0aa7f`  
		Last Modified: Tue, 29 Nov 2022 01:52:28 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4041ba1d7ca422dbd0a1e6706f59d9ba668aee7823b594b78015c6f32a0aa7f`  
		Last Modified: Tue, 29 Nov 2022 01:52:28 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
