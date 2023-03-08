## `openjdk:20-rc-jdk`

```console
$ docker pull openjdk@sha256:3afa6ec2644bcbd3c3c19d2075ce72c42f1a6ab9cf8ba571be5f7f4b97cdce5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `openjdk:20-rc-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:f0a8345f95d44036be5a6b658e4a0e675204a3b27b4ad68e436824b24a9f36dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.7 MB (257698173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90688df26b6515d46dbc2d335a11ad038110795cdd57c8eb8b39b2da72483f25`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 08 Mar 2023 20:22:31 GMT
ADD file:eca2b657866c594c67fc9041ad2a4a309e62fc8338add46c3917517649f748b2 in / 
# Wed, 08 Mar 2023 20:22:32 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 20:53:15 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 08 Mar 2023 20:54:53 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 08 Mar 2023 20:54:53 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 20:54:54 GMT
ENV LANG=C.UTF-8
# Wed, 08 Mar 2023 20:54:54 GMT
ENV JAVA_VERSION=20
# Wed, 08 Mar 2023 20:55:04 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-x64_bin.tar.gz'; 			downloadSha256='bb863b2d542976d1ae4b7b81af3e78b1e4247a64644350b552d298d8dc5980dc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-aarch64_bin.tar.gz'; 			downloadSha256='b671dd1513e7bd4f3de6b1424a90a4998997a67593bf259936d55f5e83e31959'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 08 Mar 2023 20:55:04 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:767a87c583278931a33db59dc8586fdcfa03c53a801cce573f0e861c31ec4c89`  
		Last Modified: Wed, 08 Mar 2023 20:24:06 GMT  
		Size: 44.6 MB (44557814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754d31dea44245a0029d262dade1fe4e14228c7182d3efde4994c6a76398bc7`  
		Last Modified: Wed, 08 Mar 2023 20:56:42 GMT  
		Size: 15.0 MB (15014167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90192eef3b0c096f280e178c1d1accc0b7c3191bd1a115121a03740b1134b95e`  
		Last Modified: Wed, 08 Mar 2023 20:58:22 GMT  
		Size: 198.1 MB (198126192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-rc-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c46cc372084e55b20d5d8bf02859ce96f188c90ed907a8c1fb9c23613b9a4ff3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255918182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc872572761dc916300761497ddfc56f9ea7a0ff21fef45aea4f9dd10a5b40d9`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 08 Mar 2023 21:02:19 GMT
ADD file:18f4bd510f88f32e538884e4e633449c2c8dbf8a5f88b6b6b165ab05872d9507 in / 
# Wed, 08 Mar 2023 21:02:19 GMT
CMD ["/bin/bash"]
# Wed, 08 Mar 2023 21:19:53 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 08 Mar 2023 21:20:56 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Wed, 08 Mar 2023 21:20:56 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 21:20:56 GMT
ENV LANG=C.UTF-8
# Wed, 08 Mar 2023 21:20:56 GMT
ENV JAVA_VERSION=20
# Wed, 08 Mar 2023 21:21:07 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-x64_bin.tar.gz'; 			downloadSha256='bb863b2d542976d1ae4b7b81af3e78b1e4247a64644350b552d298d8dc5980dc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_linux-aarch64_bin.tar.gz'; 			downloadSha256='b671dd1513e7bd4f3de6b1424a90a4998997a67593bf259936d55f5e83e31959'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 08 Mar 2023 21:21:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8ff0c9d62930fe3f55e00ba3be2db6be3643b07da9804d1c9b83b0d3181f0df5`  
		Last Modified: Wed, 08 Mar 2023 21:03:40 GMT  
		Size: 43.5 MB (43456139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec39ece690c19b75d657ca26bf156e883914c8bea4948e081819aff289dc43c5`  
		Last Modified: Wed, 08 Mar 2023 21:22:51 GMT  
		Size: 15.8 MB (15834481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70aa63464eb39b4f530bfef9e20ae6f52eadc144ace349fe8701455bdd9bc8bf`  
		Last Modified: Wed, 08 Mar 2023 21:24:25 GMT  
		Size: 196.6 MB (196627562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-rc-jdk` - windows version 10.0.20348.1547; amd64

```console
$ docker pull openjdk@sha256:5674ec69ae88b37564a1d4fc86551ece840b3220ebe201d127e69b20f9e34124
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1874359109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18d098347417bd884e5f7512a6bd8ce1f87201932d73044a4d42288a5e37485e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:14:39 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:21:10 GMT
ENV JAVA_HOME=C:\openjdk-20
# Thu, 16 Feb 2023 02:21:35 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:21:35 GMT
ENV JAVA_VERSION=20
# Thu, 16 Feb 2023 02:21:36 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_windows-x64_bin.zip
# Thu, 16 Feb 2023 02:21:37 GMT
ENV JAVA_SHA256=c92fae5e42b9aecf444a66c8ec563c652f60b1e231dfdd33a4f5a3e3603058fb
# Thu, 16 Feb 2023 02:22:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:22:34 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8108d16cd884206ec4969828d09af6c32cb29b30d6f5ac0628fbaa03f5acbfc3`  
		Last Modified: Thu, 16 Feb 2023 02:27:56 GMT  
		Size: 770.5 KB (770457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f520bad6be4580c1224316e101801e52057f36d215198aa668da2504f6998ae5`  
		Last Modified: Thu, 16 Feb 2023 02:29:56 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f66cf31b599b4ec97d2d9d3780203976660f7b6576ab22a2406051eb36ab55`  
		Last Modified: Thu, 16 Feb 2023 02:29:56 GMT  
		Size: 570.8 KB (570845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce060a4d77f304aab734b10e6271f48153680adec135a5883aab1dcb5adad0d8`  
		Last Modified: Thu, 16 Feb 2023 02:29:54 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d4f99c037b5a4f35382d11cf5d9c241e573e79253634a3c02058e3c07fc207`  
		Last Modified: Thu, 16 Feb 2023 02:29:54 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f285ff2e153a4dc70a78a4dd7694128b95673d0705c3d0a97eca9a23931f41d8`  
		Last Modified: Thu, 16 Feb 2023 02:29:54 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1d01fc6c1fe660c15aa1b3924e99e0e3ec3f4155dfcd70b02b15e2ed5ed954`  
		Last Modified: Thu, 16 Feb 2023 02:30:15 GMT  
		Size: 193.7 MB (193663051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4564cdffbc411bec19fc6cd8a87feaabc82292a195c73531037d0b8c899b171a`  
		Last Modified: Thu, 16 Feb 2023 02:29:54 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-rc-jdk` - windows version 10.0.17763.4010; amd64

```console
$ docker pull openjdk@sha256:1a7a5da2c5cb25ae0adc7a6114044c2e1e699d2d1174b4aec50d72bbab816eee
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2157248017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4887aa10013b02a5d41ccc3e6a45cf12f2cf2adc22321013ae181fee55b33752`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 02:17:23 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:22:54 GMT
ENV JAVA_HOME=C:\openjdk-20
# Thu, 16 Feb 2023 02:24:00 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:24:01 GMT
ENV JAVA_VERSION=20
# Thu, 16 Feb 2023 02:24:02 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk20/bdc68b4b9cbc4ebcb30745c85038d91d/36/GPL/openjdk-20_windows-x64_bin.zip
# Thu, 16 Feb 2023 02:24:02 GMT
ENV JAVA_SHA256=c92fae5e42b9aecf444a66c8ec563c652f60b1e231dfdd33a4f5a3e3603058fb
# Thu, 16 Feb 2023 02:25:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 02:25:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98437cec399b6656d20521928c292ca8c2e4c0c737b7cb970de037167fc8db6f`  
		Last Modified: Thu, 16 Feb 2023 02:28:35 GMT  
		Size: 515.3 KB (515330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadc496d012b41062c24137db8eefb12fbad8bbb9d160b298ce7a3b47818255a`  
		Last Modified: Thu, 16 Feb 2023 02:30:31 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378a39722d3a50f2f006c8f563edb2445cdb17d0dc3403a08fd5bef6be6aad67`  
		Last Modified: Thu, 16 Feb 2023 02:30:31 GMT  
		Size: 333.7 KB (333724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d2279e93f1bb11f0fca3273b59d2b5a25096527552a1cf8a61402b6dd9c603`  
		Last Modified: Thu, 16 Feb 2023 02:30:29 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b07554f745f85568e0c00afce83479dba5a2aac37ca238464c949cd572b1434`  
		Last Modified: Thu, 16 Feb 2023 02:30:29 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b24ee0d046de84b6814ad4e7a17a52dea2d5e1377947617ce488b7e965d40e`  
		Last Modified: Thu, 16 Feb 2023 02:30:29 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4e46d60e05b3d1a991a9f31fb162b77bcc61d8add07599532a74de33be8753`  
		Last Modified: Thu, 16 Feb 2023 02:30:50 GMT  
		Size: 193.4 MB (193432644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63645e1710e545643d1234f4a26693f7ba929c72ba5f80ff58d8400e068981d`  
		Last Modified: Thu, 16 Feb 2023 02:30:29 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
