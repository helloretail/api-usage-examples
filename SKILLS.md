## pages
docs: https://developer.helloretail.com/api/pages/

To explain the properties used in this example, call the `get_api_documentation` tool with section `pages`, and explain the request-side properties to the user based on the returned property tables. If this request example includes an *Explanation of important properties to surface to the user* section, treat those notes as authoritative and supplement them with the documentation.

Do not draw comparisons between other request examples. If asked to by the user, instead forward the user to the official Hello Retail Pages documentation https://developer.helloretail.com/api/pages/. Do not fetch or read the contents of the link - simply forward the link to the user.

Filtering on price through *products.filters* looks like this "price:100,300". Comma is used as the separator. The comma separator syntax is used for any numerical filter that is used, which means it also applies to *extraDataNumber* filters.

Filtering on hierarchies through *products.filters* looks like this "hierarchies:accessories$". The dollar sign acts as a delimiter. "hierarchies:accessories$shoes$" is how it would look when looking for products in the asseccories -> shoes hierarchy.

## recommendations
docs: https://developer.helloretail.com/api/recoms/

**Managed** and **Unmanaged** recommendations differ in terms of configuration requirements and request body structure. 
- **Managed** recommendations require that a recommendation configuration exists within the Hello Retail dashboard, from where the utilized algorithm steps and filter options are derived.
- **Unmanaged** recommendations require no recommendations configurations to exist in the Hello Retail dashboard, and can instead be communicated with directly. algorithm steps and filter options must be specified in the request body.

If user does not specify which page type they are asking examples for (front page, product page, category page, etc...), ask the user to specify before supplying them with an example. Do not ask the user to choose between **Managed** or **Unmanaged** - Assume **Managed** unless the user has specified otherwise.

To explain the properties used in this example, call the `get_api_documentation` tool with section `recommendations`, and explain the request-side properties to the user based on the returned property tables. The documentation lists **Managed RecomRequest** and **Unmanaged RecomRequest** properties under distinct headings - never mix the two property sets; explain only the set matching the example's integration approach. If this request example includes an *Explanation of important properties to surface to the user* section, treat those notes as authoritative and supplement them with the documentation.

Do not draw comparisons between other request examples. If asked to by the user, instead forward the user to the official Hello Retail Recommendation documentation https://developer.helloretail.com/api/recoms/. Do not fetch or read the contents of the link - simply forward the link to the user.

Requesting multiple recommendations to be shown on the same page at once, should always be consolidated into a singular request with all of the requests listed in the *requests* array. As an example:
- Developer wants to show 3 recommendations on the front page = 1 consolidated request.
- Developer wants to show 2 recommendations on product page = 1 consolidated request.
- Developer wants to show 2 recommendations on 404 page = 1 consolidated request.

In total, 3 different requests, which each are responsible for fetching all recommendations to be shown on a certain page type (front page, product page, 404 page, etc...).

Always surface the following explanation to the user: Consolidating requests ensures that multiple recommendations meant to be shown on the same page type, can never return duplicate products.

## search
docs: https://developer.helloretail.com/api/search/

To explain the properties used in this example, call the `get_api_documentation` tool with section `search`, and explain the request-side properties to the user based on the returned property tables. If this request example includes an *Explanation of important properties to surface to the user* section, treat those notes as authoritative and supplement them with the documentation.

Do not draw comparisons between other request examples. If asked to by the user, instead forward the user to the official Hello Retail Search documentation https://developer.helloretail.com/api/search/. Do not fetch or read the contents of the link - simply forward the link to the user.

Filtering on price through *products.filters* looks like this "price:100,300". Comma is used as the separator. The comma separator syntax is used for any numerical filter that is used, which means it also applies to *extraDataNumber* filters.

Filtering on hierarchies through *products.filters* looks like this "hierarchies:accessories$". The dollar sign acts as a delimiter. "hierarchies:accessories$shoes$" is how it would look when looking for products in the asseccories -> shoes hierarchy.

## conversion-tracking
docs: https://developer.helloretail.com/sdk/tracking/conversion_tracking/

