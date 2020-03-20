## `golang:1-windowsservercore`

```console
$ docker pull golang@sha256:1dd84292d40da05f4729592706256f6ea2a0a72af7a7df04ac4f76d69ba5ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64
	-	windows version 10.0.17763.1098; amd64

### `golang:1-windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull golang@sha256:847039f2deb248a8964a76a953c86a5d6b4e15be8a2ed80b3414009133ad34d1
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5907462010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abe03460bd0573986112908af6a7da898651139d351b3a0047cad3b4d711e80b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Fri, 13 Mar 2020 21:32:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 18 Mar 2020 12:12:50 GMT
ENV GIT_VERSION=2.23.0
# Wed, 18 Mar 2020 12:12:51 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 18 Mar 2020 12:12:52 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 18 Mar 2020 12:12:53 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 18 Mar 2020 12:14:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 12:14:16 GMT
ENV GOPATH=C:\gopath
# Wed, 18 Mar 2020 12:15:28 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 19 Mar 2020 23:15:31 GMT
ENV GOLANG_VERSION=1.14.1
# Thu, 19 Mar 2020 23:19:17 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '4bcc3bbdeba4b298120b4ea78e22b8c0fe93478b47dd7b84d70d97d2b264a0a6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 19 Mar 2020 23:19:19 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f08cc5bf7287bc1d8f72edfe2439c99210e433230a22fc73264fcf1685850ed2`  
		Last Modified: Fri, 13 Mar 2020 22:09:47 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d561174ac001ca0d7adb9545849bd36e269ed33f40531a998720c250c43ffb`  
		Last Modified: Wed, 18 Mar 2020 12:23:55 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d21a03a688a549f1ddaa9d9d5bb998cb8a2c0e9788b802541787ca3f1ed8ff8`  
		Last Modified: Wed, 18 Mar 2020 12:23:53 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4d91f9428f64df474729562c61ed53946510b7ab35a33f254d5cae955259ba`  
		Last Modified: Wed, 18 Mar 2020 12:23:52 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dd05a2f1cca3f7d532ddb895f160f78d4de3724c6ffcf07015232115e4a95f`  
		Last Modified: Wed, 18 Mar 2020 12:23:52 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8427dcc64be825a40aa719b7fa0062a8c227563d3d6e47a4239ea5e013d65401`  
		Last Modified: Wed, 18 Mar 2020 12:23:57 GMT  
		Size: 30.5 MB (30489302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45815090f3ebeaafd58a49c3138251d3bccaaa64ff19dfdf4e7f9c3ac65fd10`  
		Last Modified: Wed, 18 Mar 2020 12:23:49 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d25c2b0e7b36367e585fa0ea36993bf6e78051273a0e15e8251aff32436ad`  
		Last Modified: Wed, 18 Mar 2020 12:23:50 GMT  
		Size: 5.4 MB (5379505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b03500ccae99e39c781406f3a5001ae7f7b2f9c49c4619329fb236f8adc1342`  
		Last Modified: Thu, 19 Mar 2020 23:35:17 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1105ea0128c50be8814bdcec4d21532f28dc441b3d8e4d0ff881ac40d33de9b7`  
		Last Modified: Thu, 19 Mar 2020 23:35:46 GMT  
		Size: 142.8 MB (142822802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee24e840f0a61bb19a2aa549ab643ffa0204f81cb843148311db0e840b6c5f9b`  
		Last Modified: Thu, 19 Mar 2020 23:35:17 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull golang@sha256:b32b1ef714cee24b65ac36c592e63cb0dcbed163cb39584192cb67cf4cbe2f66
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2428660612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:626819e4d50fdd707c45e0c15a0378589b15924a1ac4888c26e90a62cf13b9b6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Mar 2020 12:14:42 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Mar 2020 12:14:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Mar 2020 12:14:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Mar 2020 12:14:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Mar 2020 12:15:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 12:15:56 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Mar 2020 12:16:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 19 Mar 2020 23:19:28 GMT
ENV GOLANG_VERSION=1.14.1
# Thu, 19 Mar 2020 23:22:10 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '4bcc3bbdeba4b298120b4ea78e22b8c0fe93478b47dd7b84d70d97d2b264a0a6'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 19 Mar 2020 23:22:11 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa59504e8a6021f126b043b84b365caa6366766b8fb31f9152e0f859bcfe743`  
		Last Modified: Wed, 11 Mar 2020 12:42:15 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e8d18d31c69c104e81cb83056a05bf2d4e6d4c9c834cd23a1dd372bf5eba4b`  
		Last Modified: Wed, 11 Mar 2020 12:42:05 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc519099bf17d9b046eef0d0e32d954dc7e54a0fa76708db3ae859a8c63b5e2`  
		Last Modified: Wed, 11 Mar 2020 12:42:04 GMT  
		Size: 1.2 KB (1217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ea92b91b1802207727bccdc5c099ba74e7557140d361b762c6107aa11d4632`  
		Last Modified: Wed, 11 Mar 2020 12:42:03 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314fd97d425237bbcc41f14758f52ad3fde96f2c80c5eccb26754caf0c6648ad`  
		Last Modified: Wed, 11 Mar 2020 12:42:32 GMT  
		Size: 29.8 MB (29750573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8237be75b55557e43ddf8cbe4cb67c918a149b9c971ec24857c862665f51ff34`  
		Last Modified: Wed, 11 Mar 2020 12:41:56 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf58a99dd488ee114fd242abf7b0cd3467bd9fba336c94c09c57f5f98355bad`  
		Last Modified: Wed, 11 Mar 2020 12:41:56 GMT  
		Size: 293.4 KB (293392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12bf457f7b203a7f020b08f568326aa3ee61d0d278f4a90a41255ee3566aab9`  
		Last Modified: Thu, 19 Mar 2020 23:36:02 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75aeb671d119fa54561d438c70312691c107cc725e224b9565da7a6b4885b92b`  
		Last Modified: Thu, 19 Mar 2020 23:36:31 GMT  
		Size: 133.3 MB (133270566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7df8f3d55a5670502258382e62e56d5da8a63b7636bba248ea85fb14ffc4f07`  
		Last Modified: Thu, 19 Mar 2020 23:36:02 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
