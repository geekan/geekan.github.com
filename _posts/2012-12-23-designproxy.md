---
layout: post
category : design
tags : [proxy, design]
title : a simple design of http proxy
---


  Browser                        Proxy                            HTTP server
  
  Open TCP connection  
  
  Send HTTP request  ----------->
  
                                 Read HTTP header
								 
                                 detect Host header
								 
                                 Send request to HTTP ----------->
								 
                                 Server
								 
                                                      <-----------
													  
                                 Read response and send
								 
                   <-----------  it back to the browser
				   
  Render content