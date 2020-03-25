This patch addresses a lingering issue created by the fix for [CVE-2019-8118](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2019-8118) (PRODSECBUG-2452) included in Magento 2.3.3 and 2.2.10.

While the fix for that bug stopped the logging of failed login attempts, information collected prior to updating to these current versions may still exist, and previous, unpatched versions of Magento may still have this issue.  
This patch clears the login attempts that were previously collected.  
See [Remove failed login attempts from the database](https://support.magento.com/hc/en-us/articles/360040209352) for information on how to download and install this patch.
