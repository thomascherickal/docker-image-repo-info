## `jobber:1-alpine3.11`

```console
$ docker pull jobber@sha256:10e354645c84f98fcb5b3a49b578e47d3ad16406e94d763e6e1784397fef208c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `jobber:1-alpine3.11` - linux; amd64

```console
$ docker pull jobber@sha256:e56fb65be9c98aaea8ba176013070a04454ea9b4cfdf37b3d9c1f4c443856225
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.8 MB (11763540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcc145fe02efced5fe3e93495514f757ea3add298b6b175332db4a7eb771c5cb`
-	Default Command: `["\/usr\/libexec\/jobberrunner","-u","\/var\/jobber\/1000\/cmd.sock","\/home\/jobberuser\/.jobber"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:04:43 GMT
ENV USERID=1000
# Wed, 14 Apr 2021 23:04:43 GMT
RUN addgroup jobberuser &&     adduser -S -u "${USERID}" -G jobberuser jobberuser &&     mkdir -p "/var/jobber/${USERID}" &&     chown -R jobberuser:jobberuser "/var/jobber/${USERID}"
# Wed, 14 Apr 2021 23:04:44 GMT
ENV JOBBER_VERSION=1.4.4
# Wed, 14 Apr 2021 23:04:44 GMT
ENV JOBBER_SHA256=ec09b2efafff69c91fba2124bf28607209e1c9b50ed834ff444a9d40798aa8d3
# Wed, 14 Apr 2021 23:04:46 GMT
RUN wget -O /tmp/jobber.apk "https://github.com/dshearer/jobber/releases/download/v${JOBBER_VERSION}/jobber-${JOBBER_VERSION}-r0.apk" &&     echo -n "Actual checksum: " && sha256sum /tmp/jobber.apk &&     echo "${JOBBER_SHA256} */tmp/jobber.apk" | sha256sum -c &&     apk add --no-network --no-scripts --allow-untrusted /tmp/jobber.apk &&     rm /tmp/jobber.apk
# Wed, 14 Apr 2021 23:04:46 GMT
COPY --chown=jobberuser:jobberuserfile:c7cc6d32091e7beeac78efd9fe855e36a106902c1177df0f9f6bd2bbe3b8d518 in /home/jobberuser/.jobber 
# Wed, 14 Apr 2021 23:04:47 GMT
RUN chmod 0600 /home/jobberuser/.jobber
# Wed, 14 Apr 2021 23:04:48 GMT
USER jobberuser
# Wed, 14 Apr 2021 23:04:48 GMT
CMD ["/usr/libexec/jobberrunner" "-u" "/var/jobber/1000/cmd.sock" "/home/jobberuser/.jobber"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18ff9579323ca8e04b1ef714c48bdfda3894af6fa8481348c02a33705ca2043`  
		Last Modified: Wed, 14 Apr 2021 23:04:59 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e3e95b0587c34fd777ff5f1571b7eb8091b36aa07204e2a2284d4d42cac77c`  
		Last Modified: Wed, 14 Apr 2021 23:05:02 GMT  
		Size: 8.9 MB (8945498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0975ac2a91ef4e18488a96d3b2bd12c7de0e1fcc1d23e5b30257b029ac2a11f`  
		Last Modified: Wed, 14 Apr 2021 23:04:59 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33736413733e9ebe8edd9eae0168f712bb8993dcd7573a8687ace99050c47b1`  
		Last Modified: Wed, 14 Apr 2021 23:04:59 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
