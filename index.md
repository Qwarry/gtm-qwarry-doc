## Qwarry GTM tags

### Qwarry ID persistence tag

This tag is part of a Qwarry conversion attribution mechanism. Its main purpose is to provide an easy way to persist the Qwarry ID contained in the url query parameters to the localStorage.

This way, the Qwarry ID remains accessible even after a user navigates through multiple pages (which is probably the case if you have a multi-steps form basket view to payment, for instance). Indeed, when a next page is loaded, the URL is refreshed and the Qwarry ID, that was initially present, is now definitively lost and no conversion attribution can be done afterwards.

#### When should I trigger this tag ?

This tag is designed to be triggered on the target landing page of an advertisement, but you can safely use it on all your pages.

### Qwarry Conversion tag

This tag can be used for 2 main purposes independently. You can use it as a visit tag or as a conversion tag.

#### Visit tag usage

Using this tag for a visit purpose is the simplest. Just use it standalone, without configuring the previous one (see Qwarry ID persistence tag), since you probably just want to postback on landing.

##### Configuration

1. On the "*How do you want to use this tag ?*" question, leave the default selected radio box "*As a visit tag*"
2. Choose your preferred way to postback (*Pixel* or *Hidden iframe*)
3. As a Qwarry client, you should have been granted an *Advertiser tag ID*
4. You can leave the default value for *Custom value* if no additional information was given from the Qwarry AdOps team

#### Conversion tag usage

Using this tag is a bit more complex as it requires setting up the Qwarry ID persistence tag first (see Qwarry ID persistence tag). Doing this makes the Qwarry ID available all your website wide. You can now make the attribution at the end of a conversion funnel because the ID is made available after a multiple pages navigation.

##### Configuration

1. On the "*How do you want to use this tag ?*" question, select the radio box "*As a conversion tag*"
2. Choose your preferred way to postback (*Pixel* or *Hidden iframe*)
3. As a Qwarry client, you should have been granted an *Advertiser tag ID*
4. You can leave the default value for *Custom value* if no additional information was given from the Qwarry AdOps team
5. Choose your preferred *Conversion postclick attribution* duration. This value represents the duration under which the conversion is attributed to Qwarry.
