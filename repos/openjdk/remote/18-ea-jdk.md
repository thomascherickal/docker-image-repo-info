## `openjdk:18-ea-jdk`

```console
$ docker pull openjdk@sha256:55a431f55bc2ba43f4f2ef4de9e7c87429b4febf32c716943687c77a6bf7e560
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `openjdk:18-ea-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:c28bb04ef41f21afe20b56089686f8338a4936c8084bb53d99d8a628b7526627
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.1 MB (243123711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ced75813e3403433450d9a9d1ebeb67ec4eb54921ba9c30535db2809e325cf14`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 23 Jul 2021 01:13:10 GMT
ADD file:c047ac1784a3670f52d12ad67cf238654237149dc2c9d7b921cd005c7ec42105 in / 
# Fri, 23 Jul 2021 01:13:11 GMT
CMD ["/bin/bash"]
# Fri, 23 Jul 2021 06:40:31 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 23 Jul 2021 06:40:32 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 23 Jul 2021 06:40:32 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 06:40:32 GMT
ENV LANG=C.UTF-8
# Fri, 30 Jul 2021 18:49:01 GMT
ENV JAVA_VERSION=18-ea+8
# Fri, 30 Jul 2021 18:49:13 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/8/GPL/openjdk-18-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='7ac0e0def1cf91833e165602d7292f6003ab5e33321ccb57e71019576d739dcd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/8/GPL/openjdk-18-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='2515fe4f653afa4a891250a6001da51e57928b159c0e95a408469053fa15a4ca'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 30 Jul 2021 18:49:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1da50e1664e1b58d93182fe5af093c642668ec93f67fcd8215b9c1979930b84d`  
		Last Modified: Fri, 23 Jul 2021 01:14:27 GMT  
		Size: 42.2 MB (42178827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c8e5a84542212d0126ce88facd146befb1c731fb4faafb50a7b96ad0568cd9`  
		Last Modified: Fri, 23 Jul 2021 06:49:18 GMT  
		Size: 13.4 MB (13390485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e0847038bd8da86775d631fbe4771bfca8f72751a9a69450f919718c84e9b6`  
		Last Modified: Fri, 30 Jul 2021 18:56:13 GMT  
		Size: 187.6 MB (187554399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:3010b20648064dff09c0d2ba2af303e1c7028279e807b1c8348062abb5b4bf50
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.5 MB (242517558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b0cbcc5beab63b3eb2c5e79e5ac8d2559d67fdd1c78448ee6bb4827500ce980`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 23 Jul 2021 00:50:01 GMT
ADD file:2b2b9653730f3bb9d3a6327d4b9a6b425279decd90b84755c033b95536ebe027 in / 
# Fri, 23 Jul 2021 00:50:02 GMT
CMD ["/bin/bash"]
# Fri, 23 Jul 2021 04:34:01 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 23 Jul 2021 04:34:02 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 23 Jul 2021 04:34:02 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 04:34:02 GMT
ENV LANG=C.UTF-8
# Sat, 31 Jul 2021 03:57:56 GMT
ENV JAVA_VERSION=18-ea+8
# Sat, 31 Jul 2021 03:58:20 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/8/GPL/openjdk-18-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='7ac0e0def1cf91833e165602d7292f6003ab5e33321ccb57e71019576d739dcd'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/8/GPL/openjdk-18-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='2515fe4f653afa4a891250a6001da51e57928b159c0e95a408469053fa15a4ca'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 31 Jul 2021 03:58:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a21bf021f71862240d392ffdd7f376294fa46f2729f1771f269c1a888d0aab25`  
		Last Modified: Fri, 23 Jul 2021 00:51:19 GMT  
		Size: 42.0 MB (42040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20d17a0583d5448fece8a45dc16fcd83266885f5eabbeaa44c9bcc8738ed0fa`  
		Last Modified: Fri, 23 Jul 2021 04:45:32 GMT  
		Size: 14.2 MB (14170914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa31e3dbcf48e07d5782ec98ecd68774160f5b85bc163d5c54882c9921d3cbff`  
		Last Modified: Sat, 31 Jul 2021 04:11:17 GMT  
		Size: 186.3 MB (186305888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk` - windows version 10.0.17763.2061; amd64

```console
$ docker pull openjdk@sha256:c3517491b7d201ff520f708c85a9953a19c02ec1b90d035008ae56aacaba8162
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2869153578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d8a162f4d86611aaa509b5313f8726374d24d06e7cbb6f377dde1577a38187`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 02:41:59 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 02:43:11 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Jul 2021 02:43:13 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 14 Jul 2021 02:44:11 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 06 Aug 2021 18:14:33 GMT
ENV JAVA_VERSION=18-ea+9
# Fri, 06 Aug 2021 18:14:35 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/9/GPL/openjdk-18-ea+9_windows-x64_bin.zip
# Fri, 06 Aug 2021 18:14:37 GMT
ENV JAVA_SHA256=a0af7b8be120ff46eec1522875be7e969d43fbee1e06a535ad835f4a57e619d0
# Fri, 06 Aug 2021 18:16:11 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 06 Aug 2021 18:16:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3b24b55401566ea01a5005138a23766b6b6408c2276b7ebd097da01de80897`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60588ed228454a5b9a3ebf90d5ae7109392676a95ebab716cf7bd486f4e257ae`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 365.3 KB (365286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2121b14e07fe4c6047b3da990c93bc98e05e8e5a6585d81ef2973841ca2eb183`  
		Last Modified: Wed, 14 Jul 2021 03:38:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23d09b9f1f97d76bdf221736fe3eea41783f3969bb3ae0601b6f159915c839d`  
		Last Modified: Wed, 14 Jul 2021 03:38:04 GMT  
		Size: 323.5 KB (323485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af090f94db8436654ad5e0ee921d7617a13ff965218325c7592e63ea3a57658e`  
		Last Modified: Fri, 06 Aug 2021 19:18:56 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cb089038e20af70bd4411c0a778fe4a80002afe7d3ca8fb6f1064f3e5bf06e`  
		Last Modified: Fri, 06 Aug 2021 19:18:56 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8cf2889c8d66563869a7f4c470225c2b7217f9a1d03b7630e743c9a62de2ae`  
		Last Modified: Fri, 06 Aug 2021 19:18:56 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ccfabb0747590c5b41571f7078b75ff04d8b48499d817550b9fa6c26e3f66c`  
		Last Modified: Fri, 06 Aug 2021 19:22:19 GMT  
		Size: 183.0 MB (183009777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3575a7e7a42a9a1ec72f165334de06f5648075d6b3ceb1fba3a564c2640698`  
		Last Modified: Fri, 06 Aug 2021 19:18:56 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk` - windows version 10.0.14393.4530; amd64

```console
$ docker pull openjdk@sha256:8ad3b594b2a5a31aa55b74739cd0a543894874c0f895775b5314ad290dde9fa0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6453326948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055921de3a2ccd974b24346a6f04641a99ceb25ee374f96f8d91e6ac8a0c84f4`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 02:46:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jul 2021 02:47:31 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 14 Jul 2021 02:47:33 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 14 Jul 2021 02:49:32 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 06 Aug 2021 18:16:31 GMT
ENV JAVA_VERSION=18-ea+9
# Fri, 06 Aug 2021 18:16:33 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk18/9/GPL/openjdk-18-ea+9_windows-x64_bin.zip
# Fri, 06 Aug 2021 18:16:35 GMT
ENV JAVA_SHA256=a0af7b8be120ff46eec1522875be7e969d43fbee1e06a535ad835f4a57e619d0
# Fri, 06 Aug 2021 18:18:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 06 Aug 2021 18:18:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:624cc64d28951435759fcbbc930532718666f3285fc939c97e36c2cda79f80f2`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4efeafa471485cac56b3d111ef85272828cab146a6a1ada3aeff81bcb4dda8`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 328.5 KB (328523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45c350ba545fbcd3b34762df7d779fa67615b2b172be3c9a4530584c67cb59c`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aac3eb80df2b34c91daf21be91f90376456108b2df777598c0fee81ca546da5`  
		Last Modified: Wed, 14 Jul 2021 03:41:42 GMT  
		Size: 366.6 KB (366564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042fa2c19ee95ddc6478344d891edb44a6940912213707ed8482f7908538e268`  
		Last Modified: Fri, 06 Aug 2021 19:22:41 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260c673c3d21b3e0e46d945dbf4b6ecd27c2b1c3356c1da7dc4b6a70c22b1b47`  
		Last Modified: Fri, 06 Aug 2021 19:22:41 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3974e4ef505fcc1561b87da4b7b74aef374e5ff0a8757cb0e27219e7b209e81`  
		Last Modified: Fri, 06 Aug 2021 19:22:41 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b410d872bac1b206c0ebe08d3490f562fd47331310acd6b82a8a9705df114433`  
		Last Modified: Fri, 06 Aug 2021 19:26:14 GMT  
		Size: 183.0 MB (182991947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0949555c028907984df1a31ebac9be72d803662204a478193bdd5e1f8017749`  
		Last Modified: Fri, 06 Aug 2021 19:22:41 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
