## `rakudo-star:alpine`

```console
$ docker pull rakudo-star@sha256:6ad95241a878afcbf67046e1dda9bb49810b6fb96a17673202905efa8e42aa18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:6fa71c6026f275c416de30d3cf4406951b47962b59dd47fa6e3b49412f0df08a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38437873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9f752754c0aec1856b9776d7aabd4a59b0fe17e8eaf5f9e49a061b393838ed8`
-	Default Command: `["raku"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 03:19:33 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Fri, 07 Oct 2022 03:19:33 GMT
ARG rakudo_version=2022.07-01
# Fri, 07 Oct 2022 03:19:33 GMT
ENV rakudo_version=2022.07-01
# Fri, 07 Oct 2022 03:29:32 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="${tmpdir}/gnupg"     && mkdir $GNUPGHOME     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && wget $pubkeyurl -O ${tmpdir}/key.asc         && gpg --import ${tmpdir}/key.asc     && gpg --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Fri, 07 Oct 2022 03:29:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Fri, 07 Oct 2022 03:29:32 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b032a58f13217a48f25452cfe9c5dee1667512a6ff0fa4d2b96d776a0bcc8d`  
		Last Modified: Fri, 07 Oct 2022 03:29:50 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88f46d9a29287c1600e1814d8a00826925ed7391c7de14fc40d9242b8290f88`  
		Last Modified: Fri, 07 Oct 2022 03:29:57 GMT  
		Size: 35.6 MB (35630550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:a5de21167a0dcd26b784b9fb28d86879981187e3827bf892530a25f8497837cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38129961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a3a318e2e7ec62e178c6b0e0cb8130c5b7ad18eb8c42af6973819b20bf9f217`
-	Default Command: `["raku"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 18 Aug 2022 21:56:45 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Thu, 18 Aug 2022 21:56:46 GMT
ARG rakudo_version=2022.07-01
# Thu, 18 Aug 2022 21:56:47 GMT
ENV rakudo_version=2022.07-01
# Thu, 18 Aug 2022 22:07:08 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="${tmpdir}/gnupg"     && mkdir $GNUPGHOME     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && wget $pubkeyurl -O ${tmpdir}/key.asc         && gpg --import ${tmpdir}/key.asc     && gpg --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Thu, 18 Aug 2022 22:07:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Thu, 18 Aug 2022 22:07:09 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915fc225e8719746acdd0cd05ed1a6d672270be8e8d3b47add920e524ac0f3ed`  
		Last Modified: Thu, 18 Aug 2022 22:07:45 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c527441e853c1286b7ed55870da3a1df811db8f9a9368238e2374a8d337d4f32`  
		Last Modified: Thu, 18 Aug 2022 22:07:52 GMT  
		Size: 35.4 MB (35421060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
