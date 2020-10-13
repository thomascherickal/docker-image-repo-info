## `neurodebian:stretch`

```console
$ docker pull neurodebian@sha256:cb18cfae42efa61e114123a48b692d073f8a73bb7d4a61e36cec23e5f96834ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:stretch` - linux; amd64

```console
$ docker pull neurodebian@sha256:2122a92e6f9db6735f2d6b77744beb5bf2eeb6ed1bc7121376c010b8b2365c76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52230876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4c2d925acffff35159192efde248df47c85fdc394ef03fbafdbe30b73b574aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:13 GMT
ADD file:a8742c34bf12f231279dd5086b8ec1310224c740a95170b916217f22a68eb9a7 in / 
# Tue, 13 Oct 2020 01:44:13 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:35:46 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:35:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 13 Oct 2020 08:35:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian stretch main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel stretch main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 13 Oct 2020 08:35:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0400ac8f7460260a663e0e97c24d7dfd8a2c947736f0351752b45c53e26d6e02`  
		Last Modified: Tue, 13 Oct 2020 01:50:49 GMT  
		Size: 45.4 MB (45366778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00743937e1768506aa3ccb846018c79fbc33adc6836bb6f31122f08f6ec4dd62`  
		Last Modified: Tue, 13 Oct 2020 08:37:58 GMT  
		Size: 6.6 MB (6568564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf84959b28386abb4853d0f2add545e0167b0a09a997c9c824e57c8cb277562`  
		Last Modified: Tue, 13 Oct 2020 08:37:56 GMT  
		Size: 3.2 KB (3151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fdc55d937a17f2279263e89b40c81159375b03dadb986bba18e9160ef6be24`  
		Last Modified: Tue, 13 Oct 2020 08:37:56 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86186a7959e2fb76a2976b2295b15a5074d31852be81ce5b3662b738491b3bbc`  
		Last Modified: Tue, 13 Oct 2020 08:37:56 GMT  
		Size: 292.1 KB (292139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
