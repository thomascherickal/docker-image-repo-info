<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:6.8.7`](#logstash687)
-	[`logstash:7.6.1`](#logstash761)

## `logstash:6.8.7`

```console
$ docker pull logstash@sha256:b035a31e852168fbab1d55876997bf850599cbe5bb6d4edb99cc55111b01d652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `logstash:6.8.7` - linux; amd64

```console
$ docker pull logstash@sha256:58bf2abcec3e4dd4dcba035840e06895264c04647b4b11f4bef5d91c5318cfac
```

-	Docker Version: 19.03.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.5 MB (367520077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711f044e9da728c98036e2cf1012c9528527c74ef605b08276e0ad11456d15eb`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Wed, 26 Feb 2020 16:16:50 GMT
RUN yum update -y && yum install -y java-1.8.0-openjdk-devel which &&     yum clean all
# Wed, 26 Feb 2020 16:16:54 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home-dir /usr/share/logstash --no-create-home       logstash
# Wed, 26 Feb 2020 16:17:10 GMT
RUN curl -Lo - http://localhost:8000/logstash-6.8.7.tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-6.8.7 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Wed, 26 Feb 2020 16:17:12 GMT
WORKDIR /usr/share/logstash
# Wed, 26 Feb 2020 16:17:12 GMT
ENV ELASTIC_CONTAINER=true
# Wed, 26 Feb 2020 16:17:13 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 16:17:14 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Wed, 26 Feb 2020 16:17:15 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Wed, 26 Feb 2020 16:17:16 GMT
ADD file:2ef21d4766eab3ac48ed3847c8b8d05554f1fd0b39061cba66c9ac93240087fa in config/ 
# Wed, 26 Feb 2020 16:17:17 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Wed, 26 Feb 2020 16:17:21 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Wed, 26 Feb 2020 16:17:22 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Wed, 26 Feb 2020 16:17:23 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Wed, 26 Feb 2020 16:17:25 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Wed, 26 Feb 2020 16:17:26 GMT
USER 1000
# Wed, 26 Feb 2020 16:17:26 GMT
ADD file:cebf0ff7ebe120c237a4cd02789b4d90543b551aaeb6a2e695b7ed3070e28792 in /usr/local/bin/ 
# Wed, 26 Feb 2020 16:17:26 GMT
EXPOSE 5044 9600
# Wed, 26 Feb 2020 16:17:27 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=logstash org.label-schema.version=6.8.7 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash license=Elastic License
# Wed, 26 Feb 2020 16:17:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5215ff6def3a4ca2cb05c094753f325a8eae6e8c21691a27c2b71d3a0b006b06`  
		Last Modified: Wed, 04 Mar 2020 22:16:49 GMT  
		Size: 110.1 MB (110074846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53073c3ab622466f2ec4b2055966bfe0d214a109c57944af76b86833c803033e`  
		Last Modified: Wed, 04 Mar 2020 22:16:27 GMT  
		Size: 1.9 KB (1851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06450364b7b4bbc4a0b5924c72836469e25aa5f180d1b174715e5c54d781208b`  
		Last Modified: Wed, 04 Mar 2020 22:16:48 GMT  
		Size: 180.7 MB (180653117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3588fa7fc3f563233eba831e75a8a563c76d5ee61ba3240a6bfd0e7fd5c255`  
		Last Modified: Wed, 04 Mar 2020 22:16:27 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a9f1661afb1d59a1f84fe5c9ccbff40706243ee357237825c8fa122c2e17b4`  
		Last Modified: Wed, 04 Mar 2020 22:16:27 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01fdb7ebc031d188817df2bc7ac6be2ed796eb86e32e7f9a23eaa90557b74a2`  
		Last Modified: Wed, 04 Mar 2020 22:16:25 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a41a15116d50c6c62fea6870182bd428340ceb851437d7d4c0314631e0b59d`  
		Last Modified: Wed, 04 Mar 2020 22:16:25 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03158bfab0492bb31130642ef09d415114b4f029213d9c67be2654b43cde9b25`  
		Last Modified: Wed, 04 Mar 2020 22:16:26 GMT  
		Size: 2.7 KB (2690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aeb2bf332f5ea620fa492da5b1e1ae79fd860d7b6e98539b064fbc3093ae6fb`  
		Last Modified: Wed, 04 Mar 2020 22:16:25 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aeb2bf332f5ea620fa492da5b1e1ae79fd860d7b6e98539b064fbc3093ae6fb`  
		Last Modified: Wed, 04 Mar 2020 22:16:25 GMT  
		Size: 502.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c855a0da1ec27c81332ec7e0c5eaac03c5f4b940a7c314658cae72b05defc4c4`  
		Last Modified: Wed, 04 Mar 2020 22:16:26 GMT  
		Size: 1.0 MB (1004422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:7.6.1`

```console
$ docker pull logstash@sha256:a3f6e34d17ecf311ae6b6f22985b60c6f9c7261d3831dba6c0622fba98b7e0b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `logstash:7.6.1` - linux; amd64

```console
$ docker pull logstash@sha256:06ffc882111a3b205a203d87257a1c6108ea3a8f348f11adf202936116c60b86
```

-	Docker Version: 19.03.6
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.5 MB (355534904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d66afe6805ea80e819f4a7725297bbe7c5a0adfab137ebc44f895e299fd6b5`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Sat, 29 Feb 2020 02:00:28 GMT
RUN yum update -y && yum install -y java-11-openjdk-devel which &&     yum clean all
# Sat, 29 Feb 2020 02:00:28 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home-dir /usr/share/logstash --no-create-home       logstash
# Sat, 29 Feb 2020 02:00:38 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.6.1.tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.6.1 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Sat, 29 Feb 2020 02:00:38 GMT
WORKDIR /usr/share/logstash
# Sat, 29 Feb 2020 02:00:38 GMT
ENV ELASTIC_CONTAINER=true
# Sat, 29 Feb 2020 02:00:38 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 29 Feb 2020 02:00:38 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Sat, 29 Feb 2020 02:00:38 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Sat, 29 Feb 2020 02:00:39 GMT
ADD file:67a3543613849420f3c5597cdf7f793b85362365cfa372b40a93ed03d46feadc in config/ 
# Sat, 29 Feb 2020 02:00:39 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Sat, 29 Feb 2020 02:00:40 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Sat, 29 Feb 2020 02:00:40 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Sat, 29 Feb 2020 02:00:40 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Sat, 29 Feb 2020 02:00:41 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Sat, 29 Feb 2020 02:00:41 GMT
USER 1000
# Sat, 29 Feb 2020 02:00:41 GMT
ADD file:27413a36073280132d63a9a255bb2ff3bccb55f07e11020493fefa619a65018c in /usr/local/bin/ 
# Sat, 29 Feb 2020 02:00:41 GMT
EXPOSE 5044 9600
# Sat, 29 Feb 2020 02:00:41 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=logstash org.label-schema.version=7.6.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash license=Elastic License
# Sat, 29 Feb 2020 02:00:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9f98078865ff34d98ecbf9e93a503ddef0192e8078eb7ebb44752433d8c849`  
		Last Modified: Wed, 04 Mar 2020 21:10:13 GMT  
		Size: 105.4 MB (105368074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff370996b4cbace2722415bdbee58596af7db7e71a2456ad4f6248ed9b0c88b`  
		Last Modified: Wed, 04 Mar 2020 21:09:41 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6ee64d0b6e9d7767d3e7726eb9efbc09324267ddaecb7be0f38fd47cad6fee`  
		Last Modified: Wed, 04 Mar 2020 22:17:37 GMT  
		Size: 173.4 MB (173374624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87a577c546e3dd5ee0264351d52ae4b60e1f56cf9632cb0d7507e61c64c5589`  
		Last Modified: Wed, 04 Mar 2020 22:17:14 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568954398fecbbd1407be7711d31d907b8e4c561c3c40d3ef828da62ee13f6e0`  
		Last Modified: Wed, 04 Mar 2020 22:17:12 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8994fc6fb9607162201fb2c98696848e8eb2521b8dc23fa0eafba24e1e9ccac2`  
		Last Modified: Wed, 04 Mar 2020 22:17:11 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d59412283e0ae1a6a284215a647811516f9608c63220bcfce193fe3e4a38dc`  
		Last Modified: Wed, 04 Mar 2020 22:17:10 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ddb8ceb1a721697ec11c916ba000ffe137cfaabd38f821171424a40cea2970`  
		Last Modified: Wed, 04 Mar 2020 22:17:11 GMT  
		Size: 2.8 KB (2750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a9c0701679d0d176b74c087198981fe51c713e06233e25a3b8b2789a966d86`  
		Last Modified: Wed, 04 Mar 2020 22:17:11 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a9c0701679d0d176b74c087198981fe51c713e06233e25a3b8b2789a966d86`  
		Last Modified: Wed, 04 Mar 2020 22:17:11 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70afa1fcd951c320e595feeb4f4e6921837c8fd1d07da4fa8f5acdeda1250d4`  
		Last Modified: Wed, 04 Mar 2020 22:17:11 GMT  
		Size: 1.0 MB (1004432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
