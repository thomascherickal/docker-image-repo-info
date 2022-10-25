## `notary:signer`

```console
$ docker pull notary@sha256:d49c7c7ea4d707793b132a0ab5bf76d46365390cc703b88fe6a6f5c4efc95126
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
$ docker pull notary@sha256:435522136a07d4f5dca5036914d6c54642cb17fd1d0b86badc786a4a49db3a18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7564780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7b034bbaca404162659e59fa203570e78de7572f824a237b851946962f34282`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 01:52:21 GMT
RUN RUN /bin/sh -c adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 01:52:46 GMT
RUN EXPOSE map[4444/tcp:{}]
# Tue, 25 Oct 2022 01:52:46 GMT
RUN EXPOSE map[7899/tcp:{}]
# Tue, 25 Oct 2022 01:52:46 GMT
RUN ENV INSTALLDIR=/notary/signer
# Tue, 25 Oct 2022 01:52:46 GMT
RUN ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 25 Oct 2022 01:52:46 GMT
RUN WORKDIR /notary/signer
# Tue, 25 Oct 2022 01:52:46 GMT
RUN COPY /notary-signer ./ # buildkit
# Tue, 25 Oct 2022 01:52:47 GMT
RUN RUN /bin/sh -c ./notary-signer --version # buildkit
# Tue, 25 Oct 2022 01:52:47 GMT
RUN COPY ./signer-config.json . # buildkit
# Tue, 25 Oct 2022 01:52:47 GMT
RUN COPY ./entrypoint.sh . # buildkit
# Tue, 25 Oct 2022 01:52:47 GMT
RUN USER notary
# Tue, 25 Oct 2022 01:52:47 GMT
RUN ENTRYPOINT ["entrypoint.sh"]
# Tue, 25 Oct 2022 01:52:47 GMT
RUN CMD ["notary-signer" "--version"]
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
	-	`sha256:18ee735c69980c01445ef5036153b011dcdd76875748196eaa8d8775508450ae`  
		Last Modified: Tue, 25 Oct 2022 01:53:11 GMT  
		Size: 4.8 MB (4756567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d68484c344b8650efe9be82c4354b43b79c802c8d9bf93722123e5c3881b9f`  
		Last Modified: Tue, 25 Oct 2022 01:53:10 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f7ed463735c7515ccf5e53f9f11ecb965c358c3c62eb0be96ff7994687582b`  
		Last Modified: Tue, 25 Oct 2022 01:53:10 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6bf69440a2a92b3633d1651c79e0a62ee6db216c30dc6cafdb0f995dba1871`  
		Last Modified: Tue, 25 Oct 2022 01:53:10 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm variant v6

```console
$ docker pull notary@sha256:d737047343618f0d70d7c9cb2ac189478af4d6ed168935d0ba061633e8b19187
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7134276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b353dc614ad8eebf4d39c911410c3308f3094183ef5344178d6c5f4d7edb9759`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 05:30:38 GMT
RUN RUN /bin/sh -c adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 05:31:20 GMT
RUN EXPOSE map[4444/tcp:{}]
# Tue, 25 Oct 2022 05:31:20 GMT
RUN EXPOSE map[7899/tcp:{}]
# Tue, 25 Oct 2022 05:31:20 GMT
RUN ENV INSTALLDIR=/notary/signer
# Tue, 25 Oct 2022 05:31:20 GMT
RUN ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 25 Oct 2022 05:31:20 GMT
RUN WORKDIR /notary/signer
# Tue, 25 Oct 2022 05:31:20 GMT
RUN COPY /notary-signer ./ # buildkit
# Tue, 25 Oct 2022 05:31:20 GMT
RUN RUN /bin/sh -c ./notary-signer --version # buildkit
# Tue, 25 Oct 2022 05:31:20 GMT
RUN COPY ./signer-config.json . # buildkit
# Tue, 25 Oct 2022 05:31:21 GMT
RUN COPY ./entrypoint.sh . # buildkit
# Tue, 25 Oct 2022 05:31:21 GMT
RUN USER notary
# Tue, 25 Oct 2022 05:31:21 GMT
RUN ENTRYPOINT ["entrypoint.sh"]
# Tue, 25 Oct 2022 05:31:21 GMT
RUN CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719245ee64918db6e14bc8a74787353276669a8486a5743651ec04a1872a4357`  
		Last Modified: Tue, 25 Oct 2022 05:31:43 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d24c426545e5b4d77ea372c858835d4d3cda7f072724f0b6481c74caa9c839d`  
		Last Modified: Tue, 25 Oct 2022 05:31:54 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e101f480d02973137ad75695ab85b8e0ec7bdeefb7e2371482241bf63528d703`  
		Last Modified: Tue, 25 Oct 2022 05:31:55 GMT  
		Size: 4.5 MB (4518189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6e3988a2f926074410d34a2d87bbe53f36802c0e38be6c1c85b09945a5fcac`  
		Last Modified: Tue, 25 Oct 2022 05:31:54 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9748c7273393c74b66ac7f7dfe0420f9baf92e62fa32fe236062db7779ebd5`  
		Last Modified: Tue, 25 Oct 2022 05:31:54 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:951dec79ce03244ae12f111261ce3733008b134ad14ac7650be62b80f691e6a8`  
		Last Modified: Tue, 25 Oct 2022 05:31:54 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; arm64 variant v8

```console
$ docker pull notary@sha256:bb7ecfcd9e4a8b266f64ec03ee49c8f587ac866f398440221fe72d6f5ec8f1f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7092579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a85208fecfbe93102e571fbd6aff6362001fd6e7143f988f759dfb14f18be1f`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 05:54:03 GMT
RUN RUN /bin/sh -c adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 05:54:20 GMT
RUN EXPOSE map[4444/tcp:{}]
# Tue, 25 Oct 2022 05:54:20 GMT
RUN EXPOSE map[7899/tcp:{}]
# Tue, 25 Oct 2022 05:54:20 GMT
RUN ENV INSTALLDIR=/notary/signer
# Tue, 25 Oct 2022 05:54:20 GMT
RUN ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 25 Oct 2022 05:54:20 GMT
RUN WORKDIR /notary/signer
# Tue, 25 Oct 2022 05:54:20 GMT
RUN COPY /notary-signer ./ # buildkit
# Tue, 25 Oct 2022 05:54:20 GMT
RUN RUN /bin/sh -c ./notary-signer --version # buildkit
# Tue, 25 Oct 2022 05:54:20 GMT
RUN COPY ./signer-config.json . # buildkit
# Tue, 25 Oct 2022 05:54:20 GMT
RUN COPY ./entrypoint.sh . # buildkit
# Tue, 25 Oct 2022 05:54:20 GMT
RUN USER notary
# Tue, 25 Oct 2022 05:54:20 GMT
RUN ENTRYPOINT ["entrypoint.sh"]
# Tue, 25 Oct 2022 05:54:20 GMT
RUN CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19c11ef8813c7c7e52078792213cc1951b797dfeda0933eb53237672542be0d`  
		Last Modified: Tue, 25 Oct 2022 05:54:34 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bee4f746f272fbd9c98d93ee524cc92d5c98dd19f9296a083af13b222f35c6e`  
		Last Modified: Tue, 25 Oct 2022 05:54:42 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b41838c2b3d75740e68dfa96f93ec5e452ae6e47231d99a306896c55a14efec`  
		Last Modified: Tue, 25 Oct 2022 05:54:43 GMT  
		Size: 4.4 MB (4382761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3645bbf2e19c00cab8fdb74eacb3e271393b8890a066ac9498133abb34849405`  
		Last Modified: Tue, 25 Oct 2022 05:54:42 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e8cbcd163365309c74621c2ad5c71d8fbe849181be6d70297d519fe01229cc`  
		Last Modified: Tue, 25 Oct 2022 05:54:42 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4160e26b212ddc0d69c3a4b344ed158b41e2b8920644fa6f5aa2e182b71a2b60`  
		Last Modified: Tue, 25 Oct 2022 05:54:42 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; 386

```console
$ docker pull notary@sha256:41ceb1a2a68164e052681ab760a948fb52fea3393ce37dc58c3985707eabaf41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7380072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab394df6cb87062cdff8235564cb1991ff182cf4a01240d356e5ed664486d684`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 02:33:41 GMT
RUN adduser -D -H -g "" notary
# Tue, 25 Oct 2022 02:33:59 GMT
EXPOSE 4444
# Tue, 25 Oct 2022 02:34:00 GMT
EXPOSE 7899
# Tue, 25 Oct 2022 02:34:01 GMT
ENV INSTALLDIR=/notary/signer
# Tue, 25 Oct 2022 02:34:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 25 Oct 2022 02:34:03 GMT
WORKDIR /notary/signer
# Tue, 25 Oct 2022 02:34:05 GMT
COPY file:09d7687d8c146cf18d1659c5a0a78b97c5f2e6ec7b411d334f996388b1b2e3af in ./ 
# Tue, 25 Oct 2022 02:34:05 GMT
RUN ./notary-signer --version
# Tue, 25 Oct 2022 02:34:07 GMT
COPY file:180643db1fd4154262e619c42c1255057d49a4c6cd56be3f475942fd0a35a236 in . 
# Tue, 25 Oct 2022 02:34:08 GMT
COPY file:849eab43398bc401ed08e75cbad3ea52969452506337a4135a0ef8144dff93ad in . 
# Tue, 25 Oct 2022 02:34:08 GMT
USER notary
# Tue, 25 Oct 2022 02:34:09 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 25 Oct 2022 02:34:10 GMT
CMD ["notary-signer" "--version"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c692a1d61ff49f4083804ea05880254cdbf59904eff09aa2c9284e77eed914b`  
		Last Modified: Tue, 25 Oct 2022 02:34:26 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edc955b69acafc7ee12b065cf0f66857f32b4058be7283b3be73de602eec02d`  
		Last Modified: Tue, 25 Oct 2022 02:34:38 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c674dd829e9e493e08fdd395a84b43ef965b12013d48301b3fb4e2fa14cbb3`  
		Last Modified: Tue, 25 Oct 2022 02:34:38 GMT  
		Size: 4.6 MB (4570913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4541b493ad7758881293087bf574f6fb5c29092da1d20b3939e0b1bca5ca0a47`  
		Last Modified: Tue, 25 Oct 2022 02:34:38 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4d7b0c60ba4badeebf5a07beec5040221d2638e555844b43eed7d815a9d249`  
		Last Modified: Tue, 25 Oct 2022 02:34:38 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; ppc64le

```console
$ docker pull notary@sha256:1fe0c43c00222e783638e9aba9c825425692177fb01fe0d1efbd6143eb9983f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7097685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d0ec79a73ee9b0723506834cccc9870c6164ac674a9536a2b049b75fbc7c873`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 03:23:54 GMT
RUN RUN /bin/sh -c adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 03:24:38 GMT
RUN EXPOSE map[4444/tcp:{}]
# Tue, 25 Oct 2022 03:24:38 GMT
RUN EXPOSE map[7899/tcp:{}]
# Tue, 25 Oct 2022 03:24:38 GMT
RUN ENV INSTALLDIR=/notary/signer
# Tue, 25 Oct 2022 03:24:38 GMT
RUN ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 25 Oct 2022 03:24:38 GMT
RUN WORKDIR /notary/signer
# Tue, 25 Oct 2022 03:24:39 GMT
RUN COPY /notary-signer ./ # buildkit
# Tue, 25 Oct 2022 03:24:39 GMT
RUN RUN /bin/sh -c ./notary-signer --version # buildkit
# Tue, 25 Oct 2022 03:24:39 GMT
RUN COPY ./signer-config.json . # buildkit
# Tue, 25 Oct 2022 03:24:40 GMT
RUN COPY ./entrypoint.sh . # buildkit
# Tue, 25 Oct 2022 03:24:40 GMT
RUN USER notary
# Tue, 25 Oct 2022 03:24:40 GMT
RUN ENTRYPOINT ["entrypoint.sh"]
# Tue, 25 Oct 2022 03:24:40 GMT
RUN CMD ["notary-signer" "--version"]
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
	-	`sha256:fd951db957408eb2ffcb6be895c03267d8594f16db6200fa5c368d20ec211868`  
		Last Modified: Tue, 25 Oct 2022 03:25:12 GMT  
		Size: 4.3 MB (4292201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416717d912183d36bd8f66acb237bf9444a6acdf48eeb299ab894a94985cea51`  
		Last Modified: Tue, 25 Oct 2022 03:25:11 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd48f3709d243fc9d5e8206f93d08ea32a44684c13efda01b8229f145b3fa420`  
		Last Modified: Tue, 25 Oct 2022 03:25:11 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7222a13476cf791be33c60ec04d9b4c1117014264678770177f9382f9560867`  
		Last Modified: Tue, 25 Oct 2022 03:25:11 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `notary:signer` - linux; s390x

```console
$ docker pull notary@sha256:db12a82c9b66296e5ed9c95a15ed0b7ffd4e7df3ff1f755674065c0828e78762
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7194015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:079db5b5438125037c313d032802e63377417286edfc666e1572380b504ac40e`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["notary-signer","--version"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 01:21:39 GMT
RUN RUN /bin/sh -c adduser -D -H -g "" notary # buildkit
# Tue, 25 Oct 2022 01:22:14 GMT
RUN EXPOSE map[4444/tcp:{}]
# Tue, 25 Oct 2022 01:22:14 GMT
RUN EXPOSE map[7899/tcp:{}]
# Tue, 25 Oct 2022 01:22:14 GMT
RUN ENV INSTALLDIR=/notary/signer
# Tue, 25 Oct 2022 01:22:14 GMT
RUN ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/notary/signer
# Tue, 25 Oct 2022 01:22:14 GMT
RUN WORKDIR /notary/signer
# Tue, 25 Oct 2022 01:22:14 GMT
RUN COPY /notary-signer ./ # buildkit
# Tue, 25 Oct 2022 01:22:14 GMT
RUN RUN /bin/sh -c ./notary-signer --version # buildkit
# Tue, 25 Oct 2022 01:22:14 GMT
RUN COPY ./signer-config.json . # buildkit
# Tue, 25 Oct 2022 01:22:14 GMT
RUN COPY ./entrypoint.sh . # buildkit
# Tue, 25 Oct 2022 01:22:14 GMT
RUN USER notary
# Tue, 25 Oct 2022 01:22:14 GMT
RUN ENTRYPOINT ["entrypoint.sh"]
# Tue, 25 Oct 2022 01:22:14 GMT
RUN CMD ["notary-signer" "--version"]
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
	-	`sha256:914ee92749a07541df36795929204e1db4dde0af26dbffebcd68c5280d62380c`  
		Last Modified: Tue, 25 Oct 2022 01:22:41 GMT  
		Size: 4.6 MB (4601261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:337c5b8b7050aa5b72729655bbe4b7cebfe80b809f416bc9975de2c4024c81ce`  
		Last Modified: Tue, 25 Oct 2022 01:22:40 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0bfe5e7ce871451593a461f32f992f2ed637f9bcedf2a46624e62da2d1b4aa`  
		Last Modified: Tue, 25 Oct 2022 01:22:40 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced1e547d1f2398fd325b348d5c6bf9f71864266123f6eb5cd293c199a3f5e35`  
		Last Modified: Tue, 25 Oct 2022 01:22:40 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
