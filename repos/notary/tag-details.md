<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `notary`

-	[`notary:server`](#notaryserver)
-	[`notary:server-0.7.0`](#notaryserver-070)
-	[`notary:signer`](#notarysigner)
-	[`notary:signer-0.7.0`](#notarysigner-070)

## `notary:server`

```console
$ docker pull notary@sha256:6ce6beac8cd9033b153438e2d9ed88087671eb7f868691ca8be790a640618c47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:server` - linux; amd64

```console
$ docker pull notary@sha256:725646c4d072977023698a3c1b25fc68862ed1646e26b7f8ae60ad7c2549a59e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e9925dcb4c27e30de0f81ce854368e4f7c8246d84b40e220ca2aa581b356543`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 01:52:21 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 01:52:21 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 25 Oct 2022 01:52:21 GMT
ENV INSTALLDIR=/notary/server
# Tue, 25 Oct 2022 01:52:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 25 Oct 2022 01:52:21 GMT
WORKDIR /notary/server
# Tue, 01 Nov 2022 19:49:00 GMT
COPY /notary-server ./ # buildkit
# Tue, 01 Nov 2022 19:49:00 GMT
RUN ./notary-server --version # buildkit
# Tue, 01 Nov 2022 19:49:00 GMT
COPY ./server-config.json . # buildkit
# Tue, 01 Nov 2022 19:49:00 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 01 Nov 2022 19:49:00 GMT
USER notary
# Tue, 01 Nov 2022 19:49:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 01 Nov 2022 19:49:00 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae0db85ee62912972b015b43b47b5849f5b66900a08ad146a42f7c16d02def`  
		Last Modified: Tue, 25 Oct 2022 01:53:00 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae714b9c46c68b869025bf262b5afec2bb7f99f3739cdae14e11604248f87fd`  
		Last Modified: Tue, 25 Oct 2022 01:52:58 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288b5f0093c5cb556b6e816cc8c65e59ea4a3be57cd8c9cfbab00dbe5bcdb49c`  
		Last Modified: Tue, 01 Nov 2022 19:49:21 GMT  
		Size: 5.1 MB (5143673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca8a52dd6617ccfc327338630a16dcd2ef53f59ec3014397fd87e6ace50c555`  
		Last Modified: Tue, 01 Nov 2022 19:49:20 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5a71241ee3d85608914a3d2c7779ce29252304f4225ad71dcfe3c1b046f3a2`  
		Last Modified: Tue, 01 Nov 2022 19:49:20 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c863d998853c7cbc0e52dbf21a83074cbc3f2acc5cec1f9cb7992d95cffe7e`  
		Last Modified: Tue, 01 Nov 2022 19:49:20 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm variant v6

```console
$ docker pull notary@sha256:b1009bcad7b6a49141436b4fd03fd73ae2b58547f836123cf4b4fd0d0aedbb1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7505595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54ecccd1c21b9543ad2c0070218ddb0a2bf3d250d3d0daa529a10a5e5f9cce54`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:53:33 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:53:33 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 12 Nov 2022 04:53:33 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 04:53:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 04:53:33 GMT
WORKDIR /notary/server
# Sat, 12 Nov 2022 04:53:33 GMT
COPY /notary-server ./ # buildkit
# Sat, 12 Nov 2022 04:53:34 GMT
RUN ./notary-server --version # buildkit
# Sat, 12 Nov 2022 04:53:34 GMT
COPY ./server-config.json . # buildkit
# Sat, 12 Nov 2022 04:53:34 GMT
COPY ./entrypoint.sh . # buildkit
# Sat, 12 Nov 2022 04:53:34 GMT
USER notary
# Sat, 12 Nov 2022 04:53:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 04:53:34 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f84bc6be5fe2d32e4441665bf4590588a5e805f0f4dc59ca7f20062278a1a`  
		Last Modified: Sat, 12 Nov 2022 04:54:08 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33090c22b1906904caf40830c2082f01799849efbaa3e099979f076f82c8b3a1`  
		Last Modified: Sat, 12 Nov 2022 04:54:05 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed154327c2b3fef4d2bffce7f73433261c0a377fa17a1894062da96a6b1c36d`  
		Last Modified: Sat, 12 Nov 2022 04:54:06 GMT  
		Size: 4.9 MB (4888299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02819c04fd0508bf8e160948a57a10a5e758f72a8276bbbf42857938abdaa892`  
		Last Modified: Sat, 12 Nov 2022 04:54:06 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c16e7a5248dd730be74bd565dadef6ea56f1ae328ce05cc366f6e827eb4cb99`  
		Last Modified: Sat, 12 Nov 2022 04:54:05 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1114f4089f5920f6f3aa6d9e0913d4683ba9225dcdf9723c48fcd1346a744a6`  
		Last Modified: Sat, 12 Nov 2022 04:54:05 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:3e1ec7d20889f7c37f6c13476a2763bb3d5eab5be137e327d7266fb172637566
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7441460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cada7634040dfd4c2fb6ec3b7ab4b20c831addd6233a912373688a70cdef2e17`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:36:49 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:36:49 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 12 Nov 2022 04:36:49 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 04:36:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 04:36:49 GMT
WORKDIR /notary/server
# Sat, 12 Nov 2022 04:36:49 GMT
COPY /notary-server ./ # buildkit
# Sat, 12 Nov 2022 04:36:49 GMT
RUN ./notary-server --version # buildkit
# Sat, 12 Nov 2022 04:36:49 GMT
COPY ./server-config.json . # buildkit
# Sat, 12 Nov 2022 04:36:49 GMT
COPY ./entrypoint.sh . # buildkit
# Sat, 12 Nov 2022 04:36:49 GMT
USER notary
# Sat, 12 Nov 2022 04:36:49 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 04:36:49 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d302558fe89c8fe780469f0b8d23bc5062a020060a765fb3f2fbf0d7504a640`  
		Last Modified: Sat, 12 Nov 2022 04:37:07 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e2765c49d0f6fd3ccbc844595f80ded29859b5546f880e4c2a30817ec85cf3`  
		Last Modified: Sat, 12 Nov 2022 04:37:05 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ab16aa9d289192b939cf8bc6a258048be4b1b14a5bac7450d1ccb992a88493`  
		Last Modified: Sat, 12 Nov 2022 04:37:06 GMT  
		Size: 4.7 MB (4731486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d0df93b3fce10e0eeac63d0e744daa330473f98746261aa8ac8dab31e2889`  
		Last Modified: Sat, 12 Nov 2022 04:37:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c37043c32ac4de9b32a8b409ed6dec9dc27ac9b83c95193a93f4bf2b3322ad`  
		Last Modified: Sat, 12 Nov 2022 04:37:05 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ebc35692711619a05d7ea3c0f41a7fec4ff661d473346460a7ec518c653b02`  
		Last Modified: Sat, 12 Nov 2022 04:37:05 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; 386

```console
$ docker pull notary@sha256:dc205a0a528df0f22dbbb47fb8c6338845d02b0452530f5523b0349a262368c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7754936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913b38d2891705de5ca595c05ce624501d91bb6ed027abdb2009db20cf68d7fb`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:57:54 GMT
RUN adduser -D -H -g "" notary
# Sat, 12 Nov 2022 04:57:55 GMT
EXPOSE 4443
# Sat, 12 Nov 2022 04:57:56 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 04:57:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 04:57:58 GMT
WORKDIR /notary/server
# Sat, 12 Nov 2022 04:58:00 GMT
COPY file:0a1052f2e85f22b78af7f4b75052a7720366ea3e414c533f54520e6b3a594392 in ./ 
# Sat, 12 Nov 2022 04:58:00 GMT
RUN ./notary-server --version
# Sat, 12 Nov 2022 04:58:02 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Sat, 12 Nov 2022 04:58:03 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Sat, 12 Nov 2022 04:58:03 GMT
USER notary
# Sat, 12 Nov 2022 04:58:04 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 04:58:05 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:0c10ccf9426f4a034c81b9e1a0fa81fc5cd957d8a4e0ea545ee33f4cd59f227b`  
		Last Modified: Sat, 12 Nov 2022 03:39:07 GMT  
		Size: 2.8 MB (2808348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e2a37344f15c9c47f28fb76d0bbfae6f9adb65b4d686216a9a5881505ed0ec`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9866a73f72dbc8d55f6da18666277753336525decc6cf3f5862f64f9aede0bb4`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f807281d7746373b4c96a20c56871ca4004ef2842968501c905d5dc16f6e04`  
		Last Modified: Sat, 12 Nov 2022 04:58:41 GMT  
		Size: 4.9 MB (4944486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4048b9d6704fc9db240c489997638ce169b4de7a94e984e4f8941fa447b3dd2a`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b695d3994f6d79f70083b1026ce0d89c14c995654fb129b9626cb6d5b2ad919`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; ppc64le

```console
$ docker pull notary@sha256:4ca31bfcdb4a6d89b58aa9f067d597229713d7d5275543c8dc6b8931eed2b558
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7438784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaffe1ddf7527db170da86817e9d28b6ba910c80c1cb1af2ce64ba007b379ff6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 03:23:54 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 03:23:54 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 25 Oct 2022 03:23:54 GMT
ENV INSTALLDIR=/notary/server
# Tue, 25 Oct 2022 03:23:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 25 Oct 2022 03:23:54 GMT
WORKDIR /notary/server
# Tue, 01 Nov 2022 19:52:44 GMT
COPY /notary-server ./ # buildkit
# Tue, 01 Nov 2022 19:52:45 GMT
RUN ./notary-server --version # buildkit
# Tue, 01 Nov 2022 19:52:45 GMT
COPY ./server-config.json . # buildkit
# Tue, 01 Nov 2022 19:52:46 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 01 Nov 2022 19:52:46 GMT
USER notary
# Tue, 01 Nov 2022 19:52:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 01 Nov 2022 19:52:46 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28847305e982967909062e053ecacc81ae6035a3f7b3587b0e54677ab21f709c`  
		Last Modified: Tue, 25 Oct 2022 03:25:00 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7d5711e3906a11f7dc77d3091b7991f23e497d88cd28b0d987afae0a8d597f`  
		Last Modified: Tue, 25 Oct 2022 03:24:57 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15db5598874eb3b3ecd9bb5c44cb36d683a05e4313c56aaf88b63babed2b8182`  
		Last Modified: Tue, 01 Nov 2022 19:53:19 GMT  
		Size: 4.6 MB (4633225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe346e270ce2d6d41eeb31a763b028ebe66b6aefe9aae57784708949e29f1da`  
		Last Modified: Tue, 01 Nov 2022 19:53:17 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3267ca5eea7a1a7caad2876f477ab40b3c51b3f0eea788f81aa387097710b81`  
		Last Modified: Tue, 01 Nov 2022 19:53:17 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44ccd55cd93121224074cecdb36f928912b551da93ffb74da116d8abc17dac`  
		Last Modified: Tue, 01 Nov 2022 19:53:18 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server` - linux; s390x

```console
$ docker pull notary@sha256:870f4bca386cf3b2cace6eb81b7fdf7a41cf612b49d78ab8b4faf3aec65b100e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7562067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fc61ec13e1c56504cad297107ee38033a27ecaef5ae0e3e0472301df9022760`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:29:11 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 05:29:11 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 12 Nov 2022 05:29:11 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 05:29:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 05:29:11 GMT
WORKDIR /notary/server
# Sat, 12 Nov 2022 05:29:11 GMT
COPY /notary-server ./ # buildkit
# Sat, 12 Nov 2022 05:29:11 GMT
RUN ./notary-server --version # buildkit
# Sat, 12 Nov 2022 05:29:11 GMT
COPY ./server-config.json . # buildkit
# Sat, 12 Nov 2022 05:29:12 GMT
COPY ./entrypoint.sh . # buildkit
# Sat, 12 Nov 2022 05:29:12 GMT
USER notary
# Sat, 12 Nov 2022 05:29:12 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 05:29:12 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:cff16a5ffe2df97bc1d10b021c5ceb98bdb36a18a1d70395590444ac204a9b2b`  
		Last Modified: Sat, 12 Nov 2022 03:43:06 GMT  
		Size: 2.6 MB (2591126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4ef31691b8350e3f169efda08440ffc8f858999b921631575acdfd35d88225`  
		Last Modified: Sat, 12 Nov 2022 05:29:49 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba78ca725314efb5b67eb6424fd58fc99193e2ba05a043a971a5d7bb549454fa`  
		Last Modified: Sat, 12 Nov 2022 05:29:47 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c18aee86310db355099abac8db72c7a7ce9cec9d90cd152014bac4c9e362f95`  
		Last Modified: Sat, 12 Nov 2022 05:29:48 GMT  
		Size: 5.0 MB (4968727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d688cb67bac28c4f2f131814b1956c43122b8faa02944a2293a819cf3a62e663`  
		Last Modified: Sat, 12 Nov 2022 05:29:47 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e612ec147d0337956004207865cd1454109cda75072884a75172edbc7aa83af7`  
		Last Modified: Sat, 12 Nov 2022 05:29:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1168634fb4594bf745b436f3a089f254870cdb538142ef25b85c8195e5417533`  
		Last Modified: Sat, 12 Nov 2022 05:29:47 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:server-0.7.0`

```console
$ docker pull notary@sha256:6ce6beac8cd9033b153438e2d9ed88087671eb7f868691ca8be790a640618c47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:server-0.7.0` - linux; amd64

```console
$ docker pull notary@sha256:725646c4d072977023698a3c1b25fc68862ed1646e26b7f8ae60ad7c2549a59e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.0 MB (7951963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e9925dcb4c27e30de0f81ce854368e4f7c8246d84b40e220ca2aa581b356543`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 01:52:21 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 01:52:21 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 25 Oct 2022 01:52:21 GMT
ENV INSTALLDIR=/notary/server
# Tue, 25 Oct 2022 01:52:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 25 Oct 2022 01:52:21 GMT
WORKDIR /notary/server
# Tue, 01 Nov 2022 19:49:00 GMT
COPY /notary-server ./ # buildkit
# Tue, 01 Nov 2022 19:49:00 GMT
RUN ./notary-server --version # buildkit
# Tue, 01 Nov 2022 19:49:00 GMT
COPY ./server-config.json . # buildkit
# Tue, 01 Nov 2022 19:49:00 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 01 Nov 2022 19:49:00 GMT
USER notary
# Tue, 01 Nov 2022 19:49:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 01 Nov 2022 19:49:00 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae0db85ee62912972b015b43b47b5849f5b66900a08ad146a42f7c16d02def`  
		Last Modified: Tue, 25 Oct 2022 01:53:00 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae714b9c46c68b869025bf262b5afec2bb7f99f3739cdae14e11604248f87fd`  
		Last Modified: Tue, 25 Oct 2022 01:52:58 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288b5f0093c5cb556b6e816cc8c65e59ea4a3be57cd8c9cfbab00dbe5bcdb49c`  
		Last Modified: Tue, 01 Nov 2022 19:49:21 GMT  
		Size: 5.1 MB (5143673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca8a52dd6617ccfc327338630a16dcd2ef53f59ec3014397fd87e6ace50c555`  
		Last Modified: Tue, 01 Nov 2022 19:49:20 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5a71241ee3d85608914a3d2c7779ce29252304f4225ad71dcfe3c1b046f3a2`  
		Last Modified: Tue, 01 Nov 2022 19:49:20 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c863d998853c7cbc0e52dbf21a83074cbc3f2acc5cec1f9cb7992d95cffe7e`  
		Last Modified: Tue, 01 Nov 2022 19:49:20 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:b1009bcad7b6a49141436b4fd03fd73ae2b58547f836123cf4b4fd0d0aedbb1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7505595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54ecccd1c21b9543ad2c0070218ddb0a2bf3d250d3d0daa529a10a5e5f9cce54`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:53:33 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:53:33 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 12 Nov 2022 04:53:33 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 04:53:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 04:53:33 GMT
WORKDIR /notary/server
# Sat, 12 Nov 2022 04:53:33 GMT
COPY /notary-server ./ # buildkit
# Sat, 12 Nov 2022 04:53:34 GMT
RUN ./notary-server --version # buildkit
# Sat, 12 Nov 2022 04:53:34 GMT
COPY ./server-config.json . # buildkit
# Sat, 12 Nov 2022 04:53:34 GMT
COPY ./entrypoint.sh . # buildkit
# Sat, 12 Nov 2022 04:53:34 GMT
USER notary
# Sat, 12 Nov 2022 04:53:34 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 04:53:34 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f84bc6be5fe2d32e4441665bf4590588a5e805f0f4dc59ca7f20062278a1a`  
		Last Modified: Sat, 12 Nov 2022 04:54:08 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33090c22b1906904caf40830c2082f01799849efbaa3e099979f076f82c8b3a1`  
		Last Modified: Sat, 12 Nov 2022 04:54:05 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed154327c2b3fef4d2bffce7f73433261c0a377fa17a1894062da96a6b1c36d`  
		Last Modified: Sat, 12 Nov 2022 04:54:06 GMT  
		Size: 4.9 MB (4888299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02819c04fd0508bf8e160948a57a10a5e758f72a8276bbbf42857938abdaa892`  
		Last Modified: Sat, 12 Nov 2022 04:54:06 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c16e7a5248dd730be74bd565dadef6ea56f1ae328ce05cc366f6e827eb4cb99`  
		Last Modified: Sat, 12 Nov 2022 04:54:05 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1114f4089f5920f6f3aa6d9e0913d4683ba9225dcdf9723c48fcd1346a744a6`  
		Last Modified: Sat, 12 Nov 2022 04:54:05 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:3e1ec7d20889f7c37f6c13476a2763bb3d5eab5be137e327d7266fb172637566
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7441460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cada7634040dfd4c2fb6ec3b7ab4b20c831addd6233a912373688a70cdef2e17`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:36:49 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:36:49 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 12 Nov 2022 04:36:49 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 04:36:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 04:36:49 GMT
WORKDIR /notary/server
# Sat, 12 Nov 2022 04:36:49 GMT
COPY /notary-server ./ # buildkit
# Sat, 12 Nov 2022 04:36:49 GMT
RUN ./notary-server --version # buildkit
# Sat, 12 Nov 2022 04:36:49 GMT
COPY ./server-config.json . # buildkit
# Sat, 12 Nov 2022 04:36:49 GMT
COPY ./entrypoint.sh . # buildkit
# Sat, 12 Nov 2022 04:36:49 GMT
USER notary
# Sat, 12 Nov 2022 04:36:49 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 04:36:49 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d302558fe89c8fe780469f0b8d23bc5062a020060a765fb3f2fbf0d7504a640`  
		Last Modified: Sat, 12 Nov 2022 04:37:07 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e2765c49d0f6fd3ccbc844595f80ded29859b5546f880e4c2a30817ec85cf3`  
		Last Modified: Sat, 12 Nov 2022 04:37:05 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ab16aa9d289192b939cf8bc6a258048be4b1b14a5bac7450d1ccb992a88493`  
		Last Modified: Sat, 12 Nov 2022 04:37:06 GMT  
		Size: 4.7 MB (4731486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d0df93b3fce10e0eeac63d0e744daa330473f98746261aa8ac8dab31e2889`  
		Last Modified: Sat, 12 Nov 2022 04:37:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c37043c32ac4de9b32a8b409ed6dec9dc27ac9b83c95193a93f4bf2b3322ad`  
		Last Modified: Sat, 12 Nov 2022 04:37:05 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ebc35692711619a05d7ea3c0f41a7fec4ff661d473346460a7ec518c653b02`  
		Last Modified: Sat, 12 Nov 2022 04:37:05 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; 386

```console
$ docker pull notary@sha256:dc205a0a528df0f22dbbb47fb8c6338845d02b0452530f5523b0349a262368c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.8 MB (7754936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913b38d2891705de5ca595c05ce624501d91bb6ed027abdb2009db20cf68d7fb`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:57:54 GMT
RUN adduser -D -H -g "" notary
# Sat, 12 Nov 2022 04:57:55 GMT
EXPOSE 4443
# Sat, 12 Nov 2022 04:57:56 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 04:57:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 04:57:58 GMT
WORKDIR /notary/server
# Sat, 12 Nov 2022 04:58:00 GMT
COPY file:0a1052f2e85f22b78af7f4b75052a7720366ea3e414c533f54520e6b3a594392 in ./ 
# Sat, 12 Nov 2022 04:58:00 GMT
RUN ./notary-server --version
# Sat, 12 Nov 2022 04:58:02 GMT
COPY file:33643ab6368f7007610a81abd5ef291ec43cbd47a0d1581b29490690dc44f709 in . 
# Sat, 12 Nov 2022 04:58:03 GMT
COPY file:ad1ab25ac8ceb29f1cdc7363c26c083887d76bdbd37db998baad09873ef0811e in . 
# Sat, 12 Nov 2022 04:58:03 GMT
USER notary
# Sat, 12 Nov 2022 04:58:04 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 04:58:05 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:0c10ccf9426f4a034c81b9e1a0fa81fc5cd957d8a4e0ea545ee33f4cd59f227b`  
		Last Modified: Sat, 12 Nov 2022 03:39:07 GMT  
		Size: 2.8 MB (2808348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e2a37344f15c9c47f28fb76d0bbfae6f9adb65b4d686216a9a5881505ed0ec`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9866a73f72dbc8d55f6da18666277753336525decc6cf3f5862f64f9aede0bb4`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f807281d7746373b4c96a20c56871ca4004ef2842968501c905d5dc16f6e04`  
		Last Modified: Sat, 12 Nov 2022 04:58:41 GMT  
		Size: 4.9 MB (4944486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4048b9d6704fc9db240c489997638ce169b4de7a94e984e4f8941fa447b3dd2a`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b695d3994f6d79f70083b1026ce0d89c14c995654fb129b9626cb6d5b2ad919`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:4ca31bfcdb4a6d89b58aa9f067d597229713d7d5275543c8dc6b8931eed2b558
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7438784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaffe1ddf7527db170da86817e9d28b6ba910c80c1cb1af2ce64ba007b379ff6`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 03:23:54 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 03:23:54 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 25 Oct 2022 03:23:54 GMT
ENV INSTALLDIR=/notary/server
# Tue, 25 Oct 2022 03:23:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 25 Oct 2022 03:23:54 GMT
WORKDIR /notary/server
# Tue, 01 Nov 2022 19:52:44 GMT
COPY /notary-server ./ # buildkit
# Tue, 01 Nov 2022 19:52:45 GMT
RUN ./notary-server --version # buildkit
# Tue, 01 Nov 2022 19:52:45 GMT
COPY ./server-config.json . # buildkit
# Tue, 01 Nov 2022 19:52:46 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 01 Nov 2022 19:52:46 GMT
USER notary
# Tue, 01 Nov 2022 19:52:46 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 01 Nov 2022 19:52:46 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28847305e982967909062e053ecacc81ae6035a3f7b3587b0e54677ab21f709c`  
		Last Modified: Tue, 25 Oct 2022 03:25:00 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7d5711e3906a11f7dc77d3091b7991f23e497d88cd28b0d987afae0a8d597f`  
		Last Modified: Tue, 25 Oct 2022 03:24:57 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15db5598874eb3b3ecd9bb5c44cb36d683a05e4313c56aaf88b63babed2b8182`  
		Last Modified: Tue, 01 Nov 2022 19:53:19 GMT  
		Size: 4.6 MB (4633225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe346e270ce2d6d41eeb31a763b028ebe66b6aefe9aae57784708949e29f1da`  
		Last Modified: Tue, 01 Nov 2022 19:53:17 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3267ca5eea7a1a7caad2876f477ab40b3c51b3f0eea788f81aa387097710b81`  
		Last Modified: Tue, 01 Nov 2022 19:53:17 GMT  
		Size: 422.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a44ccd55cd93121224074cecdb36f928912b551da93ffb74da116d8abc17dac`  
		Last Modified: Tue, 01 Nov 2022 19:53:18 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:server-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:870f4bca386cf3b2cace6eb81b7fdf7a41cf612b49d78ab8b4faf3aec65b100e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7562067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fc61ec13e1c56504cad297107ee38033a27ecaef5ae0e3e0472301df9022760`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:29:11 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 05:29:11 GMT
EXPOSE map[4443/tcp:{}]
# Sat, 12 Nov 2022 05:29:11 GMT
ENV INSTALLDIR=/notary/server
# Sat, 12 Nov 2022 05:29:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Sat, 12 Nov 2022 05:29:11 GMT
WORKDIR /notary/server
# Sat, 12 Nov 2022 05:29:11 GMT
COPY /notary-server ./ # buildkit
# Sat, 12 Nov 2022 05:29:11 GMT
RUN ./notary-server --version # buildkit
# Sat, 12 Nov 2022 05:29:11 GMT
COPY ./server-config.json . # buildkit
# Sat, 12 Nov 2022 05:29:12 GMT
COPY ./entrypoint.sh . # buildkit
# Sat, 12 Nov 2022 05:29:12 GMT
USER notary
# Sat, 12 Nov 2022 05:29:12 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 05:29:12 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:cff16a5ffe2df97bc1d10b021c5ceb98bdb36a18a1d70395590444ac204a9b2b`  
		Last Modified: Sat, 12 Nov 2022 03:43:06 GMT  
		Size: 2.6 MB (2591126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4ef31691b8350e3f169efda08440ffc8f858999b921631575acdfd35d88225`  
		Last Modified: Sat, 12 Nov 2022 05:29:49 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba78ca725314efb5b67eb6424fd58fc99193e2ba05a043a971a5d7bb549454fa`  
		Last Modified: Sat, 12 Nov 2022 05:29:47 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c18aee86310db355099abac8db72c7a7ce9cec9d90cd152014bac4c9e362f95`  
		Last Modified: Sat, 12 Nov 2022 05:29:48 GMT  
		Size: 5.0 MB (4968727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d688cb67bac28c4f2f131814b1956c43122b8faa02944a2293a819cf3a62e663`  
		Last Modified: Sat, 12 Nov 2022 05:29:47 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e612ec147d0337956004207865cd1454109cda75072884a75172edbc7aa83af7`  
		Last Modified: Sat, 12 Nov 2022 05:29:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1168634fb4594bf745b436f3a089f254870cdb538142ef25b85c8195e5417533`  
		Last Modified: Sat, 12 Nov 2022 05:29:47 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer`

```console
$ docker pull notary@sha256:8f27616e3850c948df084831f33072c08ca6d6d49b2f88caeb215f042664e438
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:signer` - linux; amd64

```console
$ docker pull notary@sha256:0a2df6aad290e2b26791851f575d7e51364f1b356895234542e5263114dd0e97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7565041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb7986ccf50366af23344bbe5e5bea20d70224321eab041ce94bbc227fd28d29`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 01:52:21 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 01:52:46 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 25 Oct 2022 01:52:46 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 25 Oct 2022 01:52:46 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 25 Oct 2022 01:52:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 25 Oct 2022 01:52:46 GMT
WORKDIR /notary/signer
# Tue, 01 Nov 2022 19:49:09 GMT
COPY /notary-signer ./ # buildkit
# Tue, 01 Nov 2022 19:49:10 GMT
RUN ./notary-signer --version # buildkit
# Tue, 01 Nov 2022 19:49:10 GMT
COPY ./signer-config.json . # buildkit
# Tue, 01 Nov 2022 19:49:10 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 01 Nov 2022 19:49:10 GMT
USER notary
# Tue, 01 Nov 2022 19:49:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 01 Nov 2022 19:49:10 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae0db85ee62912972b015b43b47b5849f5b66900a08ad146a42f7c16d02def`  
		Last Modified: Tue, 25 Oct 2022 01:53:00 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc4162474250e31d2a4a4d6cd0a4f0e9813709d78b77293938ace79068cf662`  
		Last Modified: Tue, 25 Oct 2022 01:53:10 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3192cc45dc578f804bb368238b31cd4f7af695d232971b8cec8a96473f753d4`  
		Last Modified: Tue, 01 Nov 2022 19:49:31 GMT  
		Size: 4.8 MB (4756819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4b82c9255f4ce3761ea28c31e5a78f829497aed8afda0a046a5c824d3457b5`  
		Last Modified: Tue, 01 Nov 2022 19:49:30 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c478cc0a5ed1da94c1f564716ee5f26f416ffb75330a89c1d8ab56b3c42df64`  
		Last Modified: Tue, 01 Nov 2022 19:49:30 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9b5cc15db1001e1f62493bb0f1bbe93104aea8b9faf88bbf46e5ad1cd1500f`  
		Last Modified: Tue, 01 Nov 2022 19:49:30 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:1f82c0dbbc82bd59fbf93f527d7f2ffbd8fc1ed12a8da4c60532973cff5a05c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7135948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b64884ecdc094e3a451c4a0d38a31f16f339236b9b4b7d44939b82dfd361ebb0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:53:33 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:53:47 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 04:53:47 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 04:53:47 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:53:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:53:47 GMT
WORKDIR /notary/signer
# Sat, 12 Nov 2022 04:53:47 GMT
COPY /notary-signer ./ # buildkit
# Sat, 12 Nov 2022 04:53:48 GMT
RUN ./notary-signer --version # buildkit
# Sat, 12 Nov 2022 04:53:48 GMT
COPY ./signer-config.json . # buildkit
# Sat, 12 Nov 2022 04:53:48 GMT
COPY ./entrypoint.sh . # buildkit
# Sat, 12 Nov 2022 04:53:48 GMT
USER notary
# Sat, 12 Nov 2022 04:53:48 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 04:53:48 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f84bc6be5fe2d32e4441665bf4590588a5e805f0f4dc59ca7f20062278a1a`  
		Last Modified: Sat, 12 Nov 2022 04:54:08 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125649f53222ca94f2e22db8ba79ba38d7d33fee96be71c6f2a0e58b1045ac49`  
		Last Modified: Sat, 12 Nov 2022 04:54:19 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b067c75c34c77df098051215649c6c0a8e91da9b069631185bc4f43552cdb008`  
		Last Modified: Sat, 12 Nov 2022 04:54:20 GMT  
		Size: 4.5 MB (4518718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887da1571ffb753050d4233e6ca65667b414bdab8e6b7c5fdada89eb4adf9329`  
		Last Modified: Sat, 12 Nov 2022 04:54:19 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76426b68b449dcb14bbd68fab31fa2f8ec7e1fe8a4967cf9da1d82fa1556c9e`  
		Last Modified: Sat, 12 Nov 2022 04:54:19 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045d2087036baa7a9e416eb846827639481ab99ffe9dfd8adf8bab3523c8f717`  
		Last Modified: Sat, 12 Nov 2022 04:54:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:6f5f4e8131ea03706d970d0246a927c3d53f435f32245a886e376564d6de3985
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7093202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06f0148bae40fc4e6af75c833b0c136f7907e50fc7b73e0bbb40cc8bae0a63d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:36:49 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:36:54 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 04:36:54 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 04:36:54 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:36:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:36:54 GMT
WORKDIR /notary/signer
# Sat, 12 Nov 2022 04:36:54 GMT
COPY /notary-signer ./ # buildkit
# Sat, 12 Nov 2022 04:36:55 GMT
RUN ./notary-signer --version # buildkit
# Sat, 12 Nov 2022 04:36:55 GMT
COPY ./signer-config.json . # buildkit
# Sat, 12 Nov 2022 04:36:55 GMT
COPY ./entrypoint.sh . # buildkit
# Sat, 12 Nov 2022 04:36:55 GMT
USER notary
# Sat, 12 Nov 2022 04:36:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 04:36:55 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d302558fe89c8fe780469f0b8d23bc5062a020060a765fb3f2fbf0d7504a640`  
		Last Modified: Sat, 12 Nov 2022 04:37:07 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92adb73f02c38f4aa06f3e987ca18858a12b469b490a35a7fb86b341f2b68fb4`  
		Last Modified: Sat, 12 Nov 2022 04:37:16 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f4534f74420a6707e247e56d44fb30f5fcfeb1bac1e96b70672bb13b362ace`  
		Last Modified: Sat, 12 Nov 2022 04:37:16 GMT  
		Size: 4.4 MB (4383290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6241ea4149079f8c74be251b95022fd118ff1b81741e8f5d599d09b5c1b26f80`  
		Last Modified: Sat, 12 Nov 2022 04:37:16 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d438ce847e1fb4cb73e893a3250887497305e431729d185fd704a98faa25265`  
		Last Modified: Sat, 12 Nov 2022 04:37:16 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdfeb8c515422b448dcee3e98dc11b02fd15d284c31646030292525bfc85d27`  
		Last Modified: Sat, 12 Nov 2022 04:37:16 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:730c407a687ad5edacc5bac402212abeee2ab1622ea677cbfcf27e57552148b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7381559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30b5b352df59bf814ff2d7ede10a2fc3fadeda4325017a635c635ed8a3316a65`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:57:54 GMT
RUN adduser -D -H -g "" notary
# Sat, 12 Nov 2022 04:58:12 GMT
EXPOSE 4444
# Sat, 12 Nov 2022 04:58:12 GMT
EXPOSE 7899
# Sat, 12 Nov 2022 04:58:13 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:58:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:58:15 GMT
WORKDIR /notary/signer
# Sat, 12 Nov 2022 04:58:17 GMT
COPY file:547f217f94a78fab0511c653078b4c2ebbfc2d07327afb125e8459bd4c7bbf8e in ./ 
# Sat, 12 Nov 2022 04:58:17 GMT
RUN ./notary-signer --version
# Sat, 12 Nov 2022 04:58:19 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 12 Nov 2022 04:58:20 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 12 Nov 2022 04:58:20 GMT
USER notary
# Sat, 12 Nov 2022 04:58:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 04:58:22 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:0c10ccf9426f4a034c81b9e1a0fa81fc5cd957d8a4e0ea545ee33f4cd59f227b`  
		Last Modified: Sat, 12 Nov 2022 03:39:07 GMT  
		Size: 2.8 MB (2808348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e2a37344f15c9c47f28fb76d0bbfae6f9adb65b4d686216a9a5881505ed0ec`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26472dc994c1e659b114a40b8becb18e4595de57079b3495843fe3ee077329d`  
		Last Modified: Sat, 12 Nov 2022 04:58:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a918512c1864d4959e73a6a130bebed64e7f9a6be38abb060713d82ade2db440`  
		Last Modified: Sat, 12 Nov 2022 04:58:52 GMT  
		Size: 4.6 MB (4571173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0689bedb37ea9c2aa60cb8235fc6264542b27b9220a52a32f6d34107475ffc9c`  
		Last Modified: Sat, 12 Nov 2022 04:58:51 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e7b61c42d5fdc9dab1e6b4051424ef57c0298feae0f5be594a713350727e2b`  
		Last Modified: Sat, 12 Nov 2022 04:58:51 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:c6a444dfd239a960e340701bfad02006b246286c230f2305f6c653ea42464ca7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7097887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:627ee952c5249f8d8440af7d2ab75f474164d0357aea1ad5dc0c9df4463491ea`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 03:23:54 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 03:24:38 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 25 Oct 2022 03:24:38 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 25 Oct 2022 03:24:38 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 25 Oct 2022 03:24:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 25 Oct 2022 03:24:38 GMT
WORKDIR /notary/signer
# Tue, 01 Nov 2022 19:52:59 GMT
COPY /notary-signer ./ # buildkit
# Tue, 01 Nov 2022 19:53:00 GMT
RUN ./notary-signer --version # buildkit
# Tue, 01 Nov 2022 19:53:00 GMT
COPY ./signer-config.json . # buildkit
# Tue, 01 Nov 2022 19:53:00 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 01 Nov 2022 19:53:00 GMT
USER notary
# Tue, 01 Nov 2022 19:53:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 01 Nov 2022 19:53:00 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28847305e982967909062e053ecacc81ae6035a3f7b3587b0e54677ab21f709c`  
		Last Modified: Tue, 25 Oct 2022 03:25:00 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d02c20adc11bb8fb2837a5733cf0aef1f84c4cd0634e062b9104f203e79c46`  
		Last Modified: Tue, 25 Oct 2022 03:25:11 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f2de88dbcf04ce9626c74bafcf97cf45b585dc60e23c85da0409a57bf7d8bc`  
		Last Modified: Tue, 01 Nov 2022 19:53:31 GMT  
		Size: 4.3 MB (4292393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996407ef4d21829dea55dc4f2aa8162cfce33818a0c9568770ceb97b9d3ac303`  
		Last Modified: Tue, 01 Nov 2022 19:53:30 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025a48a658974a1648ca85661e1bb74e0ef407c22407dd5d32af42d44359d2d3`  
		Last Modified: Tue, 01 Nov 2022 19:53:30 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29250b3e8ad80fa14098544518d02759194deb3eb0c2c86f56e46b976b336e06`  
		Last Modified: Tue, 01 Nov 2022 19:53:30 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:d5d6b8e5f4c93c3063aadc7ebfc46e8802f2931a88c60b0d31b323f4e4bc7f47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7194496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b4ae846424627d1bc27fd82d9c4b174269d2c260a6820d6e331055beaa2cd1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:29:11 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 05:29:25 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 05:29:25 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 05:29:25 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 05:29:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 05:29:25 GMT
WORKDIR /notary/signer
# Sat, 12 Nov 2022 05:29:26 GMT
COPY /notary-signer ./ # buildkit
# Sat, 12 Nov 2022 05:29:27 GMT
RUN ./notary-signer --version # buildkit
# Sat, 12 Nov 2022 05:29:27 GMT
COPY ./signer-config.json . # buildkit
# Sat, 12 Nov 2022 05:29:27 GMT
COPY ./entrypoint.sh . # buildkit
# Sat, 12 Nov 2022 05:29:27 GMT
USER notary
# Sat, 12 Nov 2022 05:29:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 05:29:27 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:cff16a5ffe2df97bc1d10b021c5ceb98bdb36a18a1d70395590444ac204a9b2b`  
		Last Modified: Sat, 12 Nov 2022 03:43:06 GMT  
		Size: 2.6 MB (2591126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4ef31691b8350e3f169efda08440ffc8f858999b921631575acdfd35d88225`  
		Last Modified: Sat, 12 Nov 2022 05:29:49 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab5959c551fe4b84515f58281a78c8105c856e6509e5d6d5f6140438605e776`  
		Last Modified: Sat, 12 Nov 2022 05:29:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4082365898c22a5e5e3d1dee40f02a634992078f8ac4d9d5b8ee9fb99ac62fe`  
		Last Modified: Sat, 12 Nov 2022 05:29:57 GMT  
		Size: 4.6 MB (4601212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476a971d17cb5d00bbe9b2644e4a92fcd83fb9bfe7028a5f262a5416598d0903`  
		Last Modified: Sat, 12 Nov 2022 05:30:06 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e42c0b96010dbeeb8e7d26d4661e7b16b82d218bdc64b291629c46a3a4572c1`  
		Last Modified: Sat, 12 Nov 2022 05:29:57 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81642580798949db05806bb1ee469fe6f8d454aa5fba863d6a9d00cc586c572`  
		Last Modified: Sat, 12 Nov 2022 05:29:56 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `notary:signer-0.7.0`

```console
$ docker pull notary@sha256:8f27616e3850c948df084831f33072c08ca6d6d49b2f88caeb215f042664e438
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `notary:signer-0.7.0` - linux; amd64

```console
$ docker pull notary@sha256:0a2df6aad290e2b26791851f575d7e51364f1b356895234542e5263114dd0e97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7565041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb7986ccf50366af23344bbe5e5bea20d70224321eab041ce94bbc227fd28d29`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 01:52:21 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 01:52:46 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 25 Oct 2022 01:52:46 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 25 Oct 2022 01:52:46 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 25 Oct 2022 01:52:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 25 Oct 2022 01:52:46 GMT
WORKDIR /notary/signer
# Tue, 01 Nov 2022 19:49:09 GMT
COPY /notary-signer ./ # buildkit
# Tue, 01 Nov 2022 19:49:10 GMT
RUN ./notary-signer --version # buildkit
# Tue, 01 Nov 2022 19:49:10 GMT
COPY ./signer-config.json . # buildkit
# Tue, 01 Nov 2022 19:49:10 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 01 Nov 2022 19:49:10 GMT
USER notary
# Tue, 01 Nov 2022 19:49:10 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 01 Nov 2022 19:49:10 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae0db85ee62912972b015b43b47b5849f5b66900a08ad146a42f7c16d02def`  
		Last Modified: Tue, 25 Oct 2022 01:53:00 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc4162474250e31d2a4a4d6cd0a4f0e9813709d78b77293938ace79068cf662`  
		Last Modified: Tue, 25 Oct 2022 01:53:10 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3192cc45dc578f804bb368238b31cd4f7af695d232971b8cec8a96473f753d4`  
		Last Modified: Tue, 01 Nov 2022 19:49:31 GMT  
		Size: 4.8 MB (4756819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4b82c9255f4ce3761ea28c31e5a78f829497aed8afda0a046a5c824d3457b5`  
		Last Modified: Tue, 01 Nov 2022 19:49:30 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c478cc0a5ed1da94c1f564716ee5f26f416ffb75330a89c1d8ab56b3c42df64`  
		Last Modified: Tue, 01 Nov 2022 19:49:30 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9b5cc15db1001e1f62493bb0f1bbe93104aea8b9faf88bbf46e5ad1cd1500f`  
		Last Modified: Tue, 01 Nov 2022 19:49:30 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; arm variant v6

```console
$ docker pull notary@sha256:1f82c0dbbc82bd59fbf93f527d7f2ffbd8fc1ed12a8da4c60532973cff5a05c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7135948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b64884ecdc094e3a451c4a0d38a31f16f339236b9b4b7d44939b82dfd361ebb0`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:53:33 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:53:47 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 04:53:47 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 04:53:47 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:53:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:53:47 GMT
WORKDIR /notary/signer
# Sat, 12 Nov 2022 04:53:47 GMT
COPY /notary-signer ./ # buildkit
# Sat, 12 Nov 2022 04:53:48 GMT
RUN ./notary-signer --version # buildkit
# Sat, 12 Nov 2022 04:53:48 GMT
COPY ./signer-config.json . # buildkit
# Sat, 12 Nov 2022 04:53:48 GMT
COPY ./entrypoint.sh . # buildkit
# Sat, 12 Nov 2022 04:53:48 GMT
USER notary
# Sat, 12 Nov 2022 04:53:48 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 04:53:48 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f84bc6be5fe2d32e4441665bf4590588a5e805f0f4dc59ca7f20062278a1a`  
		Last Modified: Sat, 12 Nov 2022 04:54:08 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125649f53222ca94f2e22db8ba79ba38d7d33fee96be71c6f2a0e58b1045ac49`  
		Last Modified: Sat, 12 Nov 2022 04:54:19 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b067c75c34c77df098051215649c6c0a8e91da9b069631185bc4f43552cdb008`  
		Last Modified: Sat, 12 Nov 2022 04:54:20 GMT  
		Size: 4.5 MB (4518718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887da1571ffb753050d4233e6ca65667b414bdab8e6b7c5fdada89eb4adf9329`  
		Last Modified: Sat, 12 Nov 2022 04:54:19 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76426b68b449dcb14bbd68fab31fa2f8ec7e1fe8a4967cf9da1d82fa1556c9e`  
		Last Modified: Sat, 12 Nov 2022 04:54:19 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045d2087036baa7a9e416eb846827639481ab99ffe9dfd8adf8bab3523c8f717`  
		Last Modified: Sat, 12 Nov 2022 04:54:19 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:6f5f4e8131ea03706d970d0246a927c3d53f435f32245a886e376564d6de3985
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7093202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06f0148bae40fc4e6af75c833b0c136f7907e50fc7b73e0bbb40cc8bae0a63d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:36:49 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 04:36:54 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 04:36:54 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 04:36:54 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:36:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:36:54 GMT
WORKDIR /notary/signer
# Sat, 12 Nov 2022 04:36:54 GMT
COPY /notary-signer ./ # buildkit
# Sat, 12 Nov 2022 04:36:55 GMT
RUN ./notary-signer --version # buildkit
# Sat, 12 Nov 2022 04:36:55 GMT
COPY ./signer-config.json . # buildkit
# Sat, 12 Nov 2022 04:36:55 GMT
COPY ./entrypoint.sh . # buildkit
# Sat, 12 Nov 2022 04:36:55 GMT
USER notary
# Sat, 12 Nov 2022 04:36:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 04:36:55 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d302558fe89c8fe780469f0b8d23bc5062a020060a765fb3f2fbf0d7504a640`  
		Last Modified: Sat, 12 Nov 2022 04:37:07 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92adb73f02c38f4aa06f3e987ca18858a12b469b490a35a7fb86b341f2b68fb4`  
		Last Modified: Sat, 12 Nov 2022 04:37:16 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f4534f74420a6707e247e56d44fb30f5fcfeb1bac1e96b70672bb13b362ace`  
		Last Modified: Sat, 12 Nov 2022 04:37:16 GMT  
		Size: 4.4 MB (4383290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6241ea4149079f8c74be251b95022fd118ff1b81741e8f5d599d09b5c1b26f80`  
		Last Modified: Sat, 12 Nov 2022 04:37:16 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d438ce847e1fb4cb73e893a3250887497305e431729d185fd704a98faa25265`  
		Last Modified: Sat, 12 Nov 2022 04:37:16 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdfeb8c515422b448dcee3e98dc11b02fd15d284c31646030292525bfc85d27`  
		Last Modified: Sat, 12 Nov 2022 04:37:16 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; 386

```console
$ docker pull notary@sha256:730c407a687ad5edacc5bac402212abeee2ab1622ea677cbfcf27e57552148b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7381559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30b5b352df59bf814ff2d7ede10a2fc3fadeda4325017a635c635ed8a3316a65`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:57:54 GMT
RUN adduser -D -H -g "" notary
# Sat, 12 Nov 2022 04:58:12 GMT
EXPOSE 4444
# Sat, 12 Nov 2022 04:58:12 GMT
EXPOSE 7899
# Sat, 12 Nov 2022 04:58:13 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 04:58:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 04:58:15 GMT
WORKDIR /notary/signer
# Sat, 12 Nov 2022 04:58:17 GMT
COPY file:547f217f94a78fab0511c653078b4c2ebbfc2d07327afb125e8459bd4c7bbf8e in ./ 
# Sat, 12 Nov 2022 04:58:17 GMT
RUN ./notary-signer --version
# Sat, 12 Nov 2022 04:58:19 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Sat, 12 Nov 2022 04:58:20 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Sat, 12 Nov 2022 04:58:20 GMT
USER notary
# Sat, 12 Nov 2022 04:58:21 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 04:58:22 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:0c10ccf9426f4a034c81b9e1a0fa81fc5cd957d8a4e0ea545ee33f4cd59f227b`  
		Last Modified: Sat, 12 Nov 2022 03:39:07 GMT  
		Size: 2.8 MB (2808348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e2a37344f15c9c47f28fb76d0bbfae6f9adb65b4d686216a9a5881505ed0ec`  
		Last Modified: Sat, 12 Nov 2022 04:58:40 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26472dc994c1e659b114a40b8becb18e4595de57079b3495843fe3ee077329d`  
		Last Modified: Sat, 12 Nov 2022 04:58:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a918512c1864d4959e73a6a130bebed64e7f9a6be38abb060713d82ade2db440`  
		Last Modified: Sat, 12 Nov 2022 04:58:52 GMT  
		Size: 4.6 MB (4571173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0689bedb37ea9c2aa60cb8235fc6264542b27b9220a52a32f6d34107475ffc9c`  
		Last Modified: Sat, 12 Nov 2022 04:58:51 GMT  
		Size: 355.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e7b61c42d5fdc9dab1e6b4051424ef57c0298feae0f5be594a713350727e2b`  
		Last Modified: Sat, 12 Nov 2022 04:58:51 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; ppc64le

```console
$ docker pull notary@sha256:c6a444dfd239a960e340701bfad02006b246286c230f2305f6c653ea42464ca7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7097887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:627ee952c5249f8d8440af7d2ab75f474164d0357aea1ad5dc0c9df4463491ea`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 03:23:54 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 03:24:38 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 25 Oct 2022 03:24:38 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 25 Oct 2022 03:24:38 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 25 Oct 2022 03:24:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 25 Oct 2022 03:24:38 GMT
WORKDIR /notary/signer
# Tue, 01 Nov 2022 19:52:59 GMT
COPY /notary-signer ./ # buildkit
# Tue, 01 Nov 2022 19:53:00 GMT
RUN ./notary-signer --version # buildkit
# Tue, 01 Nov 2022 19:53:00 GMT
COPY ./signer-config.json . # buildkit
# Tue, 01 Nov 2022 19:53:00 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 01 Nov 2022 19:53:00 GMT
USER notary
# Tue, 01 Nov 2022 19:53:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 01 Nov 2022 19:53:00 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28847305e982967909062e053ecacc81ae6035a3f7b3587b0e54677ab21f709c`  
		Last Modified: Tue, 25 Oct 2022 03:25:00 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d02c20adc11bb8fb2837a5733cf0aef1f84c4cd0634e062b9104f203e79c46`  
		Last Modified: Tue, 25 Oct 2022 03:25:11 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f2de88dbcf04ce9626c74bafcf97cf45b585dc60e23c85da0409a57bf7d8bc`  
		Last Modified: Tue, 01 Nov 2022 19:53:31 GMT  
		Size: 4.3 MB (4292393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996407ef4d21829dea55dc4f2aa8162cfce33818a0c9568770ceb97b9d3ac303`  
		Last Modified: Tue, 01 Nov 2022 19:53:30 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025a48a658974a1648ca85661e1bb74e0ef407c22407dd5d32af42d44359d2d3`  
		Last Modified: Tue, 01 Nov 2022 19:53:30 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29250b3e8ad80fa14098544518d02759194deb3eb0c2c86f56e46b976b336e06`  
		Last Modified: Tue, 01 Nov 2022 19:53:30 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer-0.7.0` - linux; s390x

```console
$ docker pull notary@sha256:d5d6b8e5f4c93c3063aadc7ebfc46e8802f2931a88c60b0d31b323f4e4bc7f47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7194496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b4ae846424627d1bc27fd82d9c4b174269d2c260a6820d6e331055beaa2cd1`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:29:11 GMT
RUN adduser -D -H -g "" notary # buildkit
# Sat, 12 Nov 2022 05:29:25 GMT
EXPOSE map[4444/tcp:{}]
# Sat, 12 Nov 2022 05:29:25 GMT
EXPOSE map[7899/tcp:{}]
# Sat, 12 Nov 2022 05:29:25 GMT
ENV INSTALLDIR=/notary/signer
# Sat, 12 Nov 2022 05:29:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Sat, 12 Nov 2022 05:29:25 GMT
WORKDIR /notary/signer
# Sat, 12 Nov 2022 05:29:26 GMT
COPY /notary-signer ./ # buildkit
# Sat, 12 Nov 2022 05:29:27 GMT
RUN ./notary-signer --version # buildkit
# Sat, 12 Nov 2022 05:29:27 GMT
COPY ./signer-config.json . # buildkit
# Sat, 12 Nov 2022 05:29:27 GMT
COPY ./entrypoint.sh . # buildkit
# Sat, 12 Nov 2022 05:29:27 GMT
USER notary
# Sat, 12 Nov 2022 05:29:27 GMT
ENTRYPOINT ["entrypoint.sh"]
# Sat, 12 Nov 2022 05:29:27 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:cff16a5ffe2df97bc1d10b021c5ceb98bdb36a18a1d70395590444ac204a9b2b`  
		Last Modified: Sat, 12 Nov 2022 03:43:06 GMT  
		Size: 2.6 MB (2591126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4ef31691b8350e3f169efda08440ffc8f858999b921631575acdfd35d88225`  
		Last Modified: Sat, 12 Nov 2022 05:29:49 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab5959c551fe4b84515f58281a78c8105c856e6509e5d6d5f6140438605e776`  
		Last Modified: Sat, 12 Nov 2022 05:29:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4082365898c22a5e5e3d1dee40f02a634992078f8ac4d9d5b8ee9fb99ac62fe`  
		Last Modified: Sat, 12 Nov 2022 05:29:57 GMT  
		Size: 4.6 MB (4601212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476a971d17cb5d00bbe9b2644e4a92fcd83fb9bfe7028a5f262a5416598d0903`  
		Last Modified: Sat, 12 Nov 2022 05:30:06 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e42c0b96010dbeeb8e7d26d4661e7b16b82d218bdc64b291629c46a3a4572c1`  
		Last Modified: Sat, 12 Nov 2022 05:29:57 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81642580798949db05806bb1ee469fe6f8d454aa5fba863d6a9d00cc586c572`  
		Last Modified: Sat, 12 Nov 2022 05:29:56 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
