# Page Load Started

### Page Load Started is part of the page load sequence, including virtual page loads in the case of single page apps, and must be the first event pushed in the page load event sequence.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Load Started",
    "page": {
        "AAMURLCookieID": "<AAMURLCookieID>",
        "baseURL": "<baseURL>",
        "channel": "<channel>",
        "navigationPath": "<navigationPath>",
        "pageName": "<pageName>",
        "pcPlatformSelection": "<pcPlatformSelection>",
        "siteAudience": "<siteAudience>",
        "siteCountry": "<siteCountry>",
        "siteLanguage": "<siteLanguage>",
        "siteSection1": "<siteSection1>",
        "siteSection2": "<siteSection2>",
        "siteSection3": "<siteSection3>",
        "siteSection4": "<siteSection4>",
        "webPageType": "<webPageType>",
        "workfrontID": "<workfrontID>"
    },
    "user": {
        "advisorId": "<advisorId>",
        "dealerCode": "<dealerCode>",
        "institutionalID": "<institutionalID>",
        "institutionalPartyId": "<institutionalPartyId>",
        "investorId": "<investorId>",
        "investorPartyId": "<investorPartyId>",
        "partyId": "<partyId>",
        "pcsSfmcId": "<pcsSfmcId>",
        "personaSegment": "<personaSegment>",
        "personalizedExperienceType": "<personalizedExperienceType>",
        "planICU": "<planICU>",
        "planId": "<planId>",
        "planParticipantId": "<planParticipantId>",
        "planType": "<planType>",
        "toolAdvisorId": "<toolAdvisorId>",
        "toolPartyId": "<toolPartyId>",
        "tracSponsorId": "<tracSponsorId>",
        "tracTPAId": "<tracTPAId>",
        "userInitials": "<userInitials>",
        "userRole": "<userRole>",
        "visionId": "<visionId>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page.AAMURLCookieID|string|Capture AAM URL Cookie ID||||||||
|page.baseURL|string|Captures the URL of the page after removing any parameters. This value can't be null and should start with Protocol \(http\/https\).|https:\/\/www.icanretire.com, https:\/\/www.capitalgroup.com\/advisor\/insights\/categories\/outlook.html|^(http[s]?:\/\/)([a-z]{1,256})([\/a-z]{1,256}[^?||@&$#=]+)$||||||
|page.channel|string|Custom value for s.channel. This value can't be null and not contain any numeric values|icanretire, Capital Group - advisor, Capital Group - individual|||||||
|page.navigationPath|string|Captures the name of the menu, panel, navigation bar , breadcrumb, breadcrumb, etc. used to navigate the site. Value should be alphbetic. E.g. Global Navigation, Footer, Breadcrumb. NULL values means no navigation was used to get on the page.|Global Navigation, Footer, Primary Navigation, Breadcrumb, Sub Navigation Menu, Primary Navigation \(small breakpoint\), Left Rail, Left navigation, Right Rail, Footer Navigation|||||||
|page.pageName|string|Custom value for the name of the page. It is inline with the page URL, with its value usually being the latest 2 path levels of the URL separated by a '&gt;'. This value can't be null or \#. This value can be alphanumeric and can contain different symbols. E.g. accounts &gt; Portfolio, rsa-existing-user &gt; Step 1a: RSA Existing User - Enter Your Login Credentials, advisor &gt; Home, literature &gt; Search results, what-we-offer &gt; Mutual funds - American Funds|accounts &gt; Portfolio, rsa-existing-user &gt; Step 1a: RSA Existing User - Enter Your Login Credentials, advisor &gt; Home, literature &gt; Search results, what-we-offer &gt; Mutual funds - American Funds|||||||
|page.pcPlatformSelection|string|What is platform selection that used for accessing pcon?||||||||
|page.siteAudience|string|Populates the built-in s.server variable with site audience \(custom usage\)||||||||
|page.siteCountry|string|Indicates the primary country served by the site. ISO 3166 \(alpha-2\) Uppercase. This value cant be null|US, CA, FR, UK|^[a-zA-Z]{2}$||||||
|page.siteLanguage|string|Language in which the site is presented ISO 639-1 code. This value cant be null|en-us, en-gb, ch-cn, fr-ca, fr-fr, da|^[a-z]{2}([-]{1}[a-z]{2}){0,1}$||||||
|page.siteSection1|string|The site section portion of the page details. This value can't be null or '\#' and value can be alphanumeric or symbol. Site Level 1, i.e, Home, Insights, About Us, etc|Home, About Us, Service &amp; Support, Insights|||||||
|page.siteSection2|string|Subsection of the page being viewed. This value can be alphanumeric and can contain different symbols. NULL values means page does not have a Site Level 2 hierarchy. E.g., Section Index, Service &amp; Support, MY ACCOUNTS, CLIENTACCOUNTS, Investments|Section Index, Service &amp; Support, MY ACCOUNTS, CLIENTACCOUNTS, Investments|||||||
|page.siteSection3|string|Sub-subsection level for the given page. This value can be alphanumeric and can contain different symbols. NULL values means page does not have a Site Level 3 hierarchy. E.g., Section Index, Login, Portfolio, Environmental&Social and Governance \(ESG\)|Section Index, Login, Portfolio, Environmental&amp;\#44; Social and Governance \(ESG\)|||||||
|page.siteSection4|string|Level below sub-subsection of the given page. This value can be alphanumeric and can contain different symbols. NULL values means page does not have a Site Level 4 hierarchy. E.g., Section Index, Transactions, Our approach to ESG integration, RSA Existing User|Section Index, Transactions, Our approach to ESG integration, RSA Existing User|||||||
|page.webPageType|string|Webpage Type such as AEM, SPA, JavaStack, Third Party, Other|AEM, SPA, JavaStack, ThirdParty, Other|||||||
|page.workfrontID|string|WorkfrontID from page properties||||||||
|user.advisorId|string|Captures the Advisor ID asssociated with user activity. This value can only contain numeric value or invalid. 0 or NULL values means Advisor did not login|6599296, 7900290|||||||
|user.dealerCode|string|Capture Dealer code for Canada Advisor Soft Login|9000, 9190, 9844, 9280, 99999|||||||
|user.institutionalID|string|Captures the ID used to login to the institutional site. Values should only be numeric or invalid. 0 or NULL values means user did not login|32066, 38830|||||||
|user.institutionalPartyId|string|Institutional Party ID associated with the user accessing the site||||||||
|user.investorId|string|Captures the unique ID that the investor used to access the site. This value can only contain numeric value or invalid. 0 or NULL values means Investor did not login|443009423362019 , 445366008521402|||||||
|user.investorPartyId|string|Investor Party ID associated with the user accessing the site||||||||
|user.partyId|string|Capture the party ID associated with the user accessing the site. This Value should only be numeric, or Invalid. E.g. 8844784, 526891, 7205090. 0 or NULL values means user did not login|8844784, 526891, 7205090|||||||
|user.pcsSfmcId|string|SFMC ID associated with the user login ID||||||||
|user.personaSegment|string|User persona from the quiz if applicable, else an empty string|g, o, j, k, s|||||||
|user.personalizedExperienceType|string|PersonalizedExperienceType|MS, GA, RIA|||||||
|user.planICU|string|What is the Plan ICU associated with the user accessing the site?|1,2,2000|||||||
|user.planId|string|Captures the Plan ID associated with user activity|1351294-01,1351294-02|||||||
|user.planParticipantId|string|The plan participant ID of the user accessing the site. Value should be alphanumeric & can contain special characters \(-\). E.g. CMS, IRK165195-3, IRK140829-14. 0 or NULL values means user did not login|CMS, IRK165195-3, IRK140829-14|||||||
|user.planType|string|Captures the Plan Type associated with user activity|403B|||||||
|user.toolAdvisorId|string|Tool Advisor ID associated with the user accessing the site||||||||
|user.toolPartyId|string|Tool Party ID associated with the user accessing the site|531361,87163|||||||
|user.tracSponsorId|string|Captures the sponsor ID associated with the user accessing the site. This value can be alphanumeric, and can contain special characters \(-,\_,space\). 0 or NULL values means Sponsor did not login|CMS, PSW00001, SLOCKE22, QRPS401K, PSW10821|||||||
|user.tracTPAId|string|Captures the TPA ID associated with user activity. This value can only contain numeric value or invalid. 0 or NULL values means TPA did not login||||||||
|user.userInitials|string|Captures CG user Initials|VQQB,FZBB|||||||
|user.userRole|string|Capture the “User Role” associated with the user accessing the site.|TPA, Sponsor|||||||
|user.visionId|string|Captures the Vision ID of the user accessing the site. Value should be alphanumeric and starts with ", and end with ==".  0 or NULL values means Advisor did not login. E.g. "robZrllGwupTfPLQGkvP9Q==", "feKGIlqj7fbh03wEwx56AQ==", "EU42kZDJlnEYBt0p0v+ofA=="|"robZrllGwupTfPLQGkvP9Q==", "feKGIlqj7fbh03wEwx56AQ==", "EU42kZDJlnEYBt0p0v+ofA=="|||||||

## Attached Notes

<p>This event captures analytics of the entire page that is loaded</p>
