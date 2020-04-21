+++
author = "Mehmet Akif Çakar"
categories = ["Programming"]
date = "2009-03-15"
description = "Terminating Unwanted Running Instances in Biztalk Server 2006"
linktitle = "Terminating Unwanted Running Instances in Biztalk Server 2006"
title = "Terminating Unwanted Running Instances in Biztalk Server 2006"
slug = "terminating-unwanted-running-instances-in-biztalk-server-2006"
type = "post"
+++

There may be several reasons prevent to suspend or terminate running instances in biztalk server. Here is the sample checklist before starting maintenance:

    * Check Receive Location Adaptors (It’s not a must, but you may need to disable it in some cases)
    * Check IIS or your custom host solution that receive adaptor uses.
    * Check SqlServer Agent Service is running(Biztalk uses it in a lot of maintenance tasks)