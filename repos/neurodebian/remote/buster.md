## `neurodebian:buster`

```console
$ docker pull neurodebian@sha256:ab17dbb4dd558ead3bf4096c557b81d6f621a2f5a4e1dc6ec9209df228b390e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster` - linux; amd64

```console
$ docker pull neurodebian@sha256:b37bef120004b4687aa2022d3e155b055d61beb954c12289995048a9e6b194c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61258410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75d2a173dfd73416762a6dfb63b7015b802fadac902b73b3f7cae9de6c78e3aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:02 GMT
ADD file:259be79d94a2549a667ad08a093fe18f15a6c93d66a0723292f49294e31fc7a1 in / 
# Tue, 25 Oct 2022 01:44:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:13:07 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:13:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 25 Oct 2022 04:13:09 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 25 Oct 2022 04:13:14 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fd31ec14dccdcda8f2472547f1a94ef0a23b8dabb764cd7b1d48aeee0afea7c8`  
		Last Modified: Tue, 25 Oct 2022 01:48:15 GMT  
		Size: 50.4 MB (50447742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9122ec6aa2a6194ca00862c6d9350bc5b3a8b530dfdf48dd3973cac441ddb49f`  
		Last Modified: Tue, 25 Oct 2022 04:15:59 GMT  
		Size: 10.5 MB (10504344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4c20cf0b981052b23457bc1f8457f68bd7515cad276917ba46fb57144c755d`  
		Last Modified: Tue, 25 Oct 2022 04:15:58 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb9a440939dfe96a44b07dfa89426581578c53b5e5d02c8b8b02b74d3fc9305`  
		Last Modified: Tue, 25 Oct 2022 04:15:58 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879b3b855360c632fcecd2c95dd76c57425ff8bb0dc3e9d94794896068a07ebf`  
		Last Modified: Tue, 25 Oct 2022 04:15:59 GMT  
		Size: 304.3 KB (304315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:2dc6d3c83993dc6a49fc286f9a1d6110258197edb1d3cacabec8b12d88d4becf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59636797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b50a8e93e8303cee10538cc56493e6e180c31a069561b078b566065bc62aca2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:28 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d154496b8ab72771340bbbfcb90129abefba06a0df134e694e436c32723ecf`  
		Last Modified: Wed, 05 Oct 2022 04:02:31 GMT  
		Size: 10.3 MB (10297436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef89a9a6d8113e10f9e579ee92783e306a5fa8bfe2acfa01e2d78d7fd818107f`  
		Last Modified: Wed, 05 Oct 2022 04:02:29 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23704a18d02fdbc4131c6f7adfaaec3730093c5504d02a143c4a78f637028721`  
		Last Modified: Wed, 05 Oct 2022 04:02:29 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d322400769bb470d58b21b11c9f6e84fb73d5e8603c40127b4804943ec7f7ec2`  
		Last Modified: Wed, 05 Oct 2022 04:02:30 GMT  
		Size: 108.5 KB (108492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster` - linux; 386

```console
$ docker pull neurodebian@sha256:1fd4cf8b2a55d0059c7adddd50e16ea9c0b91e97458079defd08db84607e50a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61982452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4611172bd93ea6abd33eb27f96eeb688a884c754e831b30d565524925f180742`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:52 GMT
ADD file:887aa5460e148ba204780ebe976e5627d5f4d0a07faf22b86afe146998d75d79 in / 
# Tue, 04 Oct 2022 23:39:53 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 02:14:43 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 02:14:44 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 02:14:45 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 02:14:50 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:98d78922e3457a6697f2cdbddaab27dbb47e2e0beedb1a4348c56102c850b343`  
		Last Modified: Tue, 04 Oct 2022 23:45:58 GMT  
		Size: 51.2 MB (51202841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53a1c4ae5a735b6da355e52d679127188fc0385520109eb7c93e31b0fd3a7c5`  
		Last Modified: Wed, 05 Oct 2022 02:17:01 GMT  
		Size: 10.7 MB (10669155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127af1b441210177fdedbe41dc0aaf6ca644be580c15ae7a5cae51e8ff1bffce`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8999f6b03a0580644ff4a8ada4dec6b0d39eec0f624022a1b96f832f8fd28a21`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5c07173b4dcb13dbcc2b4c04cdbb7546fb67e2b14f21eea7653356ac3845ba`  
		Last Modified: Wed, 05 Oct 2022 02:16:59 GMT  
		Size: 108.5 KB (108467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
