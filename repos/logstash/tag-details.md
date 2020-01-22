<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:6.8.6`](#logstash686)
-	[`logstash:7.5.2`](#logstash752)

## `logstash:6.8.6`

```console
$ docker pull logstash@sha256:0ae81d624d8791c37c8919453fb3efe144ae665ad921222da97bc761d2a002fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `logstash:6.8.6` - linux; amd64

```console
$ docker pull logstash@sha256:0ed0f4605e6848b9ae2df7edf6092abf475c4cdf0f591e00d5e15e4b1e5e1961
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.7 MB (360730159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a2dac51fcba76c923e78c0e4d0584cfc329a388d3201dd0f8affb4083e3566`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Fri, 13 Dec 2019 18:42:44 GMT
RUN yum update -y && yum install -y java-1.8.0-openjdk-devel which &&     yum clean all
# Fri, 13 Dec 2019 18:42:47 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home-dir /usr/share/logstash --no-create-home       logstash
# Fri, 13 Dec 2019 18:43:05 GMT
RUN curl -Lo - http://localhost:8000/logstash-6.8.6.tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-6.8.6 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Fri, 13 Dec 2019 18:43:07 GMT
WORKDIR /usr/share/logstash
# Fri, 13 Dec 2019 18:43:07 GMT
ENV ELASTIC_CONTAINER=true
# Fri, 13 Dec 2019 18:43:07 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Dec 2019 18:43:08 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Fri, 13 Dec 2019 18:43:08 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Fri, 13 Dec 2019 18:43:09 GMT
ADD file:2ef21d4766eab3ac48ed3847c8b8d05554f1fd0b39061cba66c9ac93240087fa in config/ 
# Fri, 13 Dec 2019 18:43:10 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Fri, 13 Dec 2019 18:43:11 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Fri, 13 Dec 2019 18:43:12 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Fri, 13 Dec 2019 18:43:12 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Fri, 13 Dec 2019 18:43:14 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Fri, 13 Dec 2019 18:43:15 GMT
USER 1000
# Fri, 13 Dec 2019 18:43:15 GMT
ADD file:a1fa9fe469353a32c6235ac29d14359edb94869d1926454f9ca23b82edcc0ffc in /usr/local/bin/ 
# Fri, 13 Dec 2019 18:43:15 GMT
EXPOSE 5044 9600
# Fri, 13 Dec 2019 18:43:16 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=logstash org.label-schema.version=6.8.6 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash license=Elastic License
# Fri, 13 Dec 2019 18:43:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bdff85c0eff7ab1a09ad8158008b8e990aa90d33c90ea202b45e28f71c6e25`  
		Last Modified: Wed, 18 Dec 2019 22:16:38 GMT  
		Size: 109.6 MB (109552546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4021eabbe3180c8dcec53f8fa5d5359ef340a147d9641c3408e19fb1852f6d`  
		Last Modified: Wed, 18 Dec 2019 22:16:17 GMT  
		Size: 1.9 KB (1850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04880b09f62d1cb728ce5e8c8c6c5c7e323d5b6ea1fb15d093d19cea86a6b977`  
		Last Modified: Wed, 18 Dec 2019 22:16:40 GMT  
		Size: 174.4 MB (174386096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495c57fa286715edb24259be89395b8f73f05b9f78f5c1231211221b02827227`  
		Last Modified: Wed, 18 Dec 2019 22:16:17 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1226a1298464eaee4cd0c7f2f0e9ec9e3cf2ebb49eb9eaaaf7fdee0ea54158e`  
		Last Modified: Wed, 18 Dec 2019 22:16:17 GMT  
		Size: 290.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a368341d068565e2c273e96c1b38b9a93441b01aeb89584c84d6c03ee4af02ab`  
		Last Modified: Wed, 18 Dec 2019 22:16:15 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bfc3cf8fb89723d8e89f8d84a81fc9bbaf10ff3e4e2f907488f762a33f279c`  
		Last Modified: Wed, 18 Dec 2019 22:16:15 GMT  
		Size: 290.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89333ddd001c9767be57b01ab275a2f4353c6d84318c43e9e496ddfdf31d8c58`  
		Last Modified: Wed, 18 Dec 2019 22:16:16 GMT  
		Size: 2.7 KB (2688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289ecf0bfa6d12f845127106689e238d4ee5bf7cd50ed1deba1ee29d2b3c497d`  
		Last Modified: Wed, 18 Dec 2019 22:16:15 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289ecf0bfa6d12f845127106689e238d4ee5bf7cd50ed1deba1ee29d2b3c497d`  
		Last Modified: Wed, 18 Dec 2019 22:16:15 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b388674055ddf13068915d66e67791d36f86ca7d84194bb61b7942ae6781861d`  
		Last Modified: Wed, 18 Dec 2019 22:16:15 GMT  
		Size: 1.0 MB (1003841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:7.5.2`

**does not exist** (yet?)
