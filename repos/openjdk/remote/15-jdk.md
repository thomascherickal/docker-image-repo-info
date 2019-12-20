## `openjdk:15-jdk`

```console
$ docker pull openjdk@sha256:f31852d8243e5569f5b2f6f2992006dc13953db1fd0055c728f87b14acbb2354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.17763.914; amd64
	-	windows version 10.0.14393.3384; amd64

### `openjdk:15-jdk` - linux; amd64

```console
$ docker pull openjdk@sha256:33fc4ffc084e628bde818d5a1de488ba0a76bc3924e0f622a38a4f182bd988c3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.5 MB (256520066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c82b4a8b70abbb92758dee0f20c1f29d81a1e09538a00e3dd974e27d4379b32d`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Aug 2018 21:49:27 GMT
MAINTAINER Oracle Linux Product Team <ol-ovm-info_ww@oracle.com>
# Fri, 20 Dec 2019 01:46:43 GMT
ADD file:e662b0d428c91ed028fec1db2cccbeddea848eb36b32c8bfad324619b8e57d9f in / 
# Fri, 20 Dec 2019 01:46:44 GMT
CMD ["/bin/bash"]
# Fri, 20 Dec 2019 02:05:13 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Fri, 20 Dec 2019 02:05:13 GMT
ENV LANG=en_US.UTF-8
# Fri, 20 Dec 2019 02:05:13 GMT
ENV JAVA_HOME=/usr/java/openjdk-15
# Fri, 20 Dec 2019 02:05:13 GMT
ENV PATH=/usr/java/openjdk-15/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 20 Dec 2019 02:05:14 GMT
ENV JAVA_VERSION=15-ea+2
# Fri, 20 Dec 2019 02:05:14 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/2/GPL/openjdk-15-ea+2_linux-x64_bin.tar.gz
# Fri, 20 Dec 2019 02:05:14 GMT
ENV JAVA_SHA256=a329c96e555819bfd005a9fbf11e75cd180c2c4331b1d2637c071ff9276e9f69
# Fri, 20 Dec 2019 02:06:44 GMT
RUN set -eux; 		curl -fL -o /openjdk.tgz "$JAVA_URL"; 	echo "$JAVA_SHA256 */openjdk.tgz" | sha256sum -c -; 	mkdir -p "$JAVA_HOME"; 	tar --extract --file /openjdk.tgz --directory "$JAVA_HOME" --strip-components 1; 	rm /openjdk.tgz; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		java --version; 	javac --version
# Fri, 20 Dec 2019 02:06:44 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:822ace0353cbeeb23baa4e10b00916d8aae76c005023f5807d16cd97e6339b9b`  
		Last Modified: Fri, 20 Dec 2019 01:48:50 GMT  
		Size: 42.7 MB (42725372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf4d0631bf4e4c98ff5629cdf7958d9db134bbabd5a323f89f8fd783ca4c524`  
		Last Modified: Fri, 20 Dec 2019 02:10:52 GMT  
		Size: 14.8 MB (14793038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b352a7481516c77f482f69dcb7544d0f071d1d827675872cbf5a9bc95f0375`  
		Last Modified: Fri, 20 Dec 2019 02:11:10 GMT  
		Size: 199.0 MB (199001656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-jdk` - windows version 10.0.17763.914; amd64

```console
$ docker pull openjdk@sha256:b94edcb6123de07a38fdc50a9df64fbd5518de65b9e1897f27d79d5963a5f4f2
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2415426046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24a436f81225b5d649a7157acbec99a42b84e930426fff629aee12631a6d5990`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 29 Nov 2019 04:34:15 GMT
RUN Install update 1809-amd64
# Tue, 10 Dec 2019 21:34:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:41:29 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Thu, 19 Dec 2019 01:22:00 GMT
ENV JAVA_HOME=C:\openjdk-15
# Thu, 19 Dec 2019 01:22:27 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Thu, 19 Dec 2019 23:20:58 GMT
ENV JAVA_VERSION=15-ea+2
# Thu, 19 Dec 2019 23:20:59 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/2/GPL/openjdk-15-ea+2_windows-x64_bin.zip
# Thu, 19 Dec 2019 23:21:00 GMT
ENV JAVA_SHA256=8855c29b5316887a20316a166140366adeeea9e5b28594d07fd4aefb44df65f0
# Thu, 19 Dec 2019 23:23:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 19 Dec 2019 23:23:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:faf31ee0aa3d3c60a38dd03c7554d632065cef50eab052ef1444590786249d07`  
		Size: 681.6 MB (681618026 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e147f14e0d6a9cbd5261162dea8f3aac7a34db5d9f6a587a9aac6b88722a2da4`  
		Last Modified: Tue, 10 Dec 2019 22:07:34 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0c4a671756d1396180ecdf66a8d6708b4290b154606229618d94780b6ab6b3`  
		Last Modified: Wed, 11 Dec 2019 19:58:31 GMT  
		Size: 4.6 MB (4578585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7042a384d9a06800f72ef1e12158b017c64448477780c16789eca5116506a547`  
		Last Modified: Thu, 19 Dec 2019 01:35:21 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7c43af5e831564c83a66de8ab18e497dea4bfc0028a6dee76433bef5dffff2`  
		Last Modified: Thu, 19 Dec 2019 01:35:22 GMT  
		Size: 318.1 KB (318105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d342f7ec8989566c9c9f6c88e6a99e211370496150b08b25e410fe018488af7f`  
		Last Modified: Thu, 19 Dec 2019 23:43:38 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63463f5d2fae8e052ed6630295cb9a4a60f90850b0baccfb8f3cf1bbdd45a330`  
		Last Modified: Thu, 19 Dec 2019 23:43:38 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57b6f82005b91d42d355b9dce8214a6aaf94d3e41db56d36c48af93e0c6a28e`  
		Last Modified: Thu, 19 Dec 2019 23:43:38 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8759ab59f6932c03a721e00fa3106c645646b71543158497826e41e41d93de1`  
		Last Modified: Thu, 19 Dec 2019 23:44:01 GMT  
		Size: 194.2 MB (194218871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7801f9a09c1bd1eca5e32d9f93a5ed1dcd9c4461c7396bdd7d102ce7e25916`  
		Last Modified: Thu, 19 Dec 2019 23:43:38 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:15-jdk` - windows version 10.0.14393.3384; amd64

```console
$ docker pull openjdk@sha256:dbf7929024a9e658027c3e843af2cc7dc254e7c5f7a5b2a16e73e71cc997de8e
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5937169939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a154f9d6b574f5790365c738822871e92147c90b358ca8ea8b2c7159eac9623b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 00:35:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Dec 2019 18:45:32 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Thu, 19 Dec 2019 01:24:42 GMT
ENV JAVA_HOME=C:\openjdk-15
# Thu, 19 Dec 2019 01:25:54 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Thu, 19 Dec 2019 23:23:41 GMT
ENV JAVA_VERSION=15-ea+2
# Thu, 19 Dec 2019 23:23:42 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/2/GPL/openjdk-15-ea+2_windows-x64_bin.zip
# Thu, 19 Dec 2019 23:23:43 GMT
ENV JAVA_SHA256=8855c29b5316887a20316a166140366adeeea9e5b28594d07fd4aefb44df65f0
# Thu, 19 Dec 2019 23:28:21 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Thu, 19 Dec 2019 23:28:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:530e4240d4261ce165890648d1df6230dc4f9ce5df2e6cf9f0d5876694c3d4f0`  
		Last Modified: Wed, 11 Dec 2019 01:14:39 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ba7ecb82646b9454a7a416c149a513479fd0ab29aaa2dfbe96281b62668931`  
		Last Modified: Wed, 11 Dec 2019 19:59:59 GMT  
		Size: 5.4 MB (5365131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e59ee70e849f790ad2dd4da52ae1d8b3154ca924aed71fdda94b3c19fa0412`  
		Last Modified: Thu, 19 Dec 2019 01:36:45 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb24f179a5c79b0fa807327ebc5529bab3227974c63983f6c404a19b49cc380`  
		Last Modified: Thu, 19 Dec 2019 01:36:47 GMT  
		Size: 5.4 MB (5350253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde658f4aa9a7679f9505f5d92a163e6741406ad1b1f05f7a27419f21d1fbb94`  
		Last Modified: Thu, 19 Dec 2019 23:44:57 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac0259d933f53d092e0675c58a73dd9561705afcd336606b96bfed86302a846`  
		Last Modified: Thu, 19 Dec 2019 23:44:57 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892160b9bcf7ee522f5ac10253ddf94d09e58be714a1dac4d8a3d115d8e4853a`  
		Last Modified: Thu, 19 Dec 2019 23:44:57 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de71ebdae195286386e54cf65a43db732f2a940e26cf4c11525e9696de302a85`  
		Last Modified: Thu, 19 Dec 2019 23:45:23 GMT  
		Size: 203.7 MB (203743588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29c592d18fc253d546c2a2e89a576ba4bb438e62fc380a6a594b9982ba419ce`  
		Last Modified: Thu, 19 Dec 2019 23:44:57 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
