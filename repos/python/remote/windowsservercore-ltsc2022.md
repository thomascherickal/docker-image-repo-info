## `python:windowsservercore-ltsc2022`

```console
$ docker pull python@sha256:ae546185750dbd587f7d3eb28ef3069ca4546649b5054ec4fd8b154d0324ab06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.469; amd64

### `python:windowsservercore-ltsc2022` - windows version 10.0.20348.469; amd64

```console
$ docker pull python@sha256:76d007ef9333a0717c4e2d177856acf6ed175ed14025ff72795b2dbcf242e911
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2261223792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4722fe013595670b2acc4e8bb842fa474afe8db13637a1a873af85ee96ddefa9`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 06 Jan 2022 03:56:33 GMT
RUN Install update ltsc2022-amd64
# Tue, 11 Jan 2022 18:59:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 18:59:18 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 19 Jan 2022 17:34:47 GMT
ENV PYTHON_VERSION=3.10.2
# Wed, 19 Jan 2022 17:34:48 GMT
ENV PYTHON_RELEASE=3.10.2
# Wed, 19 Jan 2022 17:36:11 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 19 Jan 2022 17:36:12 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 19 Jan 2022 17:36:14 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 19 Jan 2022 17:36:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 19 Jan 2022 17:36:17 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 19 Jan 2022 17:37:07 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 19 Jan 2022 17:37:08 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b593686e27e7562a5b0696823307ffa822214cee8bd2eec1075eadad4cb9712`  
		Size: 956.0 MB (956001983 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:99e0b71ede60d3b2c5b9053bf27e47c0875590991eede49813d849cc660c7551`  
		Last Modified: Tue, 11 Jan 2022 19:32:06 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4d1d03ea3685619f9f5d6b5564ecb54f5ce083dc8c701e6055980d3b9e15ff`  
		Last Modified: Tue, 11 Jan 2022 19:32:06 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65577982fe91c862ab6a7075b67d014acd4bdc454099be97758dd61294b8e4cc`  
		Last Modified: Wed, 19 Jan 2022 17:50:45 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765dba553b86208ef2010bf7eec2e876b9b29d168690cc559212b4e7a1c8374b`  
		Last Modified: Wed, 19 Jan 2022 17:50:45 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7ad88822d708e4a4f37b25058bb5cfcfabca171fe4046d3f3d97ab4d087a2b`  
		Last Modified: Wed, 19 Jan 2022 17:51:36 GMT  
		Size: 46.8 MB (46796990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3b8406392ab396c3162d5641105fbb2bd1813acb769cc4a79521e8fff16abd`  
		Last Modified: Wed, 19 Jan 2022 17:50:45 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4793fb49e7378eaf5f54fa8a0eb23af9fb9b19cc85a38b4a74666b0a432e2d87`  
		Last Modified: Wed, 19 Jan 2022 17:50:42 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f2afbd33168980abb3349ddfff8ee6af144b36c4c12c9d9836665a9c39e0e5`  
		Last Modified: Wed, 19 Jan 2022 17:50:42 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e71c6ffb1bd6783ceb99ffbd86a0e8cdfb93ce85f883969b98cb594fe9d743`  
		Last Modified: Wed, 19 Jan 2022 17:50:42 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc7b2b0a23499f600af7797e9f6573fda39eff6aa51d1136e7d833028df6648`  
		Last Modified: Wed, 19 Jan 2022 17:50:45 GMT  
		Size: 6.7 MB (6713854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0819ae565b7a76ba7b29d7f603f3fdfa82c1cd36d65da84ab4bb1e9f9ab2d419`  
		Last Modified: Wed, 19 Jan 2022 17:50:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
