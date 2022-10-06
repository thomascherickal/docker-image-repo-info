<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:6.8.23`](#logstash6823)
-	[`logstash:7.17.6`](#logstash7176)
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

## `logstash:7.17.6`

```console
$ docker pull logstash@sha256:90a4cca2b81abef53a5ae17275d71dd928ed13de14c8ae00e3f0686baeb28e05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `logstash:7.17.6` - linux; amd64

```console
$ docker pull logstash@sha256:b917b0e44bfd6e57a413b9175fc8c3d5a1bf6d2bb3932bd63e9758a18c08ef0b
```

-	Docker Version: 20.10.16
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **437.4 MB (437433126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c2e7b4094afcc58d77afb9ae5735a9ef054a32c19f7b2014e4f9874b643af2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:57:29 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Tue, 23 Aug 2022 11:57:30 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Tue, 23 Aug 2022 11:57:55 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.6-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.6 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Tue, 23 Aug 2022 11:57:58 GMT
WORKDIR /usr/share/logstash
# Tue, 23 Aug 2022 11:57:58 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 23 Aug 2022 11:57:58 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:57:58 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Tue, 23 Aug 2022 11:57:59 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Tue, 23 Aug 2022 11:57:59 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Tue, 23 Aug 2022 11:57:59 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Tue, 23 Aug 2022 11:57:59 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Tue, 23 Aug 2022 11:57:59 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 23 Aug 2022 11:58:00 GMT
ADD file:54c2eca60400e5966528ae8d5151554a6d52f2a469f9736982721f7458b30af5 in /usr/local/bin/ 
# Tue, 23 Aug 2022 11:58:00 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Tue, 23 Aug 2022 11:58:00 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Tue, 23 Aug 2022 11:58:00 GMT
USER 1000
# Tue, 23 Aug 2022 11:58:00 GMT
EXPOSE 5044 9600
# Tue, 23 Aug 2022 11:58:01 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.6 org.opencontainers.image.version=7.17.6 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-08-23T11:10:30Z org.opencontainers.image.created=2022-08-23T11:10:30Z
# Tue, 23 Aug 2022 11:58:01 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b74842ce49533cb961d70dde4c2b1491ecd2d9701164e5e4c72bef8153642d`  
		Last Modified: Wed, 24 Aug 2022 23:09:43 GMT  
		Size: 40.3 MB (40334795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a537956c621882072065d24462917601f2c8808c9e4cfd26ba66f57e280a11a2`  
		Last Modified: Wed, 24 Aug 2022 23:09:39 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5245bd32a8928ebf5ff52535fc742dd4960879b4cd64f24630ff0e5db2920471`  
		Last Modified: Wed, 24 Aug 2022 23:10:04 GMT  
		Size: 366.8 MB (366751651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0424569c78b7988cabd28b16c816dd1d31a031eec976915ba70bcc364c77e3`  
		Last Modified: Wed, 24 Aug 2022 23:09:37 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd6a4418c59f6dc401150348147896badcec6bd0ab969ddba5762c0e4c03db8`  
		Last Modified: Wed, 24 Aug 2022 23:09:37 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0e2ef05a7145cf029971ca122e6a5e4354cd8b5fbe5863acb9c37d757dd273`  
		Last Modified: Wed, 24 Aug 2022 23:09:37 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7151029b5399bc3ea6d3a501ab76f24a3d42b7b0fe9cfee34b639c3cbbf96a7c`  
		Last Modified: Wed, 24 Aug 2022 23:09:36 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d233826fbf49a4bedc0c1354a83c42a1a45afcb21a0db57d4d09f4e2bd2fe2ae`  
		Last Modified: Wed, 24 Aug 2022 23:09:36 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f0e639309c4fadfdc401824a6cb2642c73a0178ffcec8164906ba427a45095`  
		Last Modified: Wed, 24 Aug 2022 23:09:36 GMT  
		Size: 1.8 MB (1766959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb5fc33b3d61b42d6c1c48005824320924716ff4795786e4907a2ae0e021bc6`  
		Last Modified: Wed, 24 Aug 2022 23:09:36 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb5fc33b3d61b42d6c1c48005824320924716ff4795786e4907a2ae0e021bc6`  
		Last Modified: Wed, 24 Aug 2022 23:09:36 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `logstash:7.17.6` - linux; arm64 variant v8

```console
$ docker pull logstash@sha256:f3cdcc279e2e27426536d2a840809114164ad663e4d2f09077ea601536b080b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.1 MB (427127905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:164cc6b20b2c050bc3ee26fb05a674ee7c3ccb11dd408eaf15742737da3addfa`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:25:09 GMT
RUN for iter in {1..10}; do export DEBIAN_FRONTEND=noninteractive && apt-get update -y && apt-get upgrade -y && apt-get install -y procps findutils tar gzip curl && apt-get install -y locales && apt-get clean all && locale-gen 'en_US.UTF-8' &&     apt-get clean metadata && exit_code=0 && break || exit_code=$? &&     echo "packaging error: retry $iter in 10s" &&     apt-get clean all && apt-get clean metadata && sleep 10; done;     (exit $exit_code)
# Tue, 23 Aug 2022 11:25:10 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000        --home /usr/share/logstash --no-create-home       logstash
# Tue, 23 Aug 2022 11:25:29 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.17.6-linux-$(arch).tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.17.6 /usr/share/logstash && chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     mkdir /licenses/ &&     mv /usr/share/logstash/NOTICE.TXT /licenses/NOTICE.TXT &&     mv /usr/share/logstash/LICENSE.txt /licenses/LICENSE.txt &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Tue, 23 Aug 2022 11:25:30 GMT
WORKDIR /usr/share/logstash
# Tue, 23 Aug 2022 11:25:30 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 23 Aug 2022 11:25:30 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:25:30 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Tue, 23 Aug 2022 11:25:30 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Tue, 23 Aug 2022 11:25:31 GMT
ADD file:4f39d77a8986c28d67e673d4691e69ca9c175574128b0819977c2d1bb0d6e950 in config/ 
# Tue, 23 Aug 2022 11:25:31 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Tue, 23 Aug 2022 11:25:31 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Tue, 23 Aug 2022 11:25:31 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 23 Aug 2022 11:25:31 GMT
ADD file:3d1f0371871b2cf544bfbe665b8987dec9351631beb484d0e94b862d6398217f in /usr/local/bin/ 
# Tue, 23 Aug 2022 11:25:31 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Tue, 23 Aug 2022 11:25:32 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Tue, 23 Aug 2022 11:25:32 GMT
USER 1000
# Tue, 23 Aug 2022 11:25:32 GMT
EXPOSE 5044 9600
# Tue, 23 Aug 2022 11:25:32 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.opencontainers.image.vendor=Elastic org.label-schema.name=logstash org.opencontainers.image.title=logstash org.label-schema.version=7.17.6 org.opencontainers.image.version=7.17.6 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash org.label-schema.license=Elastic License org.opencontainers.image.licenses=Elastic License org.opencontainers.image.description=Logstash is a free and open server-side data processing pipeline that ingests data from a multitude of sources, transforms it, and then sends it to your favorite 'stash.' org.label-schema.build-date=2022-08-23T11:11:52+00:00 org.opencontainers.image.created=2022-08-23T11:11:52+00:00
# Tue, 23 Aug 2022 11:25:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9783234ac6a12760d6d608273912a2dfac353504d434ab099c4ed9e23ef69721`  
		Last Modified: Thu, 25 Aug 2022 02:13:01 GMT  
		Size: 34.8 MB (34780717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c576909f02ab27c4a437a2f0d4a2fbdebf98e589a0f9f806f11a7a1b1a685422`  
		Last Modified: Thu, 25 Aug 2022 02:12:56 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a880bd31b44117fdfc883bcd7155cff12d5c1cd6d70c2142078b232b3a19e75`  
		Last Modified: Thu, 25 Aug 2022 02:13:29 GMT  
		Size: 363.5 MB (363502333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04141985c7973cfd0acdcd15149a14697b6ea28f760b7b9de8acf1e16af41fc`  
		Last Modified: Thu, 25 Aug 2022 02:12:56 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4e25cb7184829cc698b5d96c08d300c9626e2902e609a6d55cfae3a8663a46`  
		Last Modified: Thu, 25 Aug 2022 02:12:56 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7489eca5a04f700ae6a760f06f3352346e90c925389b44bad2c0cfda7a5b0b7`  
		Last Modified: Thu, 25 Aug 2022 02:12:54 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2533daf42627bf01ae01478637b5eee9ca0be2273cfb8a599027aa16fc87f17f`  
		Last Modified: Thu, 25 Aug 2022 02:12:54 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb75c9b04f078829a36ba0fb30815385286a8676cfd2fa98b8a6a1c9eb4c2e34`  
		Last Modified: Thu, 25 Aug 2022 02:12:53 GMT  
		Size: 2.9 KB (2855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac20888c256e12d91be4fc6525545906d90bf2a3e0462eb78c1903028ac19512`  
		Last Modified: Thu, 25 Aug 2022 02:12:54 GMT  
		Size: 1.6 MB (1645927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4adc3d721113b1f0f4da8875e17176f00425e296981eecbf9eeb4671558ffbc`  
		Last Modified: Thu, 25 Aug 2022 02:12:54 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4adc3d721113b1f0f4da8875e17176f00425e296981eecbf9eeb4671558ffbc`  
		Last Modified: Thu, 25 Aug 2022 02:12:54 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:8.4.3`

```console
$ docker pull logstash@sha256:19c18fa8a451294c113f1a0500ce8f9fb7366650672c8b8506ceaab6a0ad003f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

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
