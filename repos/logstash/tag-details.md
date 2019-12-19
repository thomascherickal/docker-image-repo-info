<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `logstash`

-	[`logstash:6.8.6`](#logstash686)
-	[`logstash:7.5.1`](#logstash751)

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

## `logstash:7.5.1`

```console
$ docker pull logstash@sha256:e6d4b599304c9b48ccac9b612a00fd2384bf81f473847b48b52931e02d9f1da6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `logstash:7.5.1` - linux; amd64

```console
$ docker pull logstash@sha256:5de599b41ebb9478ddfaa0ce307d7264585ad9e14984c0f9691e036eb5cec2d6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.1 MB (348093206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b94897b4254eaca4a44fed3b696e6dd26d485a23dfd0d79f8c305a29fe3785b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint"]`

```dockerfile
# Tue, 12 Nov 2019 00:20:33 GMT
ADD file:45a381049c52b5664e5e911dead277b25fadbae689c0bb35be3c42dff0f2dffe in / 
# Tue, 12 Nov 2019 00:20:33 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20191001
# Tue, 12 Nov 2019 00:20:33 GMT
CMD ["/bin/bash"]
# Tue, 17 Dec 2019 01:00:25 GMT
RUN yum update -y && yum install -y java-11-openjdk-devel which &&     yum clean all
# Tue, 17 Dec 2019 01:00:27 GMT
RUN groupadd --gid 1000 logstash &&     adduser --uid 1000 --gid 1000       --home-dir /usr/share/logstash --no-create-home       logstash
# Tue, 17 Dec 2019 01:00:45 GMT
RUN curl -Lo - http://localhost:8000/logstash-7.5.1.tar.gz |     tar zxf - -C /usr/share &&     mv /usr/share/logstash-7.5.1 /usr/share/logstash &&     chown --recursive logstash:logstash /usr/share/logstash/ &&     chown -R logstash:root /usr/share/logstash &&     chmod -R g=u /usr/share/logstash &&     find /usr/share/logstash -type d -exec chmod g+s {} \; &&     ln -s /usr/share/logstash /opt/logstash
# Tue, 17 Dec 2019 01:00:46 GMT
WORKDIR /usr/share/logstash
# Tue, 17 Dec 2019 01:00:47 GMT
ENV ELASTIC_CONTAINER=true
# Tue, 17 Dec 2019 01:00:47 GMT
ENV PATH=/usr/share/logstash/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Dec 2019 01:00:48 GMT
ADD file:1183410472ec370104718a08e1144081518db1d006a8cc82de824a34455ab3f3 in config/pipelines.yml 
# Tue, 17 Dec 2019 01:00:51 GMT
ADD file:83ab096464b764c812ae68c2872c05d48ee1620e6a1629948d52c13ac6dcfe11 in config/logstash.yml 
# Tue, 17 Dec 2019 01:00:52 GMT
ADD file:2ef21d4766eab3ac48ed3847c8b8d05554f1fd0b39061cba66c9ac93240087fa in config/ 
# Tue, 17 Dec 2019 01:00:52 GMT
ADD file:0cd9cc51daf5f37b2aa8aae8cf3570a3680e22852afb2803ccb87ddcd3369f52 in pipeline/logstash.conf 
# Tue, 17 Dec 2019 01:00:54 GMT
RUN chown --recursive logstash:root config/ pipeline/
# Tue, 17 Dec 2019 01:00:54 GMT
ENV LANG=en_US.UTF-8 LC_ALL=en_US.UTF-8
# Tue, 17 Dec 2019 01:00:55 GMT
ADD file:29dd60f159d64086c20a7a02f84a9314f44b2290304547233fb96744325b1245 in /usr/local/bin/ 
# Tue, 17 Dec 2019 01:00:57 GMT
RUN chmod 0755 /usr/local/bin/docker-entrypoint
# Tue, 17 Dec 2019 01:00:57 GMT
USER 1000
# Tue, 17 Dec 2019 01:00:57 GMT
ADD file:5c5ccdd4a384a7e48f2bbf2c337adb705946473c1c2a21ccf4079e623da60dcb in /usr/local/bin/ 
# Tue, 17 Dec 2019 01:00:58 GMT
EXPOSE 5044 9600
# Tue, 17 Dec 2019 01:00:58 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.vendor=Elastic org.label-schema.name=logstash org.label-schema.version=7.5.1 org.label-schema.url=https://www.elastic.co/products/logstash org.label-schema.vcs-url=https://github.com/elastic/logstash license=Elastic License
# Tue, 17 Dec 2019 01:00:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint"]
```

-	Layers:
	-	`sha256:ab5ef0e5819490abe86106fd9f4381123e37a03e80e650be39f7938d30ecb530`  
		Last Modified: Tue, 12 Nov 2019 00:23:38 GMT  
		Size: 75.8 MB (75780712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc545bd3b3b2307471e6acb576faaefdac3dc20c1285fc0a406351817fa0cb49`  
		Last Modified: Wed, 18 Dec 2019 19:18:43 GMT  
		Size: 104.9 MB (104863670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee994bc7ab09ed2f251331063db602b05dd8608abdaf2437bb93a409d458b3e`  
		Last Modified: Wed, 18 Dec 2019 19:15:09 GMT  
		Size: 1.9 KB (1851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b63c35d1b192390a75b9b0efd118846ce23bf42f28baa9f273250e89ab9173`  
		Last Modified: Wed, 18 Dec 2019 19:18:46 GMT  
		Size: 166.4 MB (166437946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5477bd81016f959627c4d8e8563951e2ec7c48945f081b7c3740c1616976aae`  
		Last Modified: Wed, 18 Dec 2019 19:15:00 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5411daa27df029d570a30e24dd367a35e51c769d139775e38ef3cb5185448ec`  
		Last Modified: Wed, 18 Dec 2019 19:14:59 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe5fce4cbec2f5996ef5ba6a7df9b0f406ac955b666607b7553bbbb7921debc`  
		Last Modified: Wed, 18 Dec 2019 19:14:55 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04709fffcd2badf9c847beebbeb5ad4f097fa3d20e1c259d9962490b8089e99`  
		Last Modified: Wed, 18 Dec 2019 19:14:49 GMT  
		Size: 290.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:658ce93638c14fd6ba762557f55de33943ead6ed0147a8c144da5266b2ab1918`  
		Last Modified: Wed, 18 Dec 2019 19:14:46 GMT  
		Size: 2.7 KB (2732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67afcc270a2cbd41a76feff279dd59ae9516d59575eb3dbeeb6e20ff20cac96a`  
		Last Modified: Wed, 18 Dec 2019 19:14:49 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67afcc270a2cbd41a76feff279dd59ae9516d59575eb3dbeeb6e20ff20cac96a`  
		Last Modified: Wed, 18 Dec 2019 19:14:49 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a29abf3dd10b11fff17300693f067c34d0eb5df220c5f9816cfe87704a1aa4`  
		Last Modified: Wed, 18 Dec 2019 19:14:49 GMT  
		Size: 1.0 MB (1003868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
