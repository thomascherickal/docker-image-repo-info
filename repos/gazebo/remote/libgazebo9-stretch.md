## `gazebo:libgazebo9-stretch`

```console
$ docker pull gazebo@sha256:8394931ebc7d517364cfc400e781839d996b6bd1f2cc2c0d190d66c545ce2e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `gazebo:libgazebo9-stretch` - linux; amd64

```console
$ docker pull gazebo@sha256:6ab806c808d04a2ad4e4dbe75448e9a1ce0ddd7a4f0310271760e3aa1f7b03a3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **650.8 MB (650834823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d32bd16fa48b4cc61cdfa75252153e73b3fb2e94b3642732457a95f9268d5e3b`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 23:03:23 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:03:28 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Sat, 28 Dec 2019 23:03:29 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Sat, 28 Dec 2019 23:04:54 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.11.0-1*     && rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:04:55 GMT
EXPOSE 11345
# Sat, 28 Dec 2019 23:04:55 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Sat, 28 Dec 2019 23:04:55 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Sat, 28 Dec 2019 23:04:55 GMT
CMD ["gzserver"]
# Sat, 28 Dec 2019 23:07:12 GMT
RUN apt-get update && apt-get install -q -y     libgazebo9-dev=9.11.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ac4b056aa820ccd62eba13490f254fd2e5fd1d5e68d8bc240ec736625ec10c`  
		Last Modified: Sat, 28 Dec 2019 23:07:40 GMT  
		Size: 21.1 MB (21095092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcce2b2d1a628def73ccf25e5786422ad365c4a1e1d466eb1df101e16ef3057`  
		Last Modified: Sat, 28 Dec 2019 23:07:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7f6cb2c41a33535075235f2c5b1c881e2a427eae3a402e1f0baa3b6e5c107a`  
		Last Modified: Sat, 28 Dec 2019 23:07:33 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d8dfadfb93faf6007fb99a0c7d8d84085180a82fccce9a0d5f843a07327fa1`  
		Last Modified: Sat, 28 Dec 2019 23:08:20 GMT  
		Size: 279.8 MB (279814536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7e93ebcbeae6a3de80f68c9fda93dfb1476ef85954003844581d131b032e6d`  
		Last Modified: Sat, 28 Dec 2019 23:07:33 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748952a86dd3c51462e9d48435ff13cc579cd9ce492606b2b6c95cc00d85c2ff`  
		Last Modified: Sat, 28 Dec 2019 23:09:19 GMT  
		Size: 304.5 MB (304537859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gazebo:libgazebo9-stretch` - linux; arm variant v7

```console
$ docker pull gazebo@sha256:04b3753304246f70cc88af8290a473307f66a2f9235852d5439669e2acbd4df4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **597.0 MB (597006834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c38601e34e9c605b78f697cb46ca4c405841fdbe82be6c3d6b338ad99d7166b`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Tue, 05 Mar 2019 13:10:34 GMT
ADD file:8f0ec0cbcef5902fe5ef35892898a19e6c61f5c422ac3d47500d42067ad7fef8 in / 
# Tue, 05 Mar 2019 13:10:35 GMT
CMD ["bash"]
# Tue, 05 Mar 2019 14:12:08 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Tue, 05 Mar 2019 14:12:15 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Tue, 05 Mar 2019 14:12:18 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Thu, 21 Mar 2019 12:09:48 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.7.0-1*     && rm -rf /var/lib/apt/lists/*
# Thu, 21 Mar 2019 12:09:50 GMT
EXPOSE 11345
# Thu, 21 Mar 2019 12:09:51 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Thu, 21 Mar 2019 12:09:51 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Thu, 21 Mar 2019 12:09:52 GMT
CMD ["gzserver"]
# Thu, 21 Mar 2019 12:12:19 GMT
RUN apt-get update && apt-get install -q -y     libgazebo9-dev=9.7.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec43a77fdcf3d8df75738e0d3bec016f01ad00db637d5e43eee90aa67114e127`  
		Last Modified: Tue, 05 Mar 2019 13:18:22 GMT  
		Size: 42.1 MB (42075119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfe1620eae9a31d468d937705028145d4e4ad40bd8d7a96371ef05a4d641cae`  
		Last Modified: Tue, 05 Mar 2019 14:18:24 GMT  
		Size: 19.6 MB (19554481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c8188618c43dcd54081bab8020535bae67c8586f49708c5cafb387f7ece6f8`  
		Last Modified: Tue, 05 Mar 2019 14:18:18 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45d93c9607ceb050dbe8b027bbed7e2a14180e03b9228264955d6e457050717`  
		Last Modified: Tue, 05 Mar 2019 14:18:18 GMT  
		Size: 5.0 KB (5010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568ecf381553d118776fdf569e7571e9f665d50083029bc33c6be48a816074e6`  
		Last Modified: Thu, 21 Mar 2019 12:16:18 GMT  
		Size: 258.0 MB (257971594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893ae20c267a4e16e4ee94df1a0c88156479f44c69e89a015dc30f9193fd5c99`  
		Last Modified: Thu, 21 Mar 2019 12:15:17 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29bfd6ff3786a41b1a44b3161df36ad64e4d4e2af3d5ffa78167679a8e330d1`  
		Last Modified: Thu, 21 Mar 2019 12:17:46 GMT  
		Size: 277.4 MB (277399022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gazebo:libgazebo9-stretch` - linux; arm64 variant v8

```console
$ docker pull gazebo@sha256:e0950cb00cba5da8820742d2d8e95ab26ce191ce267ef94b37fa0ece218d80c0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.8 MB (584801517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8c6f9002a0c8a6556ee7449e6b9632fe0f3b5b87077c54b4aed38a8b0b5dde5`
-	Entrypoint: `["\/gzserver_entrypoint.sh"]`
-	Default Command: `["gzserver"]`

```dockerfile
# Wed, 14 Aug 2019 00:42:54 GMT
ADD file:705744f1d46153f7b1e4e803e92a622e76091e0c7812e893ccadf4c3fa3f7582 in / 
# Wed, 14 Aug 2019 00:42:55 GMT
CMD ["bash"]
# Wed, 14 Aug 2019 08:53:07 GMT
RUN apt-get update && apt-get install -q -y     dirmngr     gnupg2     lsb-release     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Aug 2019 08:53:13 GMT
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys D2486D2DD83DB69272AFE98867170598AF249743
# Wed, 14 Aug 2019 08:53:16 GMT
RUN . /etc/os-release     && echo "deb http://packages.osrfoundation.org/gazebo/$ID-stable `lsb_release -sc` main" > /etc/apt/sources.list.d/gazebo-latest.list
# Wed, 14 Aug 2019 08:55:30 GMT
RUN apt-get update && apt-get install -q -y     gazebo9=9.10.0-1*     && rm -rf /var/lib/apt/lists/*
# Wed, 14 Aug 2019 08:55:32 GMT
EXPOSE 11345
# Wed, 14 Aug 2019 08:55:32 GMT
COPY file:b79966dec12c55a0a5c9e673326cc3faf9cbbeee0ea5f172e863df237eb8a601 in / 
# Wed, 14 Aug 2019 08:55:33 GMT
ENTRYPOINT ["/gzserver_entrypoint.sh"]
# Wed, 14 Aug 2019 08:55:33 GMT
CMD ["gzserver"]
# Wed, 14 Aug 2019 08:57:48 GMT
RUN apt-get update && apt-get install -q -y     libgazebo9-dev=9.10.0-1*     && rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c9a9b339897414ebcb758c313024f2e0cdd97ccd184a2db5d2fd418c3c37bf86`  
		Last Modified: Wed, 14 Aug 2019 00:48:21 GMT  
		Size: 43.1 MB (43140037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d733261cac3051c6baca2448f9a29eeef65e2a539d23fb345be8220a682a4cb4`  
		Last Modified: Wed, 14 Aug 2019 08:58:23 GMT  
		Size: 19.7 MB (19747558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f293efbaccfb8dadbd8b27d9c5a31a573500623e58abdb4cc098e9d87fb16c`  
		Last Modified: Wed, 14 Aug 2019 08:58:16 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c5414a2c84314aa4b6317415f4c53154e571fab2de3900cda5a9d5aa19216d`  
		Last Modified: Wed, 14 Aug 2019 08:58:16 GMT  
		Size: 5.0 KB (5011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d77fbd4200a6bfa5b351cc6d2adddc9a177581cc40705ac0f3a6385f219e567`  
		Last Modified: Wed, 14 Aug 2019 08:59:23 GMT  
		Size: 265.9 MB (265875457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1451ce0fadc30d693037b2243839842580d6a804139c175adbfa38e69b6444`  
		Last Modified: Wed, 14 Aug 2019 08:58:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0e8278ca009363f937adaa396c6a951da4b63183931223a87f14f0bfb23570`  
		Last Modified: Wed, 14 Aug 2019 09:00:44 GMT  
		Size: 256.0 MB (256031845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
