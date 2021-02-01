## `python:3-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:40fc30607aa125f60d1f721bcc256c9817aa1efe351dda924cdaf916d6de6935
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `python:3-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull python@sha256:4fefbcb01b8ba9a05d95605d762573e83d43aa23071ef58f09e34343597eac93
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5869210247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31b4d828b55c88ec2d796f7a7b6e5f045e564e5339f8e54df31e8793e96f9b99`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 19:15:14 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 13 Jan 2021 19:22:23 GMT
ENV PYTHON_VERSION=3.9.1
# Wed, 13 Jan 2021 19:22:24 GMT
ENV PYTHON_RELEASE=3.9.1
# Wed, 13 Jan 2021 19:24:43 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	Start-Process python.exe -Wait 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		); 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 		Write-Host 'Complete.'
# Mon, 01 Feb 2021 22:17:42 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 01 Feb 2021 22:17:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/4be3fe44ad9dedc028629ed1497052d65d281b8e/get-pip.py
# Mon, 01 Feb 2021 22:17:43 GMT
ENV PYTHON_GET_PIP_SHA256=8006625804f55e1bd99ad4214fd07082fee27a1c35945648a58f9087a714e9d4
# Mon, 01 Feb 2021 22:19:23 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 01 Feb 2021 22:19:24 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036493f24213085956c7e7402a5d91f9c1e8e833f024c212f39aee0efbe03044`  
		Last Modified: Wed, 13 Jan 2021 19:42:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679e7ec4280ddcfabb9914410e1910ab950e28cc3bdb33737372248ff4aa2ecc`  
		Last Modified: Wed, 13 Jan 2021 19:43:38 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3747de3aa3863e73274dcc83fe0b7892f33dbf5b7c665254090b9bbd4edc72`  
		Last Modified: Wed, 13 Jan 2021 19:43:37 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1e0d1ee23d5c3f5af33b4ebdfec535b9d8d1e560882cccdc4bcfca235a47d5`  
		Last Modified: Wed, 13 Jan 2021 19:43:46 GMT  
		Size: 59.6 MB (59618831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a827251eae5fb5698eb08deb1423de9f54c2d6945e7c43b8a8803635f3cd7d`  
		Last Modified: Mon, 01 Feb 2021 22:26:59 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559fe22b7290090c0c7fe82207650ae9bb0b5e77ce067988b8ccad1409024f5b`  
		Last Modified: Mon, 01 Feb 2021 22:26:59 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5fd9ffb626600a43c1b4a1b56aae53760aff8b9f72a9d69527d6af7e57ee4f`  
		Last Modified: Mon, 01 Feb 2021 22:26:59 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231679079cf1ca6afeebfbb849be5f3dd49913e2bdd2807cd55052a2098f57a5`  
		Last Modified: Mon, 01 Feb 2021 22:27:03 GMT  
		Size: 15.7 MB (15687348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb903ac86c504938cc5dac625ebd7274bb938f042000a5a97ae62d7cead1600f`  
		Last Modified: Mon, 01 Feb 2021 22:27:00 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
