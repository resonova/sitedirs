# sitedirs.sh

## Repository Resource Links

Github Repository: [github.com/resonova/sitedirs](https://github.com/resonova/sitedirs)

View Live README Page: [README.md](https://resonova.github.io/sitedirs)

Example 'go-back' Page: [sitedirs/a/index.html](https://resonova.github.io/sitedirs/docs/sitedirs/a/index.html)

Download _sitedirs.zip_ Directories and Files (.zip): [sitedirs.zip](https://raw.githubusercontent.com/resonova/sitedirs/master/sitedirs.zip)

Download _sitedirs.sh_ Bash Script (.sh): [sitedirs.sh](https://raw.githubusercontent.com/resonova/sitedirs/master/sitedirs.sh)

## Introduction

The `sitedirs.sh` bash shell script is an alphabetic and numeric site directory creation script. It outputs directories of the following two groups:

> 1) Letters - (a-z)
> 2) Numbers - (0-9)

All directories that are generated by this script are automatically filled with a single `index.html` file which is pre-configured to serve as a _go-back_ redirect page (which sends viewers to the previous location stored in their browser history).

## Installation and Usage

After downloading or cloning this repository, simply navigate to the directory containing `sitedirs.sh` (the base directory). You can obtain the core shell script directly with:

```wget -q 'https://raw.githubusercontent.com/resonova/sitedirs/master/sitedirs.sh'```

Enable script execution with the following:

```sudo chmod +x sitedirs.sh```

Run the script to generate the full list of files and directories:

```./sitedirs.sh```

You can also skip the need to run the `sitedirs.sh` script by downloading the zipped file which contains the full output of the script at the following location: [sitedirs.zip](https://raw.githubusercontent.com/resonova/sitedirs/master/sitedirs.zip)

Alternatively, you can `wget` the zipped file via the command line with:

```wget -q 'https://raw.githubusercontent.com/resonova/sitedirs/master/sitedirs.zip'```

## index.html Source Code

The index.html files that are created with the `sitedirs.sh` script are generated from base64 encoded strings to preserve the integrity of the final output. The shell script performs the decoding automatically and outputs the following resultant HTML code into every index.html file:


```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>GO BACK</title>
</head><!-- Automatic redirection -->
<body onload="go Back()"><br>
    <p>This page perfporms an intentional redirection.</p><br>
    <script>
        function goBack() {
            window.history.back();
        }
    </script>
</body>
</html>
```

The encoded variable assignments in `sitedirs.sh` that are used to generate the above HTML are as follows:

```
ht_01='PCFET0NUWVBFIGh0bWw+PGh0bWwgbGFuZz0iZW4iPjxoZWFkPg=='
ht_02='PG1ldGEgaHR0cC1lcXVpdj0iQ29udGVudC1UeXBlIiBjb250ZW50PSJ0ZXh0L2h0bWw7IGNoYXJzZXQ9dXRmLTgiPg=='
ht_03='PG1ldGEgbmFtZT0idmlld3BvcnQiIGNvbnRlbnQ9IndpZHRoPWRldmljZS13aWR0aCwgaW5pdGlhbC1zY2FsZT0xLjAiPg=='
ht_04='PG1ldGEgaHR0cC1lcXVpdj0iWC1VQS1Db21wYXRpYmxlIiBjb250ZW50PSJJRT1lZGdlIj4='
ht_05='PHRpdGxlPkdPIEJBQ0s8L3RpdGxlPjwvaGVhZD4='
ht_06='PCEtLSBBdXRvbWF0aWMgcmVkaXJlY3Rpb24gLS0+PGJvZHkgb25sb2FkPSJnb0JhY2soKSI+'
ht_07='PGJyPjxwPlRoaXMgcGFnZSBwZXJmcG9ybXMgYW4gaW50ZW50aW9uYWwgcmVkaXJlY3Rpb24uPC9wPjxicj4='
ht_08='PHNjcmlwdD5mdW5jdGlvbiBnb0JhY2soKSB7d2luZG93Lmhpc3RvcnkuYmFjaygpO308L3NjcmlwdD4='
ht_09='PC9ib2R5PjwvaHRtbD4='
html_part1=( "${ht_01}" "${ht_02}" "${ht_03}" "${ht_04}" "${ht_05}" )
html_part2=( "${ht_06}" "${ht_07}" "${ht_08}" "${ht_09}" )
html_core=( $(echo ${html_part1[@]} ${html_part2[@]}) )
```


## Directory Tree

The following directory tree is an exhaustive listing of all files and directories that are generated by `sitedirs.sh`:
```
.
├── 0
│   └── index.html
├── 1
│   └── index.html
├── 2
│   └── index.html
├── 3
│   └── index.html
├── 4
│   └── index.html
├── 5
│   └── index.html
├── 6
│   └── index.html
├── 7
│   └── index.html
├── 8
│   └── index.html
├── 9
│   └── index.html
├── a
│   └── index.html
├── b
│   └── index.html
├── c
│   └── index.html
├── d
│   └── index.html
├── e
│   └── index.html
├── f
│   └── index.html
├── g
│   └── index.html
├── h
│   └── index.html
├── i
│   └── index.html
├── j
│   └── index.html
├── k
│   └── index.html
├── l
│   └── index.html
├── m
│   └── index.html
├── n
│   └── index.html
├── o
│   └── index.html
├── p
│   └── index.html
├── q
│   └── index.html
├── r
│   └── index.html
├── s
│   └── index.html
├── t
│   └── index.html
├── u
│   └── index.html
├── v
│   └── index.html
├── w
│   └── index.html
├── x
│   └── index.html
├── y
│   └── index.html
└── z
    └── index.html

36 directories, 36 files
```
