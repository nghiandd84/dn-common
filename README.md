# dn-common
Common library

## Step to create library
1. Create account on https://issues.sonatype.org/
2. Create issue ticket and waiting for approval 
  - Type NewProject
  - GroupId io.github.nghiandd84
  - ....
3. Install GNUPG tool at https://gnupg.org/download/
4. Create secret phrase "gpg --gen-key"
5. Send secret key 
  - gpg --keyserver http://keyserver.ubuntu.com:11371 --send-keys 58cc20651b2c0b0f"
  - gpg --keyserver http://keys.openpgp.org:11371 --send-keys 58cc20651b2c0b0f
6. Build deploy: mvn clean deploy -P release
# Use common-core
```xml
<dependency>
    <groupId>io.github.nghiandd84</groupId>
    <artifactId>common-core</artifactId>
    <version>0.0.1</version>
</dependency>
```
 