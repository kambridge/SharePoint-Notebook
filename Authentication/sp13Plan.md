##[Plan for user authentication methods in SharePoint 2013](https://technet.microsoft.com/en-us/library/cc262350.aspx#cba)

###Claims-based authentication
User obtains a digitally signed security token from a commonly trusted identity provider.  The token contains a set of claims. Each claim represents a specific item of data about a user such as his or her name, group memberships, and role on the network.  Applications that support claims-based authentication obtain a security token from a user, rather than credentials, and use the information within the claims to determine access to resources. No separate query to a directory service such as AD DS is needed.

When you use claims-based authentication, all supported authentication methods are available for your web applications and you can take advantage of new features and scenarios in SharePoint 2013 that use server-to-server authentication and app authentication.

> For claims-based authentication, SharePoint 2013 automatically changes all user accounts to claims identities.

_References:_
 - _[Claims-based Identity for Windows (white paper)](http://go.microsoft.com/fwlink/p/?LinkId=198942)_
