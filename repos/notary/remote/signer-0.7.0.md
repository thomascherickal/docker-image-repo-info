## `notary:signer-0.7.0`

```console
$ docker pull notary@sha256:4b44a59d16891af0c4c7439da6812f594ec41b03c97260ae9f9b0f99503f2efb
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
$ docker pull notary@sha256:da5657339d0cfa767bdb2bafa540af9c6b2dd908ce512761028f550dfea5107e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7193975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9afafc68a1e4b864e64efa729dbbde167e98e147e5ed1036a065be84a600092`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 01:21:39 GMT
RUN adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 01:22:14 GMT
EXPOSE map[4444/tcp:{}]
# Tue, 25 Oct 2022 01:22:14 GMT
EXPOSE map[7899/tcp:{}]
# Tue, 25 Oct 2022 01:22:14 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 25 Oct 2022 01:22:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 25 Oct 2022 01:22:14 GMT
WORKDIR /notary/signer
# Tue, 01 Nov 2022 19:23:18 GMT
COPY /notary-signer ./ # buildkit
# Tue, 01 Nov 2022 19:23:18 GMT
RUN ./notary-signer --version # buildkit
# Tue, 01 Nov 2022 19:23:18 GMT
COPY ./signer-config.json . # buildkit
# Tue, 01 Nov 2022 19:23:18 GMT
COPY ./entrypoint.sh . # buildkit
# Tue, 01 Nov 2022 19:23:18 GMT
USER notary
# Tue, 01 Nov 2022 19:23:18 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 01 Nov 2022 19:23:18 GMT
CMD ["notary-signer" "--version"]
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
	-	`sha256:bc551ab4c025f7c0eea7a8a1e22a13f7c353f3db3a08e4cae43a782e73d9b89a`  
		Last Modified: Tue, 25 Oct 2022 01:22:40 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d777d5c7c7f8c44012da6681277c73552c11a1a8fee1ac2a199efb93ed5f1a`  
		Last Modified: Tue, 01 Nov 2022 19:23:52 GMT  
		Size: 4.6 MB (4601207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a568cfe33412fb2fce4ffe36ec00270e0e9854440486248a43343187b314fe`  
		Last Modified: Tue, 01 Nov 2022 19:23:51 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3544f39b4416a9518311797adda88c8d822f8a0eff90c05508903d230f072aa`  
		Last Modified: Tue, 01 Nov 2022 19:23:51 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c2d2385d5cc36813017f6437df13c00c29a8adf2df304c47091e81e0cbebb9`  
		Last Modified: Tue, 01 Nov 2022 19:23:51 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
