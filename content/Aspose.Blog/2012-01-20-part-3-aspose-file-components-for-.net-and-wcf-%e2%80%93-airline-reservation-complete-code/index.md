---
title: 'Part 3: Aspose File Components for .NET and WCF – Airline Reservation, Complete Code'
date: Fri, 20 Jan 2012 17:07:10 +0000
draft: false
url: /2012/01/20/part-3-aspose-file-components-for-.net-and-wcf-%e2%80%93-airline-reservation-complete-code/
author: Shahzad Latif
summary: ''
tags: ['Shahzad Latif', 'Airline Reservation Scenario', 'Aspose.Total for .NET', 'Create Bar Code', 'Create Invoice', 'Create Ticket', 'Print Invoice', 'Send Attachment', 'Send Email', 'WCF Service']
categories: ['Aspose.Total Product Family']
---



{{< figure align=center src="images/aspose-Total.png" alt="Aspose.Total icon">}}


In the first part of this series, we had a look into an [airline reservation scenario][1]. The second blog post of this series gave you an [overview of the architecture of the sample application][2]. In this post, you'll have a look into the complete code of this example scenario.

This part will help you understand how easily you can create bar codes, tickets, invoices and send attachments with emails. It'll also show you how you can print the invoices. We have built this example using WCF, but you can use this code in other types of .NET applications. You can also use the code in a variety of scenarios.

This example contains a WCF service that provides the features to find flight information and reserve a seat. It also creates bar codes and tickets. The service sends the ticket as an email attachment to the customer.

We have used the following Aspose components in this example:

*   [Aspose.PDF for .NET][3]: create tickets, create invoices, print invoice
*   [Aspose.BarCode for .NET][4]: create bar codes
*   [Aspose.Email for .NET][5]: send ticket as an email attachment

On the client end, we have used Windows Forms application which allows you to find flight information and then reserve the seat for the customer. It also generates and prints an invoice for the customer.

The WCF service uses Aspose.BarCode for .NET to create bar codes for tickets and Aspose.Pdf for .NET to create tickets, while Aspose.Email for .NET sends the ticket as an email attachment to the customer.

The Windows Forms based client uses Aspose.Pdf for .NET to create invoice and then print that invoice on the default printer. This example also includes a folder containing the sample input and output files like input XML containing initial PDF structure, logos, output bar code images, sample ticket and customer invoice.

You can find the complete code in the airline reservation scenario repository on github.com along with a README.md file. The service and client projects also contain README.txt files to show you the steps for setting up the example at your end.




[1]: https://blog.aspose.com/2011/12/15/part-1-aspose-file-components-and-wcf-airline-reservation-example-scenario
[2]: https://blog.aspose.com/2011/12/21/part-2-aspose-file-components-for-.net-and-wcf-%e2%80%93-airline-reservation-example-architecture
[3]: https://products.aspose.com/pdf/net
[4]: https://products.aspose.com/barcode/net
[5]: https://products.aspose.com/email/net




