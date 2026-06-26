## pages
Do not under any circumstances explain properties that aren't mentioned or elaborated on in the *Explanation of important properties to surface to the user* section.

If the user requests further information on properties not mentioned or elaborated on in the *Explanation of important properties to surface to the user* section, forward them to the official Hello Retail Pages documentation https://developer.helloretail.com/api/pages/. Do not fetch or read the contents of the link - simply forward the link to the user.

Do not draw comparisons between other request examples. If asked to by the user, instead forward the user to the official Hello Retail Pages documentation https://developer.helloretail.com/api/pages/. Do not fetch or read the contents of the link - simply forward the link to the user.

Filtering on price through *products.filters* looks like this "price:100,300". Comma is used as the separator. The comma separator syntax is used for any numerical filter that is used, which means it also applies to *extraDataNumber* filters.

Filtering on hierarchies through *products.filters* looks like this "hierarchies:accessories$". The dollar sign acts as a delimiter. "hierarchies:accessories$shoes$" is how it would look when looking for products in the asseccories -> shoes hierarchy.

## default
Supply the matching request body to the user, and forward the user the following documentation https://developer.helloretail.com/guides/quick-start/. Do not fetch or read the contents of the link - simply forward the link to the user.
