<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:6.8.10`](#logstash6810)
-	[`logstash:7.8.0`](#logstash780)

## `logstash:6.8.10`

```console
$ docker pull logstash@sha256:d708bce6972149394b4b4a8be08634d6852061dca476c7cbc0863e4f7d12d828
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `logstash:6.8.10` - linux; amd64

```console
$ docker pull logstash@sha256:eb37d6e87574dba70e050b83ab3c5f063c905b1d61e639def9ec9c978833aa62
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.0 MB (361028883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:526c0151af4538248e7d8865aa325747d01a3e76526fcf71c208261ebed25dbc`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Thu, 28 May 2020 16:31:55 GMT
RUN yum update -y && yum install -y java-1.8.0-openjdk-devel which &&     yum clean all
# Thu, 28 May 2020 16:31:57 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home-dir /usr/share/logstash --no-create-home       logstash
# Thu, 28 May 2020 16:32:17 GMT
RUN curl -Lo - http://localhost:8000/logstash-6.8.10.tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-6.8.10 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Thu, 28 May 2020 16:32:18 GMT
WORKDIR /usr/share/logstash
# Thu, 28 May 2020 16:32:18 GMT
ENV ELASTIC_CONTAINER=true
# Thu, 28 May 2020 16:32:18 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 28 May 2020 16:32:19 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Thu, 28 May 2020 16:32:20 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Thu, 28 May 2020 16:32:20 GMT
ADD file:2ef21d4766eab3ac48ed3847c8b8d05554f1fd0b39061cba66c9ac93240087fa in config/ 
# Thu, 28 May 2020 16:32:20 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Thu, 28 May 2020 16:32:24 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Thu, 28 May 2020 16:32:24 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Thu, 28 May 2020 16:32:24 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Thu, 28 May 2020 16:32:26 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Thu, 28 May 2020 16:32:26 GMT
USER 1000
# Thu, 28 May 2020 16:32:27 GMT
ADD file:571dd4a165fa42134dca8ddb671372023424aeaef9b0ed94f044c92e999f584e in /usr/local/bin/ 
# Thu, 28 May 2020 16:32:29 GMT
EXPOSE 5044 9600
# Thu, 28 May 2020 16:32:29 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=logstash org.label-schema.version=6.8.10 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash license=Elastic License
# Thu, 28 May 2020 16:32:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0564234b8d933dde6982a630692c7145e647988bc8b468454f10f4a054fbbb24`  
		Last Modified: Wed, 03 Jun 2020 14:39:52 GMT  
		Size: 103.5 MB (103500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e675a5584f4a3f6757c6afa8cc39e4b6cc280986318c09491e3eb288df439c9d`  
		Last Modified: Wed, 03 Jun 2020 14:39:27 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab751bd7539b4a2ab72e39b9fdab3dda68bc5e7c8cf55febf8e899775837845`  
		Last Modified: Wed, 03 Jun 2020 14:41:33 GMT  
		Size: 180.6 MB (180636346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e846d0aad67421d1233492655c3b76a0b7dc4e257c3a2aeb249040eaf2a2272`  
		Last Modified: Wed, 03 Jun 2020 14:41:16 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ef45e4200114247b81a213f1997d8cdfca73a3d5e3e686a86d38e97fc08ed5`  
		Last Modified: Wed, 03 Jun 2020 14:41:16 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec508da052ae19eb57b6d724af59c0d1cba54528f98b57b1c132adefdbf4e75`  
		Last Modified: Wed, 03 Jun 2020 14:41:14 GMT  
		Size: 444.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50dd75d0b2c5724fe21b3a5eda5b961e8d725b7a43075749f92b17c47dfcaf8`  
		Last Modified: Wed, 03 Jun 2020 14:41:14 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5531ea14d2132f90fb7601e949db23395f0646d10580b6a708743fc142c84542`  
		Last Modified: Wed, 03 Jun 2020 14:41:14 GMT  
		Size: 2.7 KB (2670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f319fd7b3bce9e60aadd4635dbff1703493c2c08bf833ccd19c627ba44220a5c`  
		Last Modified: Wed, 03 Jun 2020 14:41:14 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f319fd7b3bce9e60aadd4635dbff1703493c2c08bf833ccd19c627ba44220a5c`  
		Last Modified: Wed, 03 Jun 2020 14:41:14 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f81e225e1ef475e9680af7a06b2c79f01522b1293d6f481e33ca070eb6e91d`  
		Last Modified: Wed, 03 Jun 2020 14:41:15 GMT  
		Size: 1.0 MB (1004571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `logstash:7.8.0`

**does not exist** (yet?)
