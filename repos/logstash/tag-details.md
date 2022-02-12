<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:6.8.23`](#logstash6823)
-	[`logstash:7.17.0`](#logstash7170)
-	[`logstash:8.0.0`](#logstash800)

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

## `logstash:7.17.0`

```console
$ docker pull logstash@sha256:4e3039e6348cd60615e91df128599a5ed374d39fe57cf87f1cfa0d2a9c4cda96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:7.17.0` - linux; amd64

```console
$ docker pull logstash@sha256:20082a1bb18db0712e24f5ac954fbba41a3e9573f4f8437686759f42e92cba9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **434.5 MB (434497430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fac3ccea018c8918d49194719cf2c95611810c4dec10ef5f8094cb7b47ad79a5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 28 Jan 2022 09:55:33 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y &&     apt-get upgrade -y &&     apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Fri, 28 Jan 2022 09:55:33 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home /usr/share/logstash --no-create-home       logstash
# Fri, 28 Jan 2022 09:56:00 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.0-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.0 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Fri, 28 Jan 2022 09:56:03 GMT
WORKDIR /usr/share/logstash
# Fri, 28 Jan 2022 09:56:03 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 28 Jan 2022 09:56:04 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jan 2022 09:56:04 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Fri, 28 Jan 2022 09:56:04 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Fri, 28 Jan 2022 09:56:04 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Fri, 28 Jan 2022 09:56:04 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Fri, 28 Jan 2022 09:56:05 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Fri, 28 Jan 2022 09:56:05 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Fri, 28 Jan 2022 09:56:05 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Fri, 28 Jan 2022 09:56:05 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Fri, 28 Jan 2022 09:56:06 GMT
USER 1000
# Fri, 28 Jan 2022 09:56:06 GMT
ADD file:bc2ff40ec3323fe4b7e3cc88ed3e05a6716f206361909a69b57058b5e140a579 in /usr/local/bin/ 
# Fri, 28 Jan 2022 09:56:06 GMT
EXPOSE 5044 9600
# Fri, 28 Jan 2022 09:56:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.0 org.opencontainers.image.version=7.17.0 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-01-28T08:37:12Z org.opencontainers.image.created=2022-01-28T08:37:12Z
# Fri, 28 Jan 2022 09:56:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075c549da632b7da73e0190705d55b133382067fd407df323e69680a67467711`  
		Last Modified: Wed, 02 Feb 2022 12:41:34 GMT  
		Size: 37.1 MB (37067935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59e0bbf7f36be204b00a941cbf9b9221854da9feb31abc10d14f4edc67c7ff`  
		Last Modified: Wed, 02 Feb 2022 12:41:29 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d41ef354cd1393456b04df2987dadf0aa103f64c95f99006c0f475924988c6`  
		Last Modified: Wed, 02 Feb 2022 12:43:57 GMT  
		Size: 367.2 MB (367192249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977337e2f7daceca1a011ee437ebee09ff151397daf5bc0f7c2db31af5abcbb1`  
		Last Modified: Wed, 02 Feb 2022 12:43:27 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d27a2d56953d95670e4bc2ade52094a1005a1ac7c93ba91657851c43a9936d3`  
		Last Modified: Wed, 02 Feb 2022 12:43:25 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f6021ac5633c688885fe95fc7afdfd705a4963cb97d8fe0930fee0d908e839`  
		Last Modified: Wed, 02 Feb 2022 12:43:25 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58474c5058e7bf23a587113b26495daa54edb0525d483db9f1033ecb7ee2894`  
		Last Modified: Wed, 02 Feb 2022 12:43:24 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b7873aa4630b47bcc99e9e81432d4dfc555c2715d4a02ceae9fe6a36044d17`  
		Last Modified: Wed, 02 Feb 2022 12:43:21 GMT  
		Size: 2.8 KB (2806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbb752857ba899850bb105acdfb04b352c1f7db6ecddbdafb1d421ffba1dac1`  
		Last Modified: Wed, 02 Feb 2022 12:43:21 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbb752857ba899850bb105acdfb04b352c1f7db6ecddbdafb1d421ffba1dac1`  
		Last Modified: Wed, 02 Feb 2022 12:43:21 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fb742a21576cd6415ac835c22359bc99446d601c54102352c7afef9379a1bc`  
		Last Modified: Wed, 02 Feb 2022 12:43:22 GMT  
		Size: 1.7 MB (1663759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:7.17.0` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:a362c77b64780ed72f0c34f489d8f0dd27036b98f10bc5eadc5609e54b0f95a1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **425.8 MB (425821308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d506a7a22d353dac84804966f076c1d6575ee8bf74b3eb9de3a4d62bc95907`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Fri, 07 Jan 2022 01:53:45 GMT
ADD file:521a8ada4ac06e6f7720904486d481d216a8c3e08c0c7db1376c39a33e709668 in / 
# Fri, 07 Jan 2022 01:53:45 GMT
CMD ["bash"]
# Fri, 28 Jan 2022 09:00:55 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y &&     apt-get upgrade -y &&     apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Fri, 28 Jan 2022 09:00:55 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home /usr/share/logstash --no-create-home       logstash
# Fri, 28 Jan 2022 09:01:14 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.0-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.0 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Fri, 28 Jan 2022 09:01:17 GMT
WORKDIR /usr/share/logstash
# Fri, 28 Jan 2022 09:01:17 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 28 Jan 2022 09:01:17 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 Jan 2022 09:01:17 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Fri, 28 Jan 2022 09:01:17 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Fri, 28 Jan 2022 09:01:17 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Fri, 28 Jan 2022 09:01:17 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Fri, 28 Jan 2022 09:01:18 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Fri, 28 Jan 2022 09:01:18 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Fri, 28 Jan 2022 09:01:18 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Fri, 28 Jan 2022 09:01:18 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Fri, 28 Jan 2022 09:01:18 GMT
USER 1000
# Fri, 28 Jan 2022 09:01:18 GMT
ADD file:86be8b3554008b0941aee895258eda0ddb8a6aa71aaa83d0b5f7ef3c5ef5697e in /usr/local/bin/ 
# Fri, 28 Jan 2022 09:01:18 GMT
EXPOSE 5044 9600
# Fri, 28 Jan 2022 09:01:19 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.0 org.opencontainers.image.version=7.17.0 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-01-28T08:37:56+00:00 org.opencontainers.image.created=2022-01-28T08:37:56+00:00
# Fri, 28 Jan 2022 09:01:19 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:5f3d23ccb99f6c9462a15efcf35aef0863858073a06d56df671d0e791b26222a`  
		Last Modified: Fri, 07 Jan 2022 01:55:32 GMT  
		Size: 27.2 MB (27171074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c11b3eae2e79ee33db622e0553c37f653f6149213649d5c5f6d8672c60ef1d`  
		Last Modified: Fri, 04 Feb 2022 03:18:54 GMT  
		Size: 33.2 MB (33206727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5be9c5f792a7246301e0430112c42f9b990fce855b244e79a657788f92bbe8`  
		Last Modified: Fri, 04 Feb 2022 03:18:49 GMT  
		Size: 1.8 KB (1832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ce9f0846c22719fb379d3144b133a9508b8699f80ebd4ef85fb3d6091c98da`  
		Last Modified: Fri, 04 Feb 2022 03:19:27 GMT  
		Size: 363.9 MB (363906306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8667ce401c896a0e7f73ffa55a177359ebdeba89e7eb55d9d2bc396331a66f93`  
		Last Modified: Fri, 04 Feb 2022 03:18:48 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fd31165c3a0cf400fc809744d236dce9c5235ffd0fb5b752e331bc5fd09de9`  
		Last Modified: Fri, 04 Feb 2022 03:18:48 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90348e5a7d1632cfc2060e26077ba076daf0f74f18238732285e269a452963d8`  
		Last Modified: Fri, 04 Feb 2022 03:18:45 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a919d5add02708f42499a5bb27129979a563aca18a2630ef8b2842dd028309`  
		Last Modified: Fri, 04 Feb 2022 03:18:46 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f131f0c74010548c068a0a7e678b0ad6625484d46af1cd6f086bfe0912617748`  
		Last Modified: Fri, 04 Feb 2022 03:18:46 GMT  
		Size: 2.8 KB (2812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f77155811ef61c6eee5003eca8ff85a94da18d430f2c9219f587362ac1713a`  
		Last Modified: Fri, 04 Feb 2022 03:18:46 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f77155811ef61c6eee5003eca8ff85a94da18d430f2c9219f587362ac1713a`  
		Last Modified: Fri, 04 Feb 2022 03:18:46 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f66045354814b81cca7d97798771d2095ebbda59ba36e78a215a09f2818bf65`  
		Last Modified: Fri, 04 Feb 2022 03:18:46 GMT  
		Size: 1.5 MB (1530118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:8.0.0`

```console
$ docker pull logstash@sha256:13d1fa8923144654e6df2cbf28bd411e1e23204a01cf17f343efcdf544ca1d19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:8.0.0` - linux; amd64

```console
$ docker pull logstash@sha256:7170c4822e75207226d3467a5561a12127e89b1fca303947c8740b6f044d7d9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **434.1 MB (434092633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb046ce064219eea4b85b3bc5102d66cca898aacb70066051d5c716ebc0c946`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Thu, 03 Feb 2022 18:05:57 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y &&     apt-get upgrade -y &&     apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Thu, 03 Feb 2022 18:05:57 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home /usr/share/logstash --no-create-home       logstash
# Thu, 03 Feb 2022 18:06:22 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.0.0-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.0.0 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Thu, 03 Feb 2022 18:06:25 GMT
WORKDIR /usr/share/logstash
# Thu, 03 Feb 2022 18:06:25 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 03 Feb 2022 18:06:25 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Feb 2022 18:06:25 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Thu, 03 Feb 2022 18:06:25 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Thu, 03 Feb 2022 18:06:26 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Thu, 03 Feb 2022 18:06:26 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Thu, 03 Feb 2022 18:06:26 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Thu, 03 Feb 2022 18:06:26 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Thu, 03 Feb 2022 18:06:26 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Thu, 03 Feb 2022 18:06:27 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Thu, 03 Feb 2022 18:06:27 GMT
USER 1000
# Thu, 03 Feb 2022 18:06:27 GMT
ADD file:74f1240397564c8006436b57526b98f8b3e9fcbad9cb9f7c905c223de143c5f3 in /usr/local/bin/ 
# Thu, 03 Feb 2022 18:06:27 GMT
EXPOSE 5044 9600
# Thu, 03 Feb 2022 18:06:27 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.0.0 org.opencontainers.image.version=8.0.0 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-02-03T16:51:05Z org.opencontainers.image.created=2022-02-03T16:51:05Z
# Thu, 03 Feb 2022 18:06:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89192cd6dc46dfa5e3baaf748aabc9f43282ac46f920b2dd95d47a2b76c995e`  
		Last Modified: Fri, 11 Feb 2022 00:15:35 GMT  
		Size: 36.8 MB (36843712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf16a3abe1261320de2c5d677ecf11e7c8dd4cf9ca6100411fb5bf04369c3c`  
		Last Modified: Fri, 11 Feb 2022 00:15:02 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb005e70c28160c2fbf33e8727299395a4de6217703bb6771a6760814582e8b7`  
		Last Modified: Fri, 11 Feb 2022 00:18:19 GMT  
		Size: 367.0 MB (367013910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1efd72bfe67ed70785fa137213504f39447d75a283c00bb952c70bab629835c`  
		Last Modified: Fri, 11 Feb 2022 00:14:56 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7873da3bdf3a5e6a675b2fdfedc87c5db3ca4036b3de65930ed61a838bcc41`  
		Last Modified: Fri, 11 Feb 2022 00:14:55 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ca7410bb79781638b432c4da579e7744eb55bd96ec4c8377187670423eff87`  
		Last Modified: Fri, 11 Feb 2022 00:14:55 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e90eee317e57284a3da07324259e36d1d505d459650c3e2cc75ddc6937e0e6a`  
		Last Modified: Fri, 11 Feb 2022 00:14:49 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70aa82f7e6d05409cd5ae2efb5bff768c9a7ac0d8303ef345d20840b636fcb`  
		Last Modified: Fri, 11 Feb 2022 00:14:49 GMT  
		Size: 2.8 KB (2827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce9d80315a30366eb1f804dd6f945d04445e4647ceaa99b42dfce838d835310`  
		Last Modified: Fri, 11 Feb 2022 00:14:50 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce9d80315a30366eb1f804dd6f945d04445e4647ceaa99b42dfce838d835310`  
		Last Modified: Fri, 11 Feb 2022 00:14:50 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fa1fb4cf952e4e317c996a89ea1a510358ef3160fb8c0b6098b67ff38ba378`  
		Last Modified: Fri, 11 Feb 2022 00:14:51 GMT  
		Size: 1.7 MB (1663828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:8.0.0` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:23f38d823286577930d3c294515c8ef9456451f44921ba3dcc64c4417520ffb0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **425.3 MB (425272317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9822332de5aab6bceef04b124a9899a0296c512860177232807fe6f446b13006`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Thu, 03 Feb 2022 17:14:47 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y &&     apt-get upgrade -y &&     apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Thu, 03 Feb 2022 17:14:47 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home /usr/share/logstash --no-create-home       logstash
# Thu, 03 Feb 2022 17:15:05 GMT
RUN curl -Lo - http://localhost:8000/logstash-8.0.0-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-8.0.0 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Thu, 03 Feb 2022 17:15:07 GMT
WORKDIR /usr/share/logstash
# Thu, 03 Feb 2022 17:15:07 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 03 Feb 2022 17:15:08 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Feb 2022 17:15:08 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Thu, 03 Feb 2022 17:15:08 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Thu, 03 Feb 2022 17:15:08 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Thu, 03 Feb 2022 17:15:08 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Thu, 03 Feb 2022 17:15:08 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Thu, 03 Feb 2022 17:15:08 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Thu, 03 Feb 2022 17:15:09 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Thu, 03 Feb 2022 17:15:09 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Thu, 03 Feb 2022 17:15:09 GMT
USER 1000
# Thu, 03 Feb 2022 17:15:09 GMT
ADD file:945c6fce9a9e80bbe91b66f2c2535aba760ab72a0b46cff684339f8e5b553444 in /usr/local/bin/ 
# Thu, 03 Feb 2022 17:15:09 GMT
EXPOSE 5044 9600
# Thu, 03 Feb 2022 17:15:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=8.0.0 org.opencontainers.image.version=8.0.0 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-02-03T16:52:28+00:00 org.opencontainers.image.created=2022-02-03T16:52:28+00:00
# Thu, 03 Feb 2022 17:15:09 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0386bb2c4903aa22240b69f9a43243ec7cae2014384348a8a39eeac74acdd6`  
		Last Modified: Sat, 12 Feb 2022 00:05:12 GMT  
		Size: 32.9 MB (32854931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a51d3f0beb2478934a6bbf71d4d75b5289b7441b75ddbd715e5e0922d6c0f2`  
		Last Modified: Sat, 12 Feb 2022 00:05:08 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4737899eea50f8fd557f017295eea1e5229e5ddc4d3fbd4108440eb732b64dc3`  
		Last Modified: Sat, 12 Feb 2022 00:05:41 GMT  
		Size: 363.7 MB (363710587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be30f6d94e7c3ae437e6bb4ca6f875fb0bb7fa9967befea85ef4e452cf0300a3`  
		Last Modified: Sat, 12 Feb 2022 00:05:07 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bddd32a55ab472d7767b4261645932941322f8cce093ed533f3f695149c63f`  
		Last Modified: Sat, 12 Feb 2022 00:05:07 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7aa59ec9e42422d51a8591a5db2e68fd3851b14dab57f4dc73627c6859e1cd`  
		Last Modified: Sat, 12 Feb 2022 00:05:05 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f851cd52040ec2ee26bff07d98c5f534e6ce38038a818bdb9a4644a28941952`  
		Last Modified: Sat, 12 Feb 2022 00:05:05 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838059ef765b40a64e4a2488b9748ad3b8a74a2490d57fb5db7b85b7249e4110`  
		Last Modified: Sat, 12 Feb 2022 00:05:05 GMT  
		Size: 2.8 KB (2826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cfeb45ede00f9a4e89263821168c66489168d2cc921d80802e75bf497a9092`  
		Last Modified: Sat, 12 Feb 2022 00:05:05 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cfeb45ede00f9a4e89263821168c66489168d2cc921d80802e75bf497a9092`  
		Last Modified: Sat, 12 Feb 2022 00:05:05 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8364d5c85debb87a2c7ace291d3bf0ec6bbe73ffbec7f521cb8517a01129b7`  
		Last Modified: Sat, 12 Feb 2022 00:05:05 GMT  
		Size: 1.5 MB (1530080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
