## `jobber:1-alpine3.11`

```console
$ docker pull jobber@sha256:652facc4ce8aa8669bc36de8a996361a34188e2a0b307d1d3be69e4963d41b26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jobber:1-alpine3.11` - linux; amd64

```console
$ docker pull jobber@sha256:a85b68725beeb738e5d6e0f029dd01c4e0dd793aa4f1bfdf70c8d5f37586c3d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.8 MB (11764588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3b2ec9cd879ec4ae942b88182cbeb7fa419a9511a19a5bd85e09d7f8db12399`
-	Default Command: `["\/usr\/libexec\/jobberrunner","-u","\/var\/jobber\/1000\/cmd.sock","\/home\/jobberuser\/.jobber"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 03:01:40 GMT
ENV USERID=1000
# Wed, 01 Sep 2021 03:01:41 GMT
RUN addgroup jobberuser &&     adduser -S -u "${USERID}" -G jobberuser jobberuser &&     mkdir -p "/var/jobber/${USERID}" &&     chown -R jobberuser:jobberuser "/var/jobber/${USERID}"
# Wed, 01 Sep 2021 03:01:41 GMT
ENV JOBBER_VERSION=1.4.4
# Wed, 01 Sep 2021 03:01:41 GMT
ENV JOBBER_SHA256=ec09b2efafff69c91fba2124bf28607209e1c9b50ed834ff444a9d40798aa8d3
# Wed, 01 Sep 2021 03:01:44 GMT
RUN wget -O /tmp/jobber.apk "https://github.com/dshearer/jobber/releases/download/v${JOBBER_VERSION}/jobber-${JOBBER_VERSION}-r0.apk" &&     echo -n "Actual checksum: " && sha256sum /tmp/jobber.apk &&     echo "${JOBBER_SHA256} */tmp/jobber.apk" | sha256sum -c &&     apk add --no-network --no-scripts --allow-untrusted /tmp/jobber.apk &&     rm /tmp/jobber.apk
# Wed, 01 Sep 2021 03:01:44 GMT
COPY --chown=jobberuser:jobberuserfile:c7cc6d32091e7beeac78efd9fe855e36a106902c1177df0f9f6bd2bbe3b8d518 in /home/jobberuser/.jobber 
# Wed, 01 Sep 2021 03:01:45 GMT
RUN chmod 0600 /home/jobberuser/.jobber
# Wed, 01 Sep 2021 03:01:45 GMT
USER jobberuser
# Wed, 01 Sep 2021 03:01:45 GMT
CMD ["/usr/libexec/jobberrunner" "-u" "/var/jobber/1000/cmd.sock" "/home/jobberuser/.jobber"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1b18101a627546b309d6a77a34d11d10d56ee14cdc85cf55cf5a80f62f5e23`  
		Last Modified: Wed, 01 Sep 2021 03:01:58 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef49d20280992e72362712a5ff6c391e93f34f4f964ee2983faabfa483f3e23`  
		Last Modified: Wed, 01 Sep 2021 03:02:00 GMT  
		Size: 8.9 MB (8945478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64a0c34a429abee6adf286228377fc0372842ea2c7cae950aa2f8f996a90dc7`  
		Last Modified: Wed, 01 Sep 2021 03:01:58 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e02ab2b1ad1a03911aed21418751e378016df9ead2e86f3acd38eed82bda4d`  
		Last Modified: Wed, 01 Sep 2021 03:01:58 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
