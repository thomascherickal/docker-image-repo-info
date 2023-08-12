## `openjdk:22-ea-10-jdk`

```console
$ docker pull openjdk@sha256:bce5413949ec037a9c46ccb6c4702b1724707fd3a972b602d8d73179419201f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1906; amd64
	-	windows version 10.0.17763.4737; amd64

### `openjdk:22-ea-10-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:c5e3470712a349f81dc50ae4fe41df839aa6a871560ee731cfca0a10b490eba5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.7 MB (264707346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:981906d9c6016d55f5624f4acf5cba3b9bbe924f4c4254d24d5cb570bf490427`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Aug 2023 01:20:36 GMT
ADD file:196115c6281a0a56854066be2766eb0dc9da452f60a060b90bbe681e6b8ffc11 in / 
# Fri, 11 Aug 2023 01:20:36 GMT
CMD ["/bin/bash"]
# Fri, 11 Aug 2023 01:53:51 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Aug 2023 01:53:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 11 Aug 2023 01:53:51 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Aug 2023 01:53:51 GMT
ENV LANG=C.UTF-8
# Sat, 12 Aug 2023 00:02:26 GMT
ENV JAVA_VERSION=22-ea+10
# Sat, 12 Aug 2023 00:02:37 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='aa3e45c81e7269d389411b52c17721916d2acb7d3e7ab6367c62138063f5052b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='e143f6323650bd4747e4304ef07ba80ade1510a71325bc36a7c4f51939cfe423'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Aug 2023 00:02:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b193354265ba898bb7548038f52378b3dbb6aac5afbaca49bb83ccfe51dfadeb`  
		Last Modified: Fri, 11 Aug 2023 01:21:58 GMT  
		Size: 44.9 MB (44910081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e75d2bbaed8a6321c319c610e5cd0923e1fc6a9ad6122e3b9573f10a5166f9e`  
		Last Modified: Fri, 11 Aug 2023 01:56:08 GMT  
		Size: 15.0 MB (15004378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee71eb3023bf943feee66a6e22df8fddf16ce8649e0ac1234bf449819c22485`  
		Last Modified: Sat, 12 Aug 2023 00:06:47 GMT  
		Size: 204.8 MB (204792887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-10-jdk` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:79ac04f95059f68b97a49f8cd9e58a3ddc6dfcdb4ca07265b8c1aec143870506
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.4 MB (262416511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dbc65c05bc78bb481c7e389aecfbe15c75c4c8a86bfedebb3fae6531d5717e3`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Aug 2023 00:40:33 GMT
ADD file:24663feb951dcfae36948e6cbc8697e8bef563d86c15af3daa54a1b830965593 in / 
# Fri, 11 Aug 2023 00:40:34 GMT
CMD ["/bin/bash"]
# Fri, 11 Aug 2023 01:11:14 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Aug 2023 01:11:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Fri, 11 Aug 2023 01:11:14 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Aug 2023 01:11:15 GMT
ENV LANG=C.UTF-8
# Sat, 12 Aug 2023 00:27:02 GMT
ENV JAVA_VERSION=22-ea+10
# Sat, 12 Aug 2023 00:27:19 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='aa3e45c81e7269d389411b52c17721916d2acb7d3e7ab6367c62138063f5052b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='e143f6323650bd4747e4304ef07ba80ade1510a71325bc36a7c4f51939cfe423'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Aug 2023 00:27:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bd2ec1b01835c3bcf117123886f982435cd8e445790b761779f35779d61faad3`  
		Last Modified: Fri, 11 Aug 2023 00:41:41 GMT  
		Size: 43.6 MB (43625591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7023146e285ffba3adcf0df2d0ef98b1f28c00ef46b2ffc20a5c3d01540eba`  
		Last Modified: Fri, 11 Aug 2023 01:13:09 GMT  
		Size: 15.7 MB (15666637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db693960b36ebc99440e85391219e1a89a69753a0894dd8d9f8707c1536b32b2`  
		Last Modified: Sat, 12 Aug 2023 00:31:16 GMT  
		Size: 203.1 MB (203124283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-10-jdk` - windows version 10.0.20348.1906; amd64

```console
$ docker pull openjdk@sha256:8d50987e9996e37c3389131413cff61f74e5da4305d9ed00ad11e185a08156f2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1997221969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064d5e069414e8ae7e2d4ac9f1c4c790c8372ad23fd713818fd0c3840de4e050`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:36:45 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 10 Aug 2023 02:36:46 GMT
ENV JAVA_HOME=C:\openjdk-22
# Thu, 10 Aug 2023 02:37:04 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Fri, 11 Aug 2023 23:59:38 GMT
ENV JAVA_VERSION=22-ea+10
# Fri, 11 Aug 2023 23:59:39 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_windows-x64_bin.zip
# Fri, 11 Aug 2023 23:59:39 GMT
ENV JAVA_SHA256=73edeecf978d8abfc2ce39e4dd4a8ac11b5d067d8711b2c966cb83f006186298
# Sat, 12 Aug 2023 00:00:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 12 Aug 2023 00:00:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a18930eb7350c60f06351657db53550ff8c064f9f63673a2955eb64b696ffbd`  
		Last Modified: Thu, 10 Aug 2023 02:48:56 GMT  
		Size: 452.7 KB (452708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c00de06770671fea1af1d4340401ecedf3ab6e36133f76fd965e626275a3ef6`  
		Last Modified: Thu, 10 Aug 2023 02:48:56 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d260a183baa6941016ec79f387e49673760fd96dd3bae427fc4233c651e2046`  
		Last Modified: Thu, 10 Aug 2023 02:48:56 GMT  
		Size: 262.5 KB (262490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2c7c55acd57adc0d7569853da54d6405e7d18366f57b86780c4c0d367c5587`  
		Last Modified: Sat, 12 Aug 2023 00:08:27 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3729c34b2261c8356c5669ea8aaf79a22223656249a292af8d287e1a9ae663e4`  
		Last Modified: Sat, 12 Aug 2023 00:08:27 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae302077a5385f4bc3defc51ec7a58e7d6318f6fead4e47b0990521adb89f1aa`  
		Last Modified: Sat, 12 Aug 2023 00:08:27 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf07de70800323fc52685801b365d63427e5e79a9e1fcade31b9bba43be4097`  
		Last Modified: Sat, 12 Aug 2023 00:08:48 GMT  
		Size: 199.1 MB (199134640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9d2e05fa1b877d0694ff0b7bd09b60dd6897189b96156212e68e03cbcf57e1`  
		Last Modified: Sat, 12 Aug 2023 00:08:27 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-10-jdk` - windows version 10.0.17763.4737; amd64

```console
$ docker pull openjdk@sha256:432846fa1343273708c0225dc64f66581df96f35790ba824902099476b7b9958
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2195759010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddd74d2e80cadf8e5b4c627849adab27e0a584b6bcb9f270a9bcd3d1c4a3168f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Aug 2023 02:39:19 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 10 Aug 2023 02:39:21 GMT
ENV JAVA_HOME=C:\openjdk-22
# Thu, 10 Aug 2023 02:40:19 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Sat, 12 Aug 2023 00:00:53 GMT
ENV JAVA_VERSION=22-ea+10
# Sat, 12 Aug 2023 00:00:54 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk22/10/GPL/openjdk-22-ea+10_windows-x64_bin.zip
# Sat, 12 Aug 2023 00:00:54 GMT
ENV JAVA_SHA256=73edeecf978d8abfc2ce39e4dd4a8ac11b5d067d8711b2c966cb83f006186298
# Sat, 12 Aug 2023 00:02:31 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Sat, 12 Aug 2023 00:02:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82556c0499019c0d63fc48880317518db1b5694401f0d8420ea2c4961effcee4`  
		Last Modified: Thu, 10 Aug 2023 02:49:35 GMT  
		Size: 250.9 KB (250879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5d5ec7e3c127f5942ff38f7f912fe583a70ebd26a2f23b08ec931d3ac747f0`  
		Last Modified: Thu, 10 Aug 2023 02:49:35 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0adf33ca81bc87626c3e4e8e94d469cc903ac1e4cf98961cbf569e7f7662fd`  
		Last Modified: Thu, 10 Aug 2023 02:49:35 GMT  
		Size: 246.9 KB (246857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1374530d061dd4141a41aa7f4287e18e31dfc569da0db6611df4a798a4de9c8`  
		Last Modified: Sat, 12 Aug 2023 00:09:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e695424805dc03f9df2b8802032059e58358d77935218103a0868c3104962c6c`  
		Last Modified: Sat, 12 Aug 2023 00:09:13 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f558952b52eba6953626528a10096cf46c451e6dc5c973343991d03b4def4d0`  
		Last Modified: Sat, 12 Aug 2023 00:09:13 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1848bdf90445622e87a260584e51ce67cd6cfc86db8cf3da4021823318f73a0d`  
		Last Modified: Sat, 12 Aug 2023 00:09:33 GMT  
		Size: 199.3 MB (199297493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5af17f5ded1fcccfb6cad0ef05759cf5322e15be2d530e82a170c2cbe4ad7`  
		Last Modified: Sat, 12 Aug 2023 00:09:12 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
