<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `sapmachine`

-	[`sapmachine:11`](#sapmachine11)
-	[`sapmachine:11.0.12`](#sapmachine11012)
-	[`sapmachine:16`](#sapmachine16)
-	[`sapmachine:16.0.1`](#sapmachine1601)
-	[`sapmachine:latest`](#sapmachinelatest)
-	[`sapmachine:lts`](#sapmachinelts)

## `sapmachine:11`

```console
$ docker pull sapmachine@sha256:64f962b59a38601f0dfa722f3e4c0cb84120e19ba129a8ba752a00cac9435d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:11` - linux; amd64

```console
$ docker pull sapmachine@sha256:3fbe8a57dc9eaddbd537858fe6f63597d30d5930c0cbb1d9f85811f657d035c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235078815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86c7a628e1fafc0ac5324a1abcc3380f3aa74b831368ed7779822a5eeb8eec0a`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 11:18:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:19:27 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.12     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:19:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Fri, 23 Jul 2021 11:19:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a1dc0613013ab06a3796ab75ed46b0ea7cc088afb355824c42ca579549e808`  
		Last Modified: Fri, 23 Jul 2021 11:19:52 GMT  
		Size: 8.3 MB (8321638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404dc7bf13ef94ae0b9bc30be2735edc96d5f63e878776351e34cbafa080d4c3`  
		Last Modified: Fri, 23 Jul 2021 11:20:29 GMT  
		Size: 198.2 MB (198191314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:11.0.12`

```console
$ docker pull sapmachine@sha256:64f962b59a38601f0dfa722f3e4c0cb84120e19ba129a8ba752a00cac9435d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:11.0.12` - linux; amd64

```console
$ docker pull sapmachine@sha256:3fbe8a57dc9eaddbd537858fe6f63597d30d5930c0cbb1d9f85811f657d035c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235078815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86c7a628e1fafc0ac5324a1abcc3380f3aa74b831368ed7779822a5eeb8eec0a`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 11:18:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:19:27 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.12     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:19:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Fri, 23 Jul 2021 11:19:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a1dc0613013ab06a3796ab75ed46b0ea7cc088afb355824c42ca579549e808`  
		Last Modified: Fri, 23 Jul 2021 11:19:52 GMT  
		Size: 8.3 MB (8321638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404dc7bf13ef94ae0b9bc30be2735edc96d5f63e878776351e34cbafa080d4c3`  
		Last Modified: Fri, 23 Jul 2021 11:20:29 GMT  
		Size: 198.2 MB (198191314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:16`

```console
$ docker pull sapmachine@sha256:f0024196c3979f7ab4b898bc13b95d928384c5c10f665884e05944adc93a8591
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:16` - linux; amd64

```console
$ docker pull sapmachine@sha256:e7262cee5b22868fbbd7f6dbd01b64c5490a81937ece9995aa34f6c24f064af0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.3 MB (248328836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1685b62917509255abeda2436f1ccd581bd601b75485054886fcfacbee25376`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 11:18:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 20:20:41 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-16-jdk=16.0.2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 20:20:42 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-16
# Fri, 23 Jul 2021 20:20:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a1dc0613013ab06a3796ab75ed46b0ea7cc088afb355824c42ca579549e808`  
		Last Modified: Fri, 23 Jul 2021 11:19:52 GMT  
		Size: 8.3 MB (8321638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88652fa7a781f4b350d322eea7bc697551743a37047938903dd158d05d44f72d`  
		Last Modified: Fri, 23 Jul 2021 20:21:17 GMT  
		Size: 211.4 MB (211441335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:16.0.1`

```console
$ docker pull sapmachine@sha256:b837fbb069f6b8ca9e9cd8b69963c10c1be0376e11ed7973bb6587039e3a98c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:16.0.1` - linux; amd64

```console
$ docker pull sapmachine@sha256:7304ad2318d694630e0026c6d05d8de86dc27fc4c7a790dbf7ca9e179e461cbe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.4 MB (248371379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdaebd9d7941ea3546e8c93961ed7aac9b45a2f6301e95e5ab79db6f4e95c0e9`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 11:18:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:18:49 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-16-jdk=16.0.1     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:18:50 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-16
# Fri, 23 Jul 2021 11:18:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a1dc0613013ab06a3796ab75ed46b0ea7cc088afb355824c42ca579549e808`  
		Last Modified: Fri, 23 Jul 2021 11:19:52 GMT  
		Size: 8.3 MB (8321638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c445dbb3177b44abb396b8270ff2cfcb6bcc3748ca4932d0f295ebb8e1495183`  
		Last Modified: Fri, 23 Jul 2021 11:20:01 GMT  
		Size: 211.5 MB (211483878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:latest`

```console
$ docker pull sapmachine@sha256:f0024196c3979f7ab4b898bc13b95d928384c5c10f665884e05944adc93a8591
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:latest` - linux; amd64

```console
$ docker pull sapmachine@sha256:e7262cee5b22868fbbd7f6dbd01b64c5490a81937ece9995aa34f6c24f064af0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.3 MB (248328836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1685b62917509255abeda2436f1ccd581bd601b75485054886fcfacbee25376`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 11:18:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 20:20:41 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-16-jdk=16.0.2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 20:20:42 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-16
# Fri, 23 Jul 2021 20:20:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a1dc0613013ab06a3796ab75ed46b0ea7cc088afb355824c42ca579549e808`  
		Last Modified: Fri, 23 Jul 2021 11:19:52 GMT  
		Size: 8.3 MB (8321638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88652fa7a781f4b350d322eea7bc697551743a37047938903dd158d05d44f72d`  
		Last Modified: Fri, 23 Jul 2021 20:21:17 GMT  
		Size: 211.4 MB (211441335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:lts`

```console
$ docker pull sapmachine@sha256:64f962b59a38601f0dfa722f3e4c0cb84120e19ba129a8ba752a00cac9435d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:lts` - linux; amd64

```console
$ docker pull sapmachine@sha256:3fbe8a57dc9eaddbd537858fe6f63597d30d5930c0cbb1d9f85811f657d035c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235078815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86c7a628e1fafc0ac5324a1abcc3380f3aa74b831368ed7779822a5eeb8eec0a`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:34 GMT
ADD file:5c3d9d2597e01d1cee8513ff0e1344e7791e6f582be2cbd1d5777dd204780f1c in / 
# Tue, 13 Jul 2021 22:29:34 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 11:18:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:19:27 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.12     && rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:19:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Fri, 23 Jul 2021 11:19:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a31c7b29f4ad2bd946738970f040825704a523ded1b9d6f9c7c7cafc6ab731df`  
		Last Modified: Tue, 13 Jul 2021 22:31:20 GMT  
		Size: 28.6 MB (28565863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a1dc0613013ab06a3796ab75ed46b0ea7cc088afb355824c42ca579549e808`  
		Last Modified: Fri, 23 Jul 2021 11:19:52 GMT  
		Size: 8.3 MB (8321638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404dc7bf13ef94ae0b9bc30be2735edc96d5f63e878776351e34cbafa080d4c3`  
		Last Modified: Fri, 23 Jul 2021 11:20:29 GMT  
		Size: 198.2 MB (198191314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
