---
description: "Automatically generated file. DO NOT MODIFY"
---
<!-- markdownlint-disable MD041 -->

```java
GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingAppointment bookingAppointment = new BookingAppointment();
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2018-05-06T08:30:00-04:00";
end.timeZone = "UTC";
bookingAppointment.end = end;
DateTimeTimeZone invoiceDate = new DateTimeTimeZone();
invoiceDate.dateTime = "2018-05-06T08:30:00-04:00";
invoiceDate.timeZone = "UTC";
bookingAppointment.invoiceDate = invoiceDate;
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2018-05-06T08:00:00-04:00";
start.timeZone = "UTC";
bookingAppointment.start = start;

graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").appointments("AAMkADKnAAA=")
    .buildRequest()
    .patch(bookingAppointment);
```
