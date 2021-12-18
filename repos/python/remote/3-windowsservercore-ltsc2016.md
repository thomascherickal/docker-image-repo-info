## `python:3-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:a3a1f982f13f5f0cdcf06b9f16308f50310b9e83068c8f163818a3c4d99026aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4825; amd64

### `python:3-windowsservercore-ltsc2016` - windows version 10.0.14393.4825; amd64

```console
$ docker pull python@sha256:a5292ca15ff16d8b59da90b4bbfe6faa50e3cf95abf1d462682d8795f88f60fd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6332013193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd33397f0c4458c9a37d12ad5638b76a986049698bf6b67fde54a5c5d91c8e69`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 00:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 18 Dec 2021 04:51:29 GMT
ENV PYTHONIOENCODING=UTF-8
# Sat, 18 Dec 2021 04:51:30 GMT
ENV PYTHON_VERSION=3.10.1
# Sat, 18 Dec 2021 04:51:31 GMT
ENV PYTHON_RELEASE=3.10.1
# Sat, 18 Dec 2021 04:53:46 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 04:53:47 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Sat, 18 Dec 2021 04:53:48 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Sat, 18 Dec 2021 04:53:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Sat, 18 Dec 2021 04:53:50 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Sat, 18 Dec 2021 04:55:35 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Sat, 18 Dec 2021 04:55:36 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7756a7a3024dbbb7cabda3151e8f8461ae808ae2ad3857f0c9235c5908ff7695`  
		Last Modified: Sat, 18 Dec 2021 01:22:26 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b032dea64559edddd8d7d51de64c99d62a953cc056d3a265d67caf85bb31e91`  
		Last Modified: Sat, 18 Dec 2021 05:10:59 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c613836f41f0f6d29ed53b7330d2645f037257110151715c72490fe9a07c73`  
		Last Modified: Sat, 18 Dec 2021 05:10:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f96a3bdb9b0f6630cc8f201f383efb0bb40581fb18884a92452d834cc534dfe`  
		Last Modified: Sat, 18 Dec 2021 05:10:57 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aab7a379552fd144ce95401f794206ed41264f1b7bb6166e533eebd2dc6116d`  
		Last Modified: Sat, 18 Dec 2021 05:11:53 GMT  
		Size: 50.8 MB (50836365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec543d622faa4d509208e01302d2fb819cd7e822f05e7031e72eeac3fe72c93`  
		Last Modified: Sat, 18 Dec 2021 05:10:57 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd302f1dfff0f7e7d550f3962db64a5f36765623fa65a0b4bb4bbcfdc4e15b57`  
		Last Modified: Sat, 18 Dec 2021 05:10:55 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20628a6a839fa65417a788f6e11f25da99a2d37a16206ffd9e2a66fa9bc844f6`  
		Last Modified: Sat, 18 Dec 2021 05:10:54 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19e8a777ed491675a710ebbde773378c300e9999fe26a7e3c7918cc1ab5da48`  
		Last Modified: Sat, 18 Dec 2021 05:10:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a9a74bc032c0c93499bd575f9f1cc2ac87fa2b41581d510111ed8deb0b0432`  
		Last Modified: Sat, 18 Dec 2021 05:11:02 GMT  
		Size: 6.4 MB (6449376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f12d8ba0e32cde28e32d88cf709be966c6d9e3499c19f23f4cd4cde5e3c511`  
		Last Modified: Sat, 18 Dec 2021 05:10:54 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
