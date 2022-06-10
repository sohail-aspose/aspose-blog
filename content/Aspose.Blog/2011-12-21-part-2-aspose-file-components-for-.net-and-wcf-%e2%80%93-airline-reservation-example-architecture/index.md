---
title: 'Part 2: Aspose File Components for .NET and WCF – Airline Reservation Example Architecture'
date: Wed, 21 Dec 2011 18:35:36 +0000
draft: false
url: /2011/12/21/part-2-aspose-file-components-for-.net-and-wcf-%e2%80%93-airline-reservation-example-architecture/
author: Shahzad Latif
summary: ''
tags: ['Shahzad Latif', '.NET', 'Aspose', 'Aspose.Total for .NET', 'Excel', 'Invoice', 'PDF', 'Print', 'Ticket', 'WCF', 'email']
categories: ['Aspose.Total Product Family']
---



{{< figure align=center src="images/aspose-Total.png" alt="Aspose.Total icon">}}


[Aspose.Total for .NET][1] can be used in a variety of scenarios and with many different technologies and applications. In this series, we're looking into the airline reservation scenario. We're building a small application based on WCF, Windows Forms, and a few Aspose components for file manipulation. This is the second part of the series. You may have a look into the first part at the following URL: [Part 1: Aspose File Components for .NET and WCF – Airline Reservation Example Scenario][2].

In this second part of the series, we'll have a look into the application architecture and the different parts of the application. We'll see how these parts come together to build a service for creating the airline ticket and sending it to the customer via email.

## Airline Reservation Service

We'll build a simple [WCF service][3] that will allow the booking agents to get the flight information, using a client application, based upon the customer's reservation criteria, and then reserve the seats.

In the following class diagram, you can see a service contract named "IBookingService". We have created a class named "BookingService" based on the above service contract. This class provides two methods: GetFlightInfo and BookFlight. We have also defined a couple of data contracts: FlightInfo, PassengerInfo, and BookingInfo to pass the data back and forth between the service and the client.

As we also need to add the features to create the ticket in PDF format and then send it to the customer via email, we're going to use [Aspose file format components][4] to handle file manipulation and email related tasks. Aspose file manipulation components work perfectly in a WCF service, so we can use them in this application.

We have created a separate class named "AsposeFileManager" to work with files. This class will contain all the Aspose related code like [creating bar codes using Aspose.BarCode for .NET][5], [generating ticket in PDF format using Aspose.Pdf for .NET][6], [saving flight and passenger information in Excel format using Aspose.Cells for .NET][7], and [sending ticket to the customer via email using Aspose.Email for .NET][8].



{{< figure align=center src="images/FlyNow-Airline-Reservation-Booking-Service.png" alt="Airline Reservation Service">}}


**Airline Reservation Service - Class Diagram  
**

## Airline Reservation Client

On the client end, we'll use [Windows Forms][9] to build the application which will consume the above reservation service. The booking agent will be able to find the flight information and book the seat for the customer. In addition to that, the agent will be able to print an invoice for the customer. We'll use [Aspose.PDF for .NET to create the invoice in the PDF format and then send it to the printer][10].

## What's Next?

In the next post, I'll share the actual code with you so you could see what's going on inside the service and how we're manipulating the files in this WCF based service. You'll also be able to download the sample application, so you could run and test it at your end.




[1]: https://products.aspose.com/total/net
[2]: https://blog.aspose.com/2011/12/15/part-1-aspose-file-components-and-wcf-airline-reservation-example-scenario/
[3]: http://msdn.microsoft.com/en-us/library/ms731082.aspx
[4]: http://www.aspose.com/
[5]: https://products.aspose.com/barcode/net
[6]: https://products.aspose.com/pdf/net
[7]: https://products.aspose.com/cells/net
[8]: https://downloads.aspose.com/pdf
[9]: http://en.wikipedia.org/wiki/Windows_Forms
[10]: https://products.aspose.com/pdf/net




