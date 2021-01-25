## `python:3-windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:4c07d0b2c4b7779c29949270fb267a36e3931db7ab9e2f01b5250f11f7585146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `python:3-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull python@sha256:ff7e0ace7f240413a3a037c5136c9b3a1ffba872b36ef1ddc862d8bc3901dcd7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5869218168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b37d961a94187ade114fa9e41989747738c027094bed4baa339634f4d8909c7`
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
# Mon, 25 Jan 2021 23:19:32 GMT
ENV PYTHON_PIP_VERSION=21.0
# Mon, 25 Jan 2021 23:19:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/8cc88aca7d9775fce279e8b84ef163cf1d3e8a2e/get-pip.py
# Mon, 25 Jan 2021 23:19:34 GMT
ENV PYTHON_GET_PIP_SHA256=ffb67da2e976f48dd29714fc64812d1ac419eb7d48079737166dd95640d1debd
# Mon, 25 Jan 2021 23:21:31 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 25 Jan 2021 23:21:32 GMT
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
	-	`sha256:f36a139fb681553959597d9691eb4d828fa0a69cd4f350cdf616a3b8a55af93a`  
		Last Modified: Mon, 25 Jan 2021 23:30:10 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75cd0f135a56b626f00daa2b527dbbfee4b32952d4cf79d2adf503bdbc9ee0a9`  
		Last Modified: Mon, 25 Jan 2021 23:30:10 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec0503c428ec14e0477217f99e25ee382deac949ffdabd3aef6c320320eea2`  
		Last Modified: Mon, 25 Jan 2021 23:30:11 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17841041644dcaedf33867b16312d0c3db14f84ef014ab101cfd131f92e3f791`  
		Last Modified: Mon, 25 Jan 2021 23:30:15 GMT  
		Size: 15.7 MB (15695500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a73f27caadd62eeb0fcfbce152b5f427393c71a5bb5bd47e88aeaddf9e2b02a`  
		Last Modified: Mon, 25 Jan 2021 23:30:11 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
