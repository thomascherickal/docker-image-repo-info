<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:6.8.18`](#logstash6818)
-	[`logstash:7.14.1`](#logstash7141)

## `logstash:6.8.18`

```console
$ docker pull logstash@sha256:c1f3fcc89c423ad03cd1f30dfd6669ccadfd092620e1e78b64f740fd47169f27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `logstash:6.8.18` - linux; amd64

```console
$ docker pull logstash@sha256:d1e2b38d9b12af689746df6e039b5a6d8a2b25eae8d707685a27cbaf923772a3
```

-	Docker Version: 20.10.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386141748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:903c4d35cb734be579656024b61bffc2950e134085ca13673e8849fb663e3033`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Wed, 28 Jul 2021 15:27:49 GMT
RUN yum update -y && yum install -y java-1.8.0-openjdk-devel-1.8.0.282.b08 java-1.8.0-openjdk-headless-1.8.0.282.b08 which &&     yum clean all
# Wed, 28 Jul 2021 15:27:51 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home-dir /usr/share/logstash --no-create-home       logstash
# Wed, 28 Jul 2021 15:28:07 GMT
RUN curl -Lo - http://localhost:8000/logstash-6.8.18.tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-6.8.18 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Wed, 28 Jul 2021 15:28:09 GMT
WORKDIR /usr/share/logstash
# Wed, 28 Jul 2021 15:28:09 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 28 Jul 2021 15:28:09 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 28 Jul 2021 15:28:09 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Wed, 28 Jul 2021 15:28:09 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Wed, 28 Jul 2021 15:28:10 GMT
ADD file:2ef21d4766eab3ac48ed3847c8b8d05554f1fd0b39061cba66c9ac93240087fa in config/ 
# Wed, 28 Jul 2021 15:28:10 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Wed, 28 Jul 2021 15:28:10 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Wed, 28 Jul 2021 15:28:10 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 28 Jul 2021 15:28:10 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Wed, 28 Jul 2021 15:28:11 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Wed, 28 Jul 2021 15:28:11 GMT
USER 1000
# Wed, 28 Jul 2021 15:28:11 GMT
ADD file:c92f9dee23c3c5a04a654972a270462e21648cf6cc8c61ea9ea9b75e6f2d6089 in /usr/local/bin/ 
# Wed, 28 Jul 2021 15:28:11 GMT
EXPOSE 5044 9600
# Wed, 28 Jul 2021 15:28:11 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=logstash org.label-schema.version=6.8.18 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash license=Elastic License
# Wed, 28 Jul 2021 15:28:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a712672ba481cfb7ab18d07ef709ef5115ed5dde27548f0645bb361e8c674b`  
		Last Modified: Tue, 03 Aug 2021 13:38:01 GMT  
		Size: 129.2 MB (129218305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a877f3eea5f7079bf857647ef28fe4a73145300913801e95dd1cdb6f85aef574`  
		Last Modified: Tue, 03 Aug 2021 13:37:40 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69acfd22513ab38aa165b3e464a2dadb27043891f267c52661fdad1f387d1c5`  
		Last Modified: Tue, 03 Aug 2021 13:37:57 GMT  
		Size: 179.8 MB (179814865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8d04ec36f51e581c597a767cee9e65c563b71fe39708c33ba521fac3faf887`  
		Last Modified: Tue, 03 Aug 2021 13:37:38 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9685380a916ef7d9344155fa2b74063c3ad7143e084f8dbb16166e6a7ef9b7f1`  
		Last Modified: Tue, 03 Aug 2021 13:37:37 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f566e6d13fc62b6e008070b77860c618b22c2af57ffd3997da1ef2a979286a`  
		Last Modified: Tue, 03 Aug 2021 13:37:37 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0c29e020be0103014d0d1fba510f5e634537f38344caa3aa3d6db46d727059`  
		Last Modified: Tue, 03 Aug 2021 13:37:36 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2574e0d2b979722956660590f06d46f14f31b7ad5e7c472e11b9c42748d42b96`  
		Last Modified: Tue, 03 Aug 2021 13:37:34 GMT  
		Size: 2.7 KB (2675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd5d62959bce18d174b23a82d7d0f01c16fc1c2eee4422ef73b5d4c9351a4cf`  
		Last Modified: Tue, 03 Aug 2021 13:37:34 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd5d62959bce18d174b23a82d7d0f01c16fc1c2eee4422ef73b5d4c9351a4cf`  
		Last Modified: Tue, 03 Aug 2021 13:37:34 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e655604c712b64b3c2618fd35870fae225bbb48e30fa54c9bf3ff5ce586cd070`  
		Last Modified: Tue, 03 Aug 2021 13:37:33 GMT  
		Size: 1.0 MB (1004509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:7.14.1`

```console
$ docker pull logstash@sha256:8880f89e084919bfe8007147d055b9edbaebb80cdddfa062b62a8d6de0f7a6c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `logstash:7.14.1` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:b1f3308db8149e891a0dee29a2608bdcb9f45a4bd3b6ff7bf5b4ee0c0b2c2222
```

-	Docker Version: 20.10.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **792.2 MB (792184391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b99809677148e02e2e6d059dd4c70bde0755f4235e2836e3c70b75aaa7f9b047`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Sat, 14 Nov 2020 00:40:26 GMT
ADD file:5b1e63a3cb041177b802b501dedcd71a86f1773ea0f69f048f2eb3901097711d in / 
# Sat, 14 Nov 2020 00:40:31 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:40:32 GMT
CMD ["/bin/bash"]
# Thu, 26 Aug 2021 08:17:23 GMT
RUN for iter in {1..10}; do yum install -y http://mirror.centos.org/centos/7/updates/x86_64/Packages/bind-license-9.11.4-26.P2.el7_9.5.noarch.rpm &&     yum clean all &&     yum clean metadata &&     exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     yum clean all &&     yum clean metadata && sleep 10; done;     (exit $exit_code)
# Thu, 26 Aug 2021 08:18:44 GMT
RUN for iter in {1..10}; do yum update -y &&     yum install -y procps findutils tar gzip which shadow-utils &&     yum clean all && yum clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     yum clean all && yum clean metadata && sleep 10; done;     (exit $exit_code)
# Thu, 26 Aug 2021 08:18:47 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home-dir /usr/share/logstash --no-create-home       logstash
# Thu, 26 Aug 2021 08:19:09 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.14.1-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.14.1 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Thu, 26 Aug 2021 08:19:10 GMT
WORKDIR /usr/share/logstash
# Thu, 26 Aug 2021 08:19:10 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 26 Aug 2021 08:19:10 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 26 Aug 2021 08:19:10 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Thu, 26 Aug 2021 08:19:11 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Thu, 26 Aug 2021 08:19:11 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Thu, 26 Aug 2021 08:19:11 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Thu, 26 Aug 2021 08:19:11 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Thu, 26 Aug 2021 08:19:11 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Thu, 26 Aug 2021 08:19:11 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Thu, 26 Aug 2021 08:19:12 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Thu, 26 Aug 2021 08:19:12 GMT
USER 1000
# Thu, 26 Aug 2021 08:19:12 GMT
ADD file:90dad4802ee0da80c7e83b3633edb3846df70b484fed5615c56683a9e4c1fad0 in /usr/local/bin/ 
# Thu, 26 Aug 2021 08:19:12 GMT
EXPOSE 5044 9600
# Thu, 26 Aug 2021 08:19:12 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.14.1 org.opencontainers.image.version=7.14.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2021-08-26T07:58:56+00:00 org.opencontainers.image.created=2021-08-26T07:58:56+00:00
# Thu, 26 Aug 2021 08:19:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:6717b8ec66cd6add0272c6391165585613c31314a43ff77d9751b53010e531ec`  
		Last Modified: Sat, 14 Nov 2020 00:41:36 GMT  
		Size: 108.4 MB (108374945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ba34ba5f00c190ce6f8e3baaba9c5c3744d4d35e1089330de85b671c3bebcc`  
		Last Modified: Wed, 01 Sep 2021 23:45:12 GMT  
		Size: 6.3 MB (6297481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8bd0a1dcff86704d185d2f6351a40e939ae6cd24cfbc62b1d3e97a207a3e5c`  
		Last Modified: Wed, 01 Sep 2021 23:45:40 GMT  
		Size: 314.1 MB (314139794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284b93c6d3ecdc1b53dd4558a3ef0af56432cdef90bbb2eecd2950c34ef95bea`  
		Last Modified: Wed, 01 Sep 2021 23:45:08 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc60c415e2bb617c94a3876f2fd0887e13e3fee063dee2cdb792fef7f1d4b29c`  
		Last Modified: Wed, 01 Sep 2021 23:45:42 GMT  
		Size: 362.4 MB (362421001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1180574f7e37b30333a2d8f1007170fc60155ead135ba1734dd043696bb71180`  
		Last Modified: Wed, 01 Sep 2021 23:45:08 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae08843cb628c330f14cbe4453cef65ce7a7ed3f08950d10c0f20ab258f2c1f0`  
		Last Modified: Wed, 01 Sep 2021 23:45:08 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05ba317a4c274dbda1def82ef96dcf6b08a1f5dbee500d3bb958d2981811a42`  
		Last Modified: Wed, 01 Sep 2021 23:45:04 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc8c1b8a94f5dd2f65884b76325f3630fd6ead7386ae607384c975d976a8cf7`  
		Last Modified: Wed, 01 Sep 2021 23:45:05 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a9b227a38e2a1906cdf117d0ccda1969c6eec0aefe7bd4b15968df573c1547`  
		Last Modified: Wed, 01 Sep 2021 23:45:05 GMT  
		Size: 2.8 KB (2758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54933130fe9976408ed40d4fba8fa5e74b81b69669df8d2c7ac75012956d9f5b`  
		Last Modified: Wed, 01 Sep 2021 23:45:04 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54933130fe9976408ed40d4fba8fa5e74b81b69669df8d2c7ac75012956d9f5b`  
		Last Modified: Wed, 01 Sep 2021 23:45:04 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe55efd67658f81a1b95abf44fb006f102a915837cb9107f1a8e939276b8e863`  
		Last Modified: Wed, 01 Sep 2021 23:45:04 GMT  
		Size: 944.2 KB (944168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
