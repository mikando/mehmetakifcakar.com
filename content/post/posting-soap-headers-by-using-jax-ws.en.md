+++
author = "Mehmet Akif Çakar"
categories = ["Programming"]
date = "2008-05-07"
description = "Posting Soap Headers By Using Jax-WS"
linktitle = "Posting Soap Headers By Using Jax-WS"
title = "Posting Soap Headers By Using Jax-WS"
slug = "posting-soap-headers-by-using-jax-ws"
type = "post"
+++

Metro’s wsimport utility has a new option (XadditionalHeaders) which maps additional soap headers as method parameters. So we don’t have to deal with WSBindingProvider class anymore. So this should be the easiest and probably the most reliable solution. For ant task, use xadditionalHeaders=”true” also for commandline use -XadditionalHeaders