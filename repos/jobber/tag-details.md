<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `jobber`

-	[`jobber:1-alpine3.11`](#jobber1-alpine311)
-	[`jobber:1.4-alpine3.11`](#jobber14-alpine311)
-	[`jobber:1.4.4-alpine3.11`](#jobber144-alpine311)
-	[`jobber:latest`](#jobberlatest)

## `jobber:1-alpine3.11`

```console
$ docker pull jobber@sha256:a957797e817d2ef8a0688733fa3cf2bcf601a5c22a71a3f078ea7a553ec393bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jobber:1-alpine3.11` - linux; amd64

```console
$ docker pull jobber@sha256:dfd3762dd5d545a00200bb2b44e87e239303a7b161e7ac6c81b89545e8277399
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.8 MB (11762458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ba67f47e556428b352ce161dfae34f560a7c459f68d866501abfccc5948346`
-	Default Command: `["\/usr\/libexec\/jobberrunner","-u","\/var\/jobber\/1000\/cmd.sock","\/home\/jobberuser\/.jobber"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:52:33 GMT
ENV USERID=1000
# Wed, 24 Feb 2021 23:52:35 GMT
RUN addgroup jobberuser &&     adduser -S -u "${USERID}" -G jobberuser jobberuser &&     mkdir -p "/var/jobber/${USERID}" &&     chown -R jobberuser:jobberuser "/var/jobber/${USERID}"
# Wed, 24 Feb 2021 23:52:35 GMT
ENV JOBBER_VERSION=1.4.4
# Wed, 24 Feb 2021 23:52:36 GMT
ENV JOBBER_SHA256=ec09b2efafff69c91fba2124bf28607209e1c9b50ed834ff444a9d40798aa8d3
# Wed, 24 Feb 2021 23:52:39 GMT
RUN wget -O /tmp/jobber.apk "https://github.com/dshearer/jobber/releases/download/v${JOBBER_VERSION}/jobber-${JOBBER_VERSION}-r0.apk" &&     echo -n "Actual checksum: " && sha256sum /tmp/jobber.apk &&     echo "${JOBBER_SHA256} */tmp/jobber.apk" | sha256sum -c &&     apk add --no-network --no-scripts --allow-untrusted /tmp/jobber.apk &&     rm /tmp/jobber.apk
# Wed, 24 Feb 2021 23:52:40 GMT
COPY --chown=jobberuser:jobberuserfile:c7cc6d32091e7beeac78efd9fe855e36a106902c1177df0f9f6bd2bbe3b8d518 in /home/jobberuser/.jobber 
# Wed, 24 Feb 2021 23:52:41 GMT
RUN chmod 0600 /home/jobberuser/.jobber
# Wed, 24 Feb 2021 23:52:42 GMT
USER jobberuser
# Wed, 24 Feb 2021 23:52:42 GMT
CMD ["/usr/libexec/jobberrunner" "-u" "/var/jobber/1000/cmd.sock" "/home/jobberuser/.jobber"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3d77e4a1d72bdd947ca59dbc0abb4d358aff819d1fb88c8867099bbc2ac861`  
		Last Modified: Wed, 24 Feb 2021 23:52:55 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafd70afc509a0674d1dcba80225eb35b43aedb620b4eafb8d81029fd3956efe`  
		Last Modified: Wed, 24 Feb 2021 23:53:02 GMT  
		Size: 8.9 MB (8945400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a9fb249707d3c6023c95de3a73fb2a6015568af62da4857f4842c07551cf8`  
		Last Modified: Wed, 24 Feb 2021 23:52:55 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81d6c18305351cbee407843bef85f557af41f52283dcf4223401ea359d126e1`  
		Last Modified: Wed, 24 Feb 2021 23:52:55 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jobber:1.4-alpine3.11`

```console
$ docker pull jobber@sha256:a957797e817d2ef8a0688733fa3cf2bcf601a5c22a71a3f078ea7a553ec393bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jobber:1.4-alpine3.11` - linux; amd64

```console
$ docker pull jobber@sha256:dfd3762dd5d545a00200bb2b44e87e239303a7b161e7ac6c81b89545e8277399
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.8 MB (11762458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ba67f47e556428b352ce161dfae34f560a7c459f68d866501abfccc5948346`
-	Default Command: `["\/usr\/libexec\/jobberrunner","-u","\/var\/jobber\/1000\/cmd.sock","\/home\/jobberuser\/.jobber"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:52:33 GMT
ENV USERID=1000
# Wed, 24 Feb 2021 23:52:35 GMT
RUN addgroup jobberuser &&     adduser -S -u "${USERID}" -G jobberuser jobberuser &&     mkdir -p "/var/jobber/${USERID}" &&     chown -R jobberuser:jobberuser "/var/jobber/${USERID}"
# Wed, 24 Feb 2021 23:52:35 GMT
ENV JOBBER_VERSION=1.4.4
# Wed, 24 Feb 2021 23:52:36 GMT
ENV JOBBER_SHA256=ec09b2efafff69c91fba2124bf28607209e1c9b50ed834ff444a9d40798aa8d3
# Wed, 24 Feb 2021 23:52:39 GMT
RUN wget -O /tmp/jobber.apk "https://github.com/dshearer/jobber/releases/download/v${JOBBER_VERSION}/jobber-${JOBBER_VERSION}-r0.apk" &&     echo -n "Actual checksum: " && sha256sum /tmp/jobber.apk &&     echo "${JOBBER_SHA256} */tmp/jobber.apk" | sha256sum -c &&     apk add --no-network --no-scripts --allow-untrusted /tmp/jobber.apk &&     rm /tmp/jobber.apk
# Wed, 24 Feb 2021 23:52:40 GMT
COPY --chown=jobberuser:jobberuserfile:c7cc6d32091e7beeac78efd9fe855e36a106902c1177df0f9f6bd2bbe3b8d518 in /home/jobberuser/.jobber 
# Wed, 24 Feb 2021 23:52:41 GMT
RUN chmod 0600 /home/jobberuser/.jobber
# Wed, 24 Feb 2021 23:52:42 GMT
USER jobberuser
# Wed, 24 Feb 2021 23:52:42 GMT
CMD ["/usr/libexec/jobberrunner" "-u" "/var/jobber/1000/cmd.sock" "/home/jobberuser/.jobber"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3d77e4a1d72bdd947ca59dbc0abb4d358aff819d1fb88c8867099bbc2ac861`  
		Last Modified: Wed, 24 Feb 2021 23:52:55 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafd70afc509a0674d1dcba80225eb35b43aedb620b4eafb8d81029fd3956efe`  
		Last Modified: Wed, 24 Feb 2021 23:53:02 GMT  
		Size: 8.9 MB (8945400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a9fb249707d3c6023c95de3a73fb2a6015568af62da4857f4842c07551cf8`  
		Last Modified: Wed, 24 Feb 2021 23:52:55 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81d6c18305351cbee407843bef85f557af41f52283dcf4223401ea359d126e1`  
		Last Modified: Wed, 24 Feb 2021 23:52:55 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jobber:1.4.4-alpine3.11`

```console
$ docker pull jobber@sha256:a957797e817d2ef8a0688733fa3cf2bcf601a5c22a71a3f078ea7a553ec393bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jobber:1.4.4-alpine3.11` - linux; amd64

```console
$ docker pull jobber@sha256:dfd3762dd5d545a00200bb2b44e87e239303a7b161e7ac6c81b89545e8277399
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.8 MB (11762458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ba67f47e556428b352ce161dfae34f560a7c459f68d866501abfccc5948346`
-	Default Command: `["\/usr\/libexec\/jobberrunner","-u","\/var\/jobber\/1000\/cmd.sock","\/home\/jobberuser\/.jobber"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:52:33 GMT
ENV USERID=1000
# Wed, 24 Feb 2021 23:52:35 GMT
RUN addgroup jobberuser &&     adduser -S -u "${USERID}" -G jobberuser jobberuser &&     mkdir -p "/var/jobber/${USERID}" &&     chown -R jobberuser:jobberuser "/var/jobber/${USERID}"
# Wed, 24 Feb 2021 23:52:35 GMT
ENV JOBBER_VERSION=1.4.4
# Wed, 24 Feb 2021 23:52:36 GMT
ENV JOBBER_SHA256=ec09b2efafff69c91fba2124bf28607209e1c9b50ed834ff444a9d40798aa8d3
# Wed, 24 Feb 2021 23:52:39 GMT
RUN wget -O /tmp/jobber.apk "https://github.com/dshearer/jobber/releases/download/v${JOBBER_VERSION}/jobber-${JOBBER_VERSION}-r0.apk" &&     echo -n "Actual checksum: " && sha256sum /tmp/jobber.apk &&     echo "${JOBBER_SHA256} */tmp/jobber.apk" | sha256sum -c &&     apk add --no-network --no-scripts --allow-untrusted /tmp/jobber.apk &&     rm /tmp/jobber.apk
# Wed, 24 Feb 2021 23:52:40 GMT
COPY --chown=jobberuser:jobberuserfile:c7cc6d32091e7beeac78efd9fe855e36a106902c1177df0f9f6bd2bbe3b8d518 in /home/jobberuser/.jobber 
# Wed, 24 Feb 2021 23:52:41 GMT
RUN chmod 0600 /home/jobberuser/.jobber
# Wed, 24 Feb 2021 23:52:42 GMT
USER jobberuser
# Wed, 24 Feb 2021 23:52:42 GMT
CMD ["/usr/libexec/jobberrunner" "-u" "/var/jobber/1000/cmd.sock" "/home/jobberuser/.jobber"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3d77e4a1d72bdd947ca59dbc0abb4d358aff819d1fb88c8867099bbc2ac861`  
		Last Modified: Wed, 24 Feb 2021 23:52:55 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafd70afc509a0674d1dcba80225eb35b43aedb620b4eafb8d81029fd3956efe`  
		Last Modified: Wed, 24 Feb 2021 23:53:02 GMT  
		Size: 8.9 MB (8945400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a9fb249707d3c6023c95de3a73fb2a6015568af62da4857f4842c07551cf8`  
		Last Modified: Wed, 24 Feb 2021 23:52:55 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81d6c18305351cbee407843bef85f557af41f52283dcf4223401ea359d126e1`  
		Last Modified: Wed, 24 Feb 2021 23:52:55 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `jobber:latest`

```console
$ docker pull jobber@sha256:a957797e817d2ef8a0688733fa3cf2bcf601a5c22a71a3f078ea7a553ec393bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jobber:latest` - linux; amd64

```console
$ docker pull jobber@sha256:dfd3762dd5d545a00200bb2b44e87e239303a7b161e7ac6c81b89545e8277399
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.8 MB (11762458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ba67f47e556428b352ce161dfae34f560a7c459f68d866501abfccc5948346`
-	Default Command: `["\/usr\/libexec\/jobberrunner","-u","\/var\/jobber\/1000\/cmd.sock","\/home\/jobberuser\/.jobber"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:11 GMT
ADD file:7eeea546ecde7a036bf634c08719879d32c7ec6ae599708cd91dc1b830735223 in / 
# Wed, 24 Feb 2021 20:20:12 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:52:33 GMT
ENV USERID=1000
# Wed, 24 Feb 2021 23:52:35 GMT
RUN addgroup jobberuser &&     adduser -S -u "${USERID}" -G jobberuser jobberuser &&     mkdir -p "/var/jobber/${USERID}" &&     chown -R jobberuser:jobberuser "/var/jobber/${USERID}"
# Wed, 24 Feb 2021 23:52:35 GMT
ENV JOBBER_VERSION=1.4.4
# Wed, 24 Feb 2021 23:52:36 GMT
ENV JOBBER_SHA256=ec09b2efafff69c91fba2124bf28607209e1c9b50ed834ff444a9d40798aa8d3
# Wed, 24 Feb 2021 23:52:39 GMT
RUN wget -O /tmp/jobber.apk "https://github.com/dshearer/jobber/releases/download/v${JOBBER_VERSION}/jobber-${JOBBER_VERSION}-r0.apk" &&     echo -n "Actual checksum: " && sha256sum /tmp/jobber.apk &&     echo "${JOBBER_SHA256} */tmp/jobber.apk" | sha256sum -c &&     apk add --no-network --no-scripts --allow-untrusted /tmp/jobber.apk &&     rm /tmp/jobber.apk
# Wed, 24 Feb 2021 23:52:40 GMT
COPY --chown=jobberuser:jobberuserfile:c7cc6d32091e7beeac78efd9fe855e36a106902c1177df0f9f6bd2bbe3b8d518 in /home/jobberuser/.jobber 
# Wed, 24 Feb 2021 23:52:41 GMT
RUN chmod 0600 /home/jobberuser/.jobber
# Wed, 24 Feb 2021 23:52:42 GMT
USER jobberuser
# Wed, 24 Feb 2021 23:52:42 GMT
CMD ["/usr/libexec/jobberrunner" "-u" "/var/jobber/1000/cmd.sock" "/home/jobberuser/.jobber"]
```

-	Layers:
	-	`sha256:e95f33c60a645d6d31f52fdc334aecec0d79a1b410789eae37fbf69efcd587ab`  
		Last Modified: Wed, 24 Feb 2021 20:20:43 GMT  
		Size: 2.8 MB (2815313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3d77e4a1d72bdd947ca59dbc0abb4d358aff819d1fb88c8867099bbc2ac861`  
		Last Modified: Wed, 24 Feb 2021 23:52:55 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafd70afc509a0674d1dcba80225eb35b43aedb620b4eafb8d81029fd3956efe`  
		Last Modified: Wed, 24 Feb 2021 23:53:02 GMT  
		Size: 8.9 MB (8945400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8a9fb249707d3c6023c95de3a73fb2a6015568af62da4857f4842c07551cf8`  
		Last Modified: Wed, 24 Feb 2021 23:52:55 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81d6c18305351cbee407843bef85f557af41f52283dcf4223401ea359d126e1`  
		Last Modified: Wed, 24 Feb 2021 23:52:55 GMT  
		Size: 233.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
