---
title: "callRecord: getSmsLog"
description: "Get log of sent/received SMS"
author: "radoslag"
ms.localizationpriority: medium
ms.prod: "cloud-communications"
doc_type: apiPageType
---

# callRecord: getSmsLog
Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get log of sent/received SMS as a collection of [smsLogRow](../resources/callrecords-smslogrow.md) entries.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)| Not supported. |
|Delegated (personal Microsoft account)| Not supported. |
|Application| CallRecord-PstnCalls.Read.All, CallRecords.Read.All |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /communications/callRecords/getSmsLog
```

## Function parameters

In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|fromDateTime|DateTimeOffset|Start of time range to query. UTC, inclusive.|
|toDateTime|DateTimeOffset|End of time range to query. UTC, inclusive.|

> [!IMPORTANT]
> The **fromDateTime** and **toDateTime** values cannot be more than a date range of 90 days.

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body

Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a collection of [smsLogRow](../resources/callrecords-smslogrow.md) entries in the response body.
  
If there are more than 1000 entries in the date range, the body also includes an `@odata.NextLink` with a URL to query the next page of entries. The last page in the date range does not have `@odata.NextLink`. For more information, see [paging Microsoft Graph data in your app](/graph/paging).

## Example

The following example shows how to get the log of sent/received SMS that occurred in the specified date range. The response includes `"@odata.count": 1000` to enumerate the number of records in this first response, and `@odata.NextLink` to get records beyond the first 1000. For readability, the response shows only a collection of 1 record. Please assume there are more than 1000 records in that date range.

### Request

The following is an example of a request:
<!-- {
  "blockType": "request",
  "name": "callrecordthis.getsmslog"
}
-->
``` http
GET https://graph.microsoft.com/beta/communications/callRecords/getSmsLog(fromDateTime=2022-11-01,toDateTime=2022-12-01)
```

[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

### Response

The following is an example of the response:
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.callRecords.smsLogRow)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.callRecords.smsLogRow)",
    "@odata.count": 1000,
    "@odata.nextLink": "https://graph.microsoft.com/beta/communications/callRecords/getSmsLog(fromDateTime=2022-11-01,toDateTime=2022-12-01)?$skip=1000",
    "value": [
        {
            "smsId": "ef36b3e8-9922-4763-90e2-f4345c04a5d6",
            "userId": "19b900af-fe99-48d6-a9a4-b79c995afc33",
            "userPrincipalName": "ruwini.perera@contoso.com",
            "userDisplayName": "Ruwini Perera",
            "userCountryCode": "US",
            "tenantCountryCode": "US",
            "sourceNumber": "+12818602122",
            "destinationNumber": "+12673173004",
            "sentDateTime": "2022-10-06T11:15:48.6113555Z",
            "callCharge": 0.00,
            "currency": "USD",
            "smsType": "sms_in",
            "destinationContext": "Domestic",
            "destinationName": "United States",
            "otherPartyCountryCode": "US",
            "licenseCapability": "MCOSMS1",
            "smsUnits": 1
        }
    ]
}
```

## See also

* [Get log of PSTN calls](callrecords-callrecord-getpstncalls.md)
* [Get log of direct routing calls](callrecords-callrecord-getdirectroutingcalls.md)
* [Get aggregated report of the audio conferencing dial-out](callrecords-callrecord-getpstnonlinemeetingdialoutreport.md)
* [Microsoft Teams PSTN usage report](/microsoftteams/teams-analytics-and-reports/pstn-usage-report)