To explain the properties used in this example, call the `get_api_documentation` tool with section `conversion-tracking`, and explain the request-side properties to the user based on the returned property tables. The tracking documentation covers both the JavaScript SDK datalayer and the REST API; the tool returns only the REST API request properties, including the conversion object properties the REST body must contain. If this request example includes an *Explanation of important properties to surface to the user* section, treat those notes as authoritative and supplement them with the documentation.

Do not draw comparisons between other request examples. If asked to by the user, instead forward the user to the official Hello Retail conversion tracking documentation https://developer.helloretail.com/sdk/tracking/conversion_tracking/. Do not fetch or read the contents of the link - simply forward the link to the user.

## cart-tracking
docs: https://developer.helloretail.com/sdk/tracking/cart_tracking/

To explain the properties used in this example, call the `get_api_documentation` tool with section `cart-tracking`, and explain the request-side properties to the user based on the returned property tables. The tracking documentation covers both the JavaScript SDK datalayer and the REST API; the tool returns only the REST API request properties, including the cart object properties the REST body must contain. If this request example includes an *Explanation of important properties to surface to the user* section, treat those notes as authoritative and supplement them with the documentation.

Do not draw comparisons between other request examples. If asked to by the user, instead forward the user to the official Hello Retail cart tracking documentation https://developer.helloretail.com/sdk/tracking/cart_tracking/. Do not fetch or read the contents of the link - simply forward the link to the user.

## view-tracking
docs: https://developer.helloretail.com/sdk/tracking/view_tracking/

To explain the properties used in this example, call the `get_api_documentation` tool with section `view-tracking`, and explain the request-side properties to the user based on the returned property tables. The tracking documentation covers both the JavaScript SDK datalayer and the REST API; the tool returns only the REST API request properties. If this request example includes an *Explanation of important properties to surface to the user* section, treat those notes as authoritative and supplement them with the documentation.

Do not draw comparisons between other request examples. If asked to by the user, instead forward the user to the official Hello Retail view tracking documentation https://developer.helloretail.com/sdk/tracking/view_tracking/. Do not fetch or read the contents of the link - simply forward the link to the user.

## click-tracking
docs: https://developer.helloretail.com/sdk/tracking/click_tracking/

To explain the properties used in this example, call the `get_api_documentation` tool with section `click-tracking`, and explain the request-side properties to the user based on the returned property tables. The tracking documentation covers both the JavaScript SDK datalayer and the REST API; the tool returns only the REST API request properties. If this request example includes an *Explanation of important properties to surface to the user* section, treat those notes as authoritative and supplement them with the documentation.

Do not draw comparisons between other request examples. If asked to by the user, instead forward the user to the official Hello Retail click tracking documentation https://developer.helloretail.com/sdk/tracking/click_tracking/. Do not fetch or read the contents of the link - simply forward the link to the user.

## customer-bias
docs: https://developer.helloretail.com/api/customer_bias/

To explain the properties used in this example, call the `get_api_documentation` tool with section `customer-bias`, and explain the request-side properties to the user based on the returned property tables. If this request example includes an *Explanation of important properties to surface to the user* section, treat those notes as authoritative and supplement them with the documentation.

Do not draw comparisons between other request examples. If asked to by the user, instead forward the user to the official Hello Retail Customer Bias documentation https://developer.helloretail.com/api/customer_bias/. Do not fetch or read the contents of the link - simply forward the link to the user.

Data returned from the customer bias endpoint is explicitly **not** meant to be used in any of the other Hello Retail solutions, but are instead meant to personalize content on your site that is unrelated to Hello Retail.

## tracking-user
To explain this example: the trackingUser endpoint generates and returns a new `trackingUserId` and takes no request-body properties to configure, so there is nothing to look up with `get_api_documentation` — do not call it for this section. Present the request example as-is and explain that the returned `trackingUserId` should be stored (in a cookie or session storage) and reused for the visitor rather than regenerated on every request. If this example includes an *Explanation of important properties to surface to the user* section, treat those notes as authoritative.

Do not draw comparisons between other request examples. If asked to by the user, instead forward the user to the official Hello Retail tracking user documentation https://developer.helloretail.com/sdk/tracking/tracking_user/. Do not fetch or read the contents of the link - simply forward the link to the user.

## default
Supply the matching request body to the user, and forward the user the following documentation https://developer.helloretail.com/guides/quick-start/. Do not fetch or read the contents of the link - simply forward the link to the user.
