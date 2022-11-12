## `notary:server`

```console
$ docker pull notary@sha256:f2bc2c16061c7b78a3b720eeb182846a5d58c6d3f1fd75dbacc16198030f72eb
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
$ docker pull notary@sha256:e0bf9c880e5857c4043e9a6fec00f472a2f19af198192a5189c36afc6c1155c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7561572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f6b49a52a7439412f8c0d05706851e5e327b29cf9bd71177f3924a1489347c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-server","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 01:21:39 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 01:21:39 GMT
EXPOSE map[4443/tcp:{}]
# Tue, 25 Oct 2022 01:21:39 GMT
ENV INSTALLDIR=/notary/server
# Tue, 25 Oct 2022 01:21:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/server
# Tue, 25 Oct 2022 01:21:39 GMT
WORKDIR /notary/server
# Tue, 01 Nov 2022 19:22:59 GMT
COPY /notary-server ./ # buildkit
# Tue, 01 Nov 2022 19:22:59 GMT
RUN ./notary-server --version # buildkit
# Tue, 01 Nov 2022 19:23:00 GMT
COPY ./server-config.json . # buildkit
# Tue, 01 Nov 2022 19:23:00 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 01 Nov 2022 19:23:00 GMT
USER notary
# Tue, 01 Nov 2022 19:23:00 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 01 Nov 2022 19:23:00 GMT
CMD ["notary-server" "--version"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e57b7c2a2dbd108e38c96fd7b110170d3b57a921f34c3b015736a93b17e5ad`  
		Last Modified: Tue, 25 Oct 2022 01:22:34 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb73212e82f7d46920138e024d3233301bdffa778ba147338014ae69d65ba43c`  
		Last Modified: Tue, 25 Oct 2022 01:22:33 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0b0f1ca5387a892ad627d97e99e96b30cad174a591dbe1375adac0a87db741`  
		Last Modified: Tue, 01 Nov 2022 19:23:39 GMT  
		Size: 5.0 MB (4968737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203dfc74ac5ba65a949de65aec38016eacb8fe750fe2e5357924559bbd6e5afe`  
		Last Modified: Tue, 01 Nov 2022 19:23:39 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362dedb8e4f58a86a6e7e5965a12eb241b599dc6949f68b22217026f2f3857e5`  
		Last Modified: Tue, 01 Nov 2022 19:23:38 GMT  
		Size: 423.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce527d322ebdd7c3f241053ee30c18e1fa62d83d7449a6c2237a4e32af7c7fea`  
		Last Modified: Tue, 01 Nov 2022 19:23:38 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
