---
title: 'Aspose.Network for .NET v4.4.0.0 Released'
date: Sun, 21 Dec 2008 13:53:00 +0000
draft: false
url: /2008/12/21/aspose-network-for-net-v4-4-0-0-released/
author: Iret
summary: ''
tags: []
categories: ['Aspose.Email Product Family']
---

We just released Aspose.Network for .NET v4.4.0.0.

Many new features and enhancements are included in this new version, like sending appointments in email messages. Now you can send an appointment request in email, **update** the appointment or **cancel** the appointment. Here is the sample code:

**Request Apoinment**

           MailMessage msg = new MailMessage();  
            msg.From = "[organizer@aspose.com][1]";  
             
            //attendees for the event  
            MailAddressCollection attendees = new MailAddressCollection();  
            attendees.Add(new MailAddress("[attendee1@aspose.com][2]"));  
            attendees.Add(new MailAddress("[attendee2@aspose.com][3]"));  
            attendees.Add(new MailAddress("[attendee3@aspose.com][4]"));  
            msg.To = attendees;

            DateTime dtstart = new DateTime(2008, 12, 24, 14, 30, 0);

            //create calendar  
            Appointment appoinment= new Appointment(  
                "Room 112",  
                "Product Release meeting",  
                "Product release meeting",  
                dtstart,  
                dtstart.AddHours(1),  
                msg.From\[0\],  
                attendees);

            string uniqueId = "f6bd236b-a48b-4eb5-a9ec-2177a77bd2f4";  
            appoinment.UniqueId = uniqueId;  
            msg.Subject = "Release Meeting";

            //add the appointmentto mail message  
            msg.AddAlternateView(appoinment.RequestAppointment(0));  
           

**Update Appoinment**   
          //set the uniqueid of the appointment  
           string uniqueId = "f6bd236b-a48b-4eb5-a9ec-2177a77bd2f4";  
           appoinment.UniqueId = uniqueId;

            //send appointment with 1 as sequence id  
            msg.AddAlternateView(appoinment.UpdateAppointment(1));

**Cancel Appoinment** 

           //set the uniqueid of the appointment  
           string uniqueId = "f6bd236b-a48b-4eb5-a9ec-2177a77bd2f4";  
           appoinment.UniqueId = uniqueId;

            //send cancel appointment with 2 as the sequence id  
            msg.AddAlternateView(appoinment.CancelAppointment(2));

Check out the download page:

[http://www.aspose.com/community/files/51/file-format-components/aspose.network/default.aspx][5]




[1]: mailto:organizer@aspose.com
[2]: mailto:attendee1@aspose.com
[3]: mailto:attendee2@aspose.com
[4]: mailto:attendee3@aspose.com
[5]: http://www.aspose.com/community/files/51/file-format-components/aspose.network/default.aspx




