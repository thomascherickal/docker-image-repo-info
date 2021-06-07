<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:6.8.16`](#logstash6816)
-	[`logstash:7.13.1`](#logstash7131)

## `logstash:6.8.16`

```console
$ docker pull logstash@sha256:f992ff664b1302e91d0c1c35c3d035f67456b4975172fa8d90923fdf78350d33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `logstash:6.8.16` - linux; amd64

```console
$ docker pull logstash@sha256:d5053648560866a6be2985ffedfb3c974e6730f680545008cd3f38ad01d16e2a
```

-	Docker Version: 20.10.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.9 MB (383912907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe24d4d4121e2806cedba8cb76271b55b1bd051065ab0e2d1e01720261fe9125`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Fri, 21 May 2021 14:28:52 GMT
RUN yum update -y && yum install -y java-1.8.0-openjdk-devel-1.8.0.282.b08 java-1.8.0-openjdk-headless-1.8.0.282.b08 which &&     yum clean all
# Fri, 21 May 2021 14:28:55 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home-dir /usr/share/logstash --no-create-home       logstash
# Fri, 21 May 2021 14:29:11 GMT
RUN curl -Lo - http://localhost:8000/logstash-6.8.16.tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-6.8.16 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Fri, 21 May 2021 14:29:13 GMT
WORKDIR /usr/share/logstash
# Fri, 21 May 2021 14:29:13 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 21 May 2021 14:29:13 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 21 May 2021 14:29:13 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Fri, 21 May 2021 14:29:14 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Fri, 21 May 2021 14:29:14 GMT
ADD file:2ef21d4766eab3ac48ed3847c8b8d05554f1fd0b39061cba66c9ac93240087fa in config/ 
# Fri, 21 May 2021 14:29:14 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Fri, 21 May 2021 14:29:14 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Fri, 21 May 2021 14:29:15 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Fri, 21 May 2021 14:29:15 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Fri, 21 May 2021 14:29:15 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Fri, 21 May 2021 14:29:15 GMT
USER 1000
# Fri, 21 May 2021 14:29:16 GMT
ADD file:c92f9dee23c3c5a04a654972a270462e21648cf6cc8c61ea9ea9b75e6f2d6089 in /usr/local/bin/ 
# Fri, 21 May 2021 14:29:16 GMT
EXPOSE 5044 9600
# Fri, 21 May 2021 14:29:16 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=logstash org.label-schema.version=6.8.16 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash license=Elastic License
# Fri, 21 May 2021 14:29:16 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89a50411b67da19098f6f4c54d72e452c59bd145292305c5f3d3174b87c56f0`  
		Last Modified: Tue, 25 May 2021 11:28:28 GMT  
		Size: 129.2 MB (129213476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f0b73169ca8e4ae9902629bacce71642ed8073a46dee331838c386e07638ef`  
		Last Modified: Tue, 25 May 2021 11:28:07 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e77188e38a41ab11f4a1487c40b855b876088bfae784d3ba9303527ab1deb8`  
		Last Modified: Tue, 25 May 2021 11:28:22 GMT  
		Size: 177.6 MB (177590850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ffbc7b505ccbdae6b4d88eec8345f8050d7168ab2d2ab87ed150c603ae15bc`  
		Last Modified: Tue, 25 May 2021 11:28:04 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ee63215d64d8d8273c2179330c267e01b7e80cdf6f8bdc517adf660d67e605`  
		Last Modified: Tue, 25 May 2021 11:28:04 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01747ded2c5bf674a05557e9d4c9854846c823f38c4a5d35f710039e0166854`  
		Last Modified: Tue, 25 May 2021 11:28:04 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e819fb16a265cd5ec97efc6ccc5faac5269f81eba2e57568347d7b783972019d`  
		Last Modified: Tue, 25 May 2021 11:28:04 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9c6d91a0b8264f720a37c363d1f90cc6f7a9d26388ae555d22679f96bb64d5`  
		Last Modified: Tue, 25 May 2021 11:28:00 GMT  
		Size: 2.7 KB (2677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bb26ca9a614b57f309eb3bdfc6b940d436fc246e63644fd66adc29c881fc68`  
		Last Modified: Tue, 25 May 2021 11:28:01 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bb26ca9a614b57f309eb3bdfc6b940d436fc246e63644fd66adc29c881fc68`  
		Last Modified: Tue, 25 May 2021 11:28:01 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a516ef18f7496070e5946955d6e50a8d1ac425599881555be3578e3869b20b`  
		Last Modified: Tue, 25 May 2021 11:28:01 GMT  
		Size: 1.0 MB (1004513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:7.13.1`

```console
$ docker pull logstash@sha256:82869233a526c5fc7a13c75ca4455c7dba1e4f4eeed837aa147916e427f984e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:7.13.1` - linux; amd64

```console
$ docker pull logstash@sha256:a649b537959924556b64d6bb4b8a74530adfff5d4a8f7792936d40e7834341c8
```

-	Docker Version: 20.10.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.2 MB (488243812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea21030558664acb2ee300edf20f292aa4bf7d58204793eb33a675d65ebad206`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Fri, 28 May 2021 17:37:43 GMT
RUN for iter in {1..10}; do yum update -y &&     yum install -y procps findutils tar gzip which shadow-utils &&     yum clean all && yum clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     yum clean all && yum clean metadata && sleep 10; done;     (exit $exit_code)
# Fri, 28 May 2021 17:37:45 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home-dir /usr/share/logstash --no-create-home       logstash
# Fri, 28 May 2021 17:38:08 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.13.1-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.13.1 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Fri, 28 May 2021 17:38:11 GMT
WORKDIR /usr/share/logstash
# Fri, 28 May 2021 17:38:11 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 28 May 2021 17:38:11 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 May 2021 17:38:12 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Fri, 28 May 2021 17:38:12 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Fri, 28 May 2021 17:38:12 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Fri, 28 May 2021 17:38:12 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Fri, 28 May 2021 17:38:13 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Fri, 28 May 2021 17:38:13 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Fri, 28 May 2021 17:38:13 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Fri, 28 May 2021 17:38:13 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Fri, 28 May 2021 17:38:13 GMT
USER 1000
# Fri, 28 May 2021 17:38:14 GMT
ADD file:4fc35f1873d25f5258bad3492de23d09cc33fd409639a119015123b4adae1db5 in /usr/local/bin/ 
# Fri, 28 May 2021 17:38:14 GMT
EXPOSE 5044 9600
# Fri, 28 May 2021 17:38:14 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.13.1 org.opencontainers.image.version=7.13.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2021-05-28T16:32:23Z org.opencontainers.image.created=2021-05-28T16:32:23Z
# Fri, 28 May 2021 17:38:14 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a92d6a3d1218e57dd08dd7c87f52d966d889b5ca71d28b4db3f01f456932ca`  
		Last Modified: Thu, 03 Jun 2021 06:06:26 GMT  
		Size: 47.6 MB (47628487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68299aefaf1f44a0fd822373789defae2bd973d95c8f7ba2217b0f9960511e1a`  
		Last Modified: Thu, 03 Jun 2021 06:06:14 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a0b94e9ae23d11dd37cca35f862c9c322c72295dd921725d4127bc58cfad9a`  
		Last Modified: Thu, 03 Jun 2021 06:06:48 GMT  
		Size: 363.5 MB (363506520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdd0b780a4035ba59c8427bf0492c351ae641fc619656d6ba256557645f8248`  
		Last Modified: Thu, 03 Jun 2021 06:06:11 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3981f4824dbe426c200e07a85b6f892524036878dc33ee9950f019a65cc51ad`  
		Last Modified: Thu, 03 Jun 2021 06:06:11 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35052ccdc005e68a87d26142dcf0650ed63e0fefdcfdcee948138460b56a6ba`  
		Last Modified: Thu, 03 Jun 2021 06:06:10 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d136dab8dee6c945887e81ad61bce6b829d4afdebc438d0e4d43c0fc6b9720`  
		Last Modified: Thu, 03 Jun 2021 06:06:08 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7c070b51f20c194653800c861d8f6fd26d024fb44a043650d11c38cb5504f0`  
		Last Modified: Thu, 03 Jun 2021 06:06:07 GMT  
		Size: 2.8 KB (2761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1af7ae085e22379fcb578e41542e1c3050184bf9ddf4167df819d4402c7617`  
		Last Modified: Thu, 03 Jun 2021 06:06:07 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1af7ae085e22379fcb578e41542e1c3050184bf9ddf4167df819d4402c7617`  
		Last Modified: Thu, 03 Jun 2021 06:06:07 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb153906a5970cbeed3c6c768db7eafe22af1ca09ee14ef3d4abdc8db016724`  
		Last Modified: Thu, 03 Jun 2021 06:06:07 GMT  
		Size: 1.0 MB (1004615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:7.13.1` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:5b0870867e3fe9e89acd28c72b348dfe73dc2b9ad939f0c4673db4be12e87183
```

-	Docker Version: 20.10.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **523.3 MB (523307084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f865dc0edb36e367bb2f960ac87d162d3e2b6c6215739e2f4d18b79dae1919f4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Sat, 14 Nov 2020 00:40:26 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Sat, 14 Nov 2020 00:40:31 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:40:32 GMT
CMD ["/bin/bash"]
# Fri, 28 May 2021 16:47:37 GMT
RUN for iter in {1..10}; do yum install -y http://mirror.centos.org/centos/7/updates/x86_64/Packages/bind-license-9.11.4-26.P2.el7_9.5.noarch.rpm &&     yum clean all &&     yum clean metadata &&     exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     yum clean all &&     yum clean metadata && sleep 10; done;     (exit $exit_code)
# Fri, 28 May 2021 16:48:08 GMT
RUN for iter in {1..10}; do yum update -y &&     yum install -y procps findutils tar gzip which shadow-utils &&     yum clean all && yum clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     yum clean all && yum clean metadata && sleep 10; done;     (exit $exit_code)
# Fri, 28 May 2021 16:48:09 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home-dir /usr/share/logstash --no-create-home       logstash
# Fri, 28 May 2021 16:48:28 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.13.1-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.13.1 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Fri, 28 May 2021 16:48:30 GMT
WORKDIR /usr/share/logstash
# Fri, 28 May 2021 16:48:30 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 28 May 2021 16:48:30 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 May 2021 16:48:31 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Fri, 28 May 2021 16:48:31 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Fri, 28 May 2021 16:48:31 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Fri, 28 May 2021 16:48:31 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Fri, 28 May 2021 16:48:31 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Fri, 28 May 2021 16:48:31 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Fri, 28 May 2021 16:48:32 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Fri, 28 May 2021 16:48:32 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Fri, 28 May 2021 16:48:32 GMT
USER 1000
# Fri, 28 May 2021 16:48:32 GMT
ADD file:90dad4802ee0da80c7e83b3633edb3846df70b484fed5615c56683a9e4c1fad0 in /usr/local/bin/ 
# Fri, 28 May 2021 16:48:32 GMT
EXPOSE 5044 9600
# Fri, 28 May 2021 16:48:32 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.13.1 org.opencontainers.image.version=7.13.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2021-05-28T16:31:07+00:00 org.opencontainers.image.created=2021-05-28T16:31:07+00:00
# Fri, 28 May 2021 16:48:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a58f3e529a9c6c3c4e980b2798a844fb8ca86fd6e3bd9abe9483627161c3ac1`  
		Last Modified: Mon, 07 Jun 2021 17:42:28 GMT  
		Size: 6.3 MB (6297505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed64d77c6a043393b8d75689d01dc78fc76d667d280e19d4d715829fb94397d`  
		Last Modified: Mon, 07 Jun 2021 17:42:33 GMT  
		Size: 47.4 MB (47444736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c29fa6f5f6a2a55356dbf8df6dbe679e39cf982e4f196b24cdf454cbd60d8a`  
		Last Modified: Mon, 07 Jun 2021 17:42:24 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ea0441a0d837fc439be4ada74afb835f149f9f6852f39eb23fc0141ac8e00b`  
		Last Modified: Mon, 07 Jun 2021 17:42:59 GMT  
		Size: 360.2 MB (360238711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6328492dcf9989397371bf192e76f4773939d06c379835261017fb00e58568c`  
		Last Modified: Mon, 07 Jun 2021 17:42:24 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b511f55818e7ed61a6984331ea2f94089e4f9334867877dae38b1c562c6cfbc`  
		Last Modified: Mon, 07 Jun 2021 17:42:24 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f509fab2e787c7760abf8198c56f6cacb4ffd86cd7a09360abafe16a7b81cd1`  
		Last Modified: Mon, 07 Jun 2021 17:42:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de18963ad4d18a3fc5269260c6306f57160881e13c1cf3eea7b0a9f4b70e94a1`  
		Last Modified: Mon, 07 Jun 2021 17:42:22 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc084ae7d08f6abaf0aeb4304f663bb2cc52654c5b3a3f6577d9de8500e06604`  
		Last Modified: Mon, 07 Jun 2021 17:42:21 GMT  
		Size: 2.8 KB (2760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56f0e0c20fb3d6ed259bc487b33563c0c1e48f0347f8dbfcf4019d1df53d68e`  
		Last Modified: Mon, 07 Jun 2021 17:42:21 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56f0e0c20fb3d6ed259bc487b33563c0c1e48f0347f8dbfcf4019d1df53d68e`  
		Last Modified: Mon, 07 Jun 2021 17:42:21 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3edf5cddf9c0412ba0af3b4b89ea090590b468c035927e35916b071b07c031a4`  
		Last Modified: Mon, 07 Jun 2021 17:42:22 GMT  
		Size: 944.2 KB (944167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
