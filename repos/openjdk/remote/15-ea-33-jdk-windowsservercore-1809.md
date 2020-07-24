## `openjdk:15-ea-33-jdk-windowsservercore-1809`

```console
$ docker pull openjdk@sha256:60cc153caca75eff86e13fd12bd9f92dfa973eb72f80847d398274ae902fac84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:15-ea-33-jdk-windowsservercore-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:7814096ebcb3b71a883d65368939a65bf2483e37acd4b7cc4fcde402999da651
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2515724308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e16ff9b208fdb2f3d1301da68e173ce8b82d127ca262fd394b55f56a4313731`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Wed, 08 Jul 2020 04:26:49 GMT
RUN Install update 1809-amd64
# Tue, 14 Jul 2020 18:41:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Fri, 24 Jul 2020 18:15:15 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force
# Fri, 24 Jul 2020 18:22:15 GMT
ENV JAVA_HOME=C:\openjdk-15
# Fri, 24 Jul 2020 18:22:36 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath
# Fri, 24 Jul 2020 18:22:37 GMT
ENV JAVA_VERSION=15-ea+33
# Fri, 24 Jul 2020 18:22:38 GMT
ENV JAVA_URL=https://download.java.net/java/early_access/jdk15/33/GPL/openjdk-15-ea+33_windows-x64_bin.zip
# Fri, 24 Jul 2020 18:22:39 GMT
ENV JAVA_SHA256=dd64d924e93166d99883452ab24f5449087055d6736807e6a21ed9934b7e968e
# Fri, 24 Jul 2020 18:24:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Fri, 24 Jul 2020 18:24:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc1b9e59edad2bf789457b52138acc367e86072b73bf862eaf96be70f4d4edbb`  
		Size: 591.9 MB (591859374 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:25edfecb5915de420000d722dc47ef9b13bc344a8330c4300e36a4ec8ca73033`  
		Last Modified: Tue, 14 Jul 2020 19:42:57 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ded26bb196400f1cf541826f3f44c1025664089ba3c58aaf3b7afca018655df`  
		Last Modified: Fri, 24 Jul 2020 18:33:13 GMT  
		Size: 9.2 MB (9158926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0f53144ce773907d36e6c83618a425753b07225d8e931a79d88e33cf3093d1`  
		Last Modified: Fri, 24 Jul 2020 18:35:25 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a60ac3d369ea68fca880f6ca38b2004fad14c7885711c0e640b691fefb6bf`  
		Last Modified: Fri, 24 Jul 2020 18:35:25 GMT  
		Size: 314.3 KB (314280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b3f900142ea31cf541860e7f3dd3941f3723635e753a9e8c72c7e91e25a235`  
		Last Modified: Fri, 24 Jul 2020 18:35:22 GMT  
		Size: 1.1 KB (1076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874a21c1b4b465f65713f58c4709492d543c7849029362e4c1822c10d1115770`  
		Last Modified: Fri, 24 Jul 2020 18:35:22 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae17680772f4041b0ead0477f0fac7a9055b4940b6577914c588acbd4c421f8`  
		Last Modified: Fri, 24 Jul 2020 18:35:23 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59406172cd1183c41ebc12c0c61f354641dcd2d2b895b8055d5759033df942d7`  
		Last Modified: Fri, 24 Jul 2020 18:35:42 GMT  
		Size: 196.1 MB (196052235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bedc6dd3cdd97c71f8c201f991f69559256d0c2b6b3c2294e6065fd78993ee`  
		Last Modified: Fri, 24 Jul 2020 18:35:22 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
