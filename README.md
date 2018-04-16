# kyozetsu
Automatic creation of nginx block scripts based on ASN data.

# Usage
## From the command line...
```
perl6 kyozetsu.p6 [ASN] [OPTIONS]
```

## `-o`, `--output`
Specify the output file to which the blocklist is saved. Defaults to `/etc/nginx/conf.d/blocklists/{ASN_NUNBER}.asn`. This directory must already exist, or the script will fail to write the file.

## `-r`, `--reload`
Trigger nginx to automatically reload the configuration after writing to the new blocklist file. Your user account must have permission to do this otherwise it will fail.
