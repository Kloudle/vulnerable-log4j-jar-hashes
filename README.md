# Vulnerable log4j JAR Hashes

The repository contains a CSV file with names of log4j JAR files along with their SHA1 hashes for each version that is known to be vulnerable.

## Evaluating if a log4j JAR is vulnerable

1. Calculate the `SHA1` sum for the file
    * Linux: `sha1sum <path/to/file>`
    * Windows (in Powershell): `get-filehash -Algorithm SHA1 <path\to\file>`
    * Mac: `shasum </path/to/file>`

2. Check if the hash generated in step 1 exists in [log4j-vuln-versions-sha1sum.csv](log4j-vuln-versions-sha1sum.csv)
3. If the hash exists, the log4j JAR is a vulnerable version
