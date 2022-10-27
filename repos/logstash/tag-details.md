<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:6.8.23`](#logstash6823)
-	[`logstash:7.17.7`](#logstash7177)
-	[`logstash:8.4.3`](#logstash843)

## `logstash:6.8.23`

```console
$ docker pull logstash@sha256:53d822de31e74c91dcb623abf0d0bfd95192ee571e695e39ea4fe2af626c9232
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `logstash:6.8.23` - linux; amd64

```console
$ docker pull logstash@sha256:347be947d25fad34bcb808af6884c9f7c06a3d9a1f9599d036bb4d05bd2a46a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.6 MB (395596751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e03e2750214e21b7f3a5a7b5cf55db2adb0aad5eb897eb03e77e05b2e6a1ebb`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:23 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Wed, 15 Sep 2021 18:20:23 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Wed, 15 Sep 2021 18:20:23 GMT
CMD ["/bin/bash"]
# Thu, 06 Jan 2022 20:50:28 GMT
RUN yum update -y && yum install -y java-1.8.0-openjdk-devel-1.8.0.282.b08 java-1.8.0-openjdk-headless-1.8.0.282.b08 which &&     yum clean all
# Thu, 06 Jan 2022 20:50:30 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home-dir /usr/share/logstash --no-create-home       logstash
# Thu, 06 Jan 2022 20:50:46 GMT
RUN curl -Lo - http://localhost:8000/logstash-6.8.23.tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-6.8.23 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Thu, 06 Jan 2022 20:50:48 GMT
WORKDIR /usr/share/logstash
# Thu, 06 Jan 2022 20:50:48 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 06 Jan 2022 20:50:48 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 20:50:49 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Thu, 06 Jan 2022 20:50:49 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Thu, 06 Jan 2022 20:50:49 GMT
ADD file:2ef21d4766eab3ac48ed3847c8b8d05554f1fd0b39061cba66c9ac93240087fa in config/ 
# Thu, 06 Jan 2022 20:50:49 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Thu, 06 Jan 2022 20:50:49 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Thu, 06 Jan 2022 20:50:50 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Thu, 06 Jan 2022 20:50:50 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Thu, 06 Jan 2022 20:50:50 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Thu, 06 Jan 2022 20:50:50 GMT
USER 1000
# Thu, 06 Jan 2022 20:50:50 GMT
ADD file:c571f1340b3840928052ac69357eca598068bd1a752b377b661e4a526205c25b in /usr/local/bin/ 
# Thu, 06 Jan 2022 20:50:51 GMT
EXPOSE 5044 9600
# Thu, 06 Jan 2022 20:50:51 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=logstash org.label-schema.version=6.8.23 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash license=Elastic License
# Thu, 06 Jan 2022 20:50:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b1fb6f60b9250e42308ecf6503a441f9fc10b2e603a46e8767f9646555f43d`  
		Last Modified: Thu, 13 Jan 2022 16:12:17 GMT  
		Size: 139.1 MB (139127934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab13d3e354e35c347031eddca0d4bb20209d98ace9d3223a8358de9120fc72b`  
		Last Modified: Thu, 13 Jan 2022 16:11:56 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5ffc479f94b8a50d1647f4dfce26f0045e4fcb2055db4859ddcc840208bb96`  
		Last Modified: Thu, 13 Jan 2022 16:12:10 GMT  
		Size: 178.7 MB (178701203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88d374d1955f1098a61ca9fee227fce373072d7b9379399153efe94b7a0774f`  
		Last Modified: Thu, 13 Jan 2022 16:11:53 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07700abd6d6ac998267b237b6308c2722005f4b43601aadf6fe67b2ff92a4d3`  
		Last Modified: Thu, 13 Jan 2022 16:11:53 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a109f862359a4f53f5f8b0c2c48138454070d95f9b003bd4332b725f466223`  
		Last Modified: Thu, 13 Jan 2022 16:11:53 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8800e09be38effb116e9b61cbfe8810b2c48c0a08af461cbfd3e58d52bf84f`  
		Last Modified: Thu, 13 Jan 2022 16:11:50 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2282ae509684254b6426aa0880f79c8147ebf07313803f64519567c602654a`  
		Last Modified: Thu, 13 Jan 2022 16:11:50 GMT  
		Size: 2.7 KB (2676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b4125dcde9ccc2725f69e8f367f96efe05fc158888dad1fb7d3502c268f7e0`  
		Last Modified: Thu, 13 Jan 2022 16:11:50 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b4125dcde9ccc2725f69e8f367f96efe05fc158888dad1fb7d3502c268f7e0`  
		Last Modified: Thu, 13 Jan 2022 16:11:50 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963fece8ba60aee91b52cdf69bf5b3548119d5efb180f0c3ccb045831ac1cd18`  
		Last Modified: Thu, 13 Jan 2022 16:11:49 GMT  
		Size: 1.7 MB (1663550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

## `logstash:8.4.3`

```console
$ docker pull logstash@sha256:94e9281c18f8230dd04d0bc30d98ce72fb53158bc2b2160beb11f900ca8b3ac3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:8.4.3` - linux; amd64

```console
$ docker pull logstash@sha256:edf9ca5e84bafb12398b8a8c9c227ffef7071580c83ad9ebfafa0e1af97409c8
```

-	Docker Version: 20.10.16
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **403.7 MB (403714313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfb18e1ac1feceba033d6d348762777325124e186a3d8dbf98cbea8706d1188d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 08:11:53 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Tue, 04 Oct 2022 08:11:53 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Tue, 04 Oct 2022 08:12:16 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.4.3-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.4.3 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash
# Tue, 04 Oct 2022 08:12:19 GMT
WORKDIR /usr/share/logstash
# Tue, 04 Oct 2022 08:12:19 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 04 Oct 2022 08:12:20 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 08:12:20 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Tue, 04 Oct 2022 08:12:20 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Tue, 04 Oct 2022 08:12:20 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Tue, 04 Oct 2022 08:12:20 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Tue, 04 Oct 2022 08:12:21 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Tue, 04 Oct 2022 08:12:21 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 04 Oct 2022 08:12:21 GMT
ADD file:01c94f52658ce0028c9fbb01770029c361ab602f72abca08df74221ee0678ad3 in /usr/local/bin/ 
# Tue, 04 Oct 2022 08:12:21 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Tue, 04 Oct 2022 08:12:22 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Tue, 04 Oct 2022 08:12:22 GMT
USER 1000
# Tue, 04 Oct 2022 08:12:22 GMT
EXPOSE 5044 9600
# Tue, 04 Oct 2022 08:12:22 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.4.3 org.opencontainers.image.version=8.4.3 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-10-04T07:19:07Z org.opencontainers.image.created=2022-10-04T07:19:07Z
# Tue, 04 Oct 2022 08:12:22 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3875ad3bad32654bfc757d51382541f8ec81c4892942a7090780bd41b86145`  
		Last Modified: Thu, 06 Oct 2022 09:24:22 GMT  
		Size: 40.6 MB (40576400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f579b2ccb023a49f93d91b403bb20b5d65b574b6f2b67753d811478c9a3a3ce5`  
		Last Modified: Thu, 06 Oct 2022 09:24:18 GMT  
		Size: 1.8 KB (1829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a3439dd6123f874b8075daab9733e01ba5c7405ec79a11fd78e5beeb4fa5f9`  
		Last Modified: Thu, 06 Oct 2022 09:24:44 GMT  
		Size: 332.8 MB (332791205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6442cb8d4f7dd6d9f86b9cc5e0fb574fe8b6742b8d3b07de48e474ddbd10a`  
		Last Modified: Thu, 06 Oct 2022 09:24:17 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee883133caf5af21e86cc265ad563b15e657d25c43fad72f0b9529d20149068`  
		Last Modified: Thu, 06 Oct 2022 09:24:17 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e72ba837a5e910a6fe06ad48f27448091ef89870b53e7124807be442a52cb64`  
		Last Modified: Thu, 06 Oct 2022 09:24:15 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c7257dcd3b5ec9ff2253f1770029f897232287ce169df77861a7263b6afd84`  
		Last Modified: Thu, 06 Oct 2022 09:24:15 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f69b7a6264c3eafbe76a3699f85a65b21ac19131aecab3ccc74cacfe36d600f`  
		Last Modified: Thu, 06 Oct 2022 09:24:15 GMT  
		Size: 2.7 KB (2720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa09d2a907d8ab2694e3af6d9f717114fffd9ef4e8288186a2644ccf4e8d5b3c`  
		Last Modified: Thu, 06 Oct 2022 09:24:15 GMT  
		Size: 1.8 MB (1767034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c44ce50d5e2516c02a1c28c7d7f6a5db38813cedce09edbf1402146f78dfeef`  
		Last Modified: Thu, 06 Oct 2022 09:24:15 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c44ce50d5e2516c02a1c28c7d7f6a5db38813cedce09edbf1402146f78dfeef`  
		Last Modified: Thu, 06 Oct 2022 09:24:15 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:8.4.3` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:744ad315ab172c283fde6b485641a20500a2035777d1e6678323146fd7f8c08d
```

-	Docker Version: 20.10.18
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.2 MB (395173515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0087f0f4e9a83109ed1b34b40936b348fc8636bad679bef9c41d4f3766c97189`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 07:37:11 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Tue, 04 Oct 2022 07:37:11 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Tue, 04 Oct 2022 07:37:30 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.4.3-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.4.3 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt && find /usr/share/logstash -type d -exec chmod g+s {} \; && ln -s /usr/share/logstash /opt/logstash
# Tue, 04 Oct 2022 07:37:31 GMT
WORKDIR /usr/share/logstash
# Tue, 04 Oct 2022 07:37:31 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 04 Oct 2022 07:37:32 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Oct 2022 07:37:32 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Tue, 04 Oct 2022 07:37:32 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Tue, 04 Oct 2022 07:37:32 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Tue, 04 Oct 2022 07:37:32 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Tue, 04 Oct 2022 07:37:32 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Tue, 04 Oct 2022 07:37:32 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 04 Oct 2022 07:37:33 GMT
ADD file:b0dec48ba1ae4318d7e3271ab894ca4d0d2e283a0c681a4b6b18119bff9e4690 in /usr/local/bin/ 
# Tue, 04 Oct 2022 07:37:33 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Tue, 04 Oct 2022 07:37:33 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Tue, 04 Oct 2022 07:37:33 GMT
USER 1000
# Tue, 04 Oct 2022 07:37:33 GMT
EXPOSE 5044 9600
# Tue, 04 Oct 2022 07:37:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.4.3 org.opencontainers.image.version=8.4.3 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-10-04T07:21:37+00:00 org.opencontainers.image.created=2022-10-04T07:21:37+00:00
# Tue, 04 Oct 2022 07:37:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb56756dd54303cc9eafa8837d87a7f2555d397cc5782c36994c0181af9eb98a`  
		Last Modified: Thu, 06 Oct 2022 07:51:33 GMT  
		Size: 34.8 MB (34772107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751df7e19a4688fbc66bd42a591bdd88c0f3e9b0a6a53f4ae0e7c354d5a786bc`  
		Last Modified: Thu, 06 Oct 2022 07:51:28 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8e11a320e1da14b187b0ec5dad63e375fc7c6ace8b711b0a146c37783f2371`  
		Last Modified: Thu, 06 Oct 2022 07:51:59 GMT  
		Size: 331.6 MB (331556285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90427094e6ece807bc60a0317d49152457e09a4b39c512f4c875ab71b0e0182c`  
		Last Modified: Thu, 06 Oct 2022 07:51:28 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de408133093d12152eedeef79f0b8b65dce1ea876379800ea08fb1e16fde176a`  
		Last Modified: Thu, 06 Oct 2022 07:51:28 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2874650b792db600aee2d1da612c256cd63b7613eac489ad533715cb7171e22`  
		Last Modified: Thu, 06 Oct 2022 07:51:26 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0025a9328338cbc82e86fc2234034316039fa612b3d5137c328d78260f5cb414`  
		Last Modified: Thu, 06 Oct 2022 07:51:26 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9005a1462d9873a9b860f47cd3ef40bbde3c2d21ee5f4f614c7c73637e915a02`  
		Last Modified: Thu, 06 Oct 2022 07:51:26 GMT  
		Size: 2.7 KB (2715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0b8018740b4662420539e916c878ba60d6e886621aa4c6826b9f8865450616`  
		Last Modified: Thu, 06 Oct 2022 07:51:26 GMT  
		Size: 1.6 MB (1646325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a9eb0f86312e2942efaf0fc608b0082d4fb7b94ecc921a242aaaf48a9c9156`  
		Last Modified: Thu, 06 Oct 2022 07:51:26 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a9eb0f86312e2942efaf0fc608b0082d4fb7b94ecc921a242aaaf48a9c9156`  
		Last Modified: Thu, 06 Oct 2022 07:51:26 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
