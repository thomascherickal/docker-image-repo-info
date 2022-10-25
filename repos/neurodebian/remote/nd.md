## `neurodebian:nd`

```console
$ docker pull neurodebian@sha256:1b50fcc2da055bc3dc335b7e4530c158a109378e84c91d8e4a068accafc5dcad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd` - linux; amd64

```console
$ docker pull neurodebian@sha256:640442f8215c858c0ed493030077b99c6f4f565e7db918ef369e28c9d6e2c798
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62440441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3585fe8c53e9d25f64c6ef99ad3fbbfabeba73c7de3aa6e6dc1c839b09770c66`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:41 GMT
ADD file:635f36e1a46e6c28b2a6ab0637cca9e47837c3547b17916d1dbb2595fbeb0821 in / 
# Tue, 25 Oct 2022 01:44:41 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:14:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:14:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 25 Oct 2022 04:14:14 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 25 Oct 2022 04:14:18 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d90f8b044e56f2589b41d1fe9b249b85bde027855731c6f512f0f9401c99e68d`  
		Last Modified: Tue, 25 Oct 2022 01:49:42 GMT  
		Size: 50.6 MB (50641226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940e2a7702be736f2aad5111fec997e5d6fbda3112a52885fe56600b9f20506f`  
		Last Modified: Tue, 25 Oct 2022 04:17:04 GMT  
		Size: 11.5 MB (11517246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90729320165f6559c49f8bc4ce3506f2b3589d4e506fa960c53d2a9f6d25e086`  
		Last Modified: Tue, 25 Oct 2022 04:17:02 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcff98e07edcf843907a8559602876590355c68e7064ab6055f44485f8ddec9c`  
		Last Modified: Tue, 25 Oct 2022 04:17:02 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2861bf0d5d9e8ef934651360c457bda665e3726d7085e6a97345af3a59b1cac2`  
		Last Modified: Tue, 25 Oct 2022 04:17:03 GMT  
		Size: 280.0 KB (279961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:606fe2624ff9d573725a337157db984416d1c306f5902bfb084818a3486d5f5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64331879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcca08c9aa4f00502bf9002fe0c8d93d67c00042c3e9b5de049a083af432b0d4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:47 GMT
ADD file:28797d8b43689eae5ccab5b01e88b732a5fca655590a0c9f066d6f0a4d880a95 in / 
# Tue, 04 Oct 2022 23:45:48 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:41 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:43 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:59:44 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:59:49 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6499ab100dbfb0305e0d96b62f7ad515906275ab30864ac686f0af8ff2fdd114`  
		Last Modified: Tue, 04 Oct 2022 23:52:17 GMT  
		Size: 52.7 MB (52699991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df1adfecab1461b8bd99768350d329ebd6e7b7f5e62880f44688fa052d81ee5`  
		Last Modified: Wed, 05 Oct 2022 04:03:49 GMT  
		Size: 11.5 MB (11532459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211df1c3633aa1661947564b9ed3696aa1124f6f50b0f8f3b5955b1375b7edc9`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae2e7a8e83e699919e6d0b01c2018d0aa2bab3c68163dd11674788e3045521d`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c48121c4388703126d8476e2c0db10a4f0e3fe3b6cf4b0c6c837990718ec487`  
		Last Modified: Wed, 05 Oct 2022 04:03:47 GMT  
		Size: 97.4 KB (97449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd` - linux; 386

```console
$ docker pull neurodebian@sha256:723fcb4319dc470a62adb2c3765720692d48d6ac68a243dbbb4b078135f63508
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.7 MB (65738969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288db7a1ad4289391574ac79c607ffdc110abea480167360cec2bd805154eefd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:40:48 GMT
ADD file:ea6d247c762f6294c87144d1a4308c30669e9e732bd8ff9ef892c71d14563165 in / 
# Tue, 04 Oct 2022 23:40:49 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:16:03 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:16:04 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:16:05 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:16:10 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a0d07a7940ebb4ded014cd2eaedc6b9aa8767ff5afeee7b1b09fce7cbd7a31e`  
		Last Modified: Tue, 04 Oct 2022 23:47:29 GMT  
		Size: 53.6 MB (53647464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155ef37d1ca044b99973bac8a03dd842b017b7e1459194239fd83e9dd188597c`  
		Last Modified: Wed, 05 Oct 2022 02:18:16 GMT  
		Size: 12.0 MB (11992190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a7bb9a78d2d85b84ec9ffbfb13e408d286021108c33addfecf65bcc2993839`  
		Last Modified: Wed, 05 Oct 2022 02:18:14 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994eb0042ba9c275a2f107edab9fd532d71c9a01c5addf5d4966600e9bac59b3`  
		Last Modified: Wed, 05 Oct 2022 02:18:14 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d19a641e13b51478bf8e07a69c870d20f5b6988a813cb8082a4e0636567fa19`  
		Last Modified: Wed, 05 Oct 2022 02:18:15 GMT  
		Size: 97.3 KB (97327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
