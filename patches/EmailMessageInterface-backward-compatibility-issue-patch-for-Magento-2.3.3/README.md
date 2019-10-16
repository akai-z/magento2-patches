This patch addresses backward compatibility issues that extension developers may have experienced after the introduction of `Magento\Framework\Mail\EmailMessageInterface`, which was released in Magento 2.3.3.  
In the scope of this patch, the new `EmailMessageInterface` inherits from the old MessageInterface, and core modules are changed back to rely on MessageInterface.  
**Merchants should apply this patch as soon as possible, especially if their deployments include extensions or customizations that use the mail interface.**

Affected Magento versions: Magento Commerce and Open Source v2.3.3.

See [the Magento forum DevBlog post](https://community.magento.com/t5/Magento-DevBlog/Backward-incompatible-Changes-in-the-Mail-Library-for-Magento-2/ba-p/144787) for much more information. 
