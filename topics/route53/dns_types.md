## DNS Record Types  

### A Record Type  

The value for an A record is an IPv4 address in dotted decimal notation.

Ex console:  
```
192.0.2.1
```

Ex API:  
```
 <Value>192.0.2.1</Value>  
```

###  AAAA Record Type  

The value for a AAAA an IPv6 address in colon-separated hexadecimal format.  

Ex console:
```
 2001:0db8:85a3:0:0:8a2e:0370:7334
```

Ex API:
```
 <Value>2001:0db8:85a3:0:0:8a2e:0370:7334</Value>
```

###  


###  CNAME  

A CNAME Value element is the same format as a domain name.  

> The DNS protocol does not allow you to create a CNAME record for the top node of a DNS namespace, also known as the zone apex. For example, if you register the DNS name example.com, the zone apex is example.com. You cannot create a CNAME record for example.com, but you can create CNAME records for www.example.com, newproduct.example.com, and so on.  

Ex Console
```
hostname.example.com
```

Ex API
```
<Value>hostname.example.com</Value>
```

###  MX Record  

Each value for an MX record actually contains two value, priority and domain name:  

##### Priority  

An integer that represents the priority for an email server. If you specify only one server, the priority can be any integer between 0 and 65535.  

##### Domain name  

The domain name of the email server. Specify the name(such as mail.example.com) of an A or AAAA record.

Ex Console
```
10 mail.example.com
```

Ex API
```
<Value>10 mail.example.com</Value>
```

###  NAPTR Record  

A Name Authority Pointer(NAPTR) is a type of record that is used by Dynamic Delegation Discovery System(DDDS) applications to covert one value to another or to replace one value with another. For example, one common use is to convert phone numbers into SIP URIs.  

##### The Value element for an NAPTR record consists of six space-separated values:  

**Order**  

When you specify two or more records that have the same Order, yout preference for the sequence that those records are evaluated in. For example, if two records have an Order of 1, the DDDS application first evaluates the record that has the lower Preference. Valid 0-65535.  

**Flags**  

A setting that is specific to DDDS applications. Values currently defined in RFC 3404 are uppercase- and - lowecase letters "A","P", "S" and "U", and the empty string, "". Enclose Flags in quotation marks.  

**Service**  

A setting that is specific to DDDS applications. Enclose Service in quotation marks.  

**Regexp**  

A regular expression that the DDDS application to convert input value into an output value.  

**Replacement**  

The fully qualified domain name(FQDN) of the next domain name that you want the DDDS application to submit a DNS query for.  



Ex Console
```
100 50 "u" "E2U+sip" "!^(\\+441632960083)$!sip:\\1@example.com!" .
100 51 "u" "E2U+h323" "!^\\+441632960083$!h323:operator@example.com!" .
100 52 "u" "E2U+email:mailto" "!^.*$!mailto:info@example.com!" .
```

Ex API
```
<ResourceRecord>
   <Value>100 50 "u" "E2U+sip" "!^(\\+441632960083)$!sip:\\1@example.com!" .</Value>
   <Value>100 51 "u" "E2U+h323" "!^\\+441632960083$!h323:operator@example.com!" .</Value>
   <Value>100 52 "u" "E2U+email:mailto" "!^.*$!mailto:info@example.com!" .</Value>
</ResourceRecord>
```

###  NS Record  

An NS record identifies the name servers for the hosted zone. The value for an NS record is the domain name of a name server.

Ex Console
```
ns-1.example.com
```

Ex API
```
<Value>ns-1.example.com</Value>
```

###  PTR Record  

A PTR record Value element is the same format as a domain name.  

Ex Console
```
hostname.example.com
```

Ex API
```
<Value>hostname.example.com</Value>
```

###  SOA Record  

A start of authority record provide information about a domain and the corresponding Amazon Route 53 hosted zone.

Ex Console
```
ns-2048.awsdns-64.net hostmaster.awsdns.com 1 1 1 1 60
```

Ex API
```
<Value>ns-2048.awsdns-64.net hostmaster.awsdns.com 1 1 1 1 60</Value>
```

###  SPF Record  

SPF records were formerly used to verify the identity of the sender of email messages. However, we no longer recommend that you create records for which the record typeis SPF.  

Ex Console
```
"v=spf1 ip4:192.168.0.1/16 -all"
```

Ex API
```
<Value>"v=spf1 ip4:192.168.0.1/16 -all"</Value>
```


### SRV record

An SRV record Value element consists of four space-separated values.  
* The first three values are decimal numbers representing priority, weight, and port.
* The fourth value is a domain name.  

Ex Console  
```
10 5 80 hostname.example.com
```

Ex API  
```
<Value>10 5 80 hostname.example.com</Value>
```

### TXT Record  

A TXT recordcontains one or more stringsthat are enclosed in double quotation marks. When you use the simple routing policy, include all values for a domain os subdomain in the same TXT record.  

Ex Console
```
"This string includes \"quotation marks\"."
"The last character in this string is an accented e specified in octal format: \351"
"v=spf1 ip4:192.168.0.1/16 -all"
```

Ex API  
```
<Value>"This string includes \"quotation marks\"."</Value>
<Value>"The last character in this string is an accented e specified in octal format: \351"</Value>
<Value>"v=spf1 ip4:192.168.0.1/16 -all"</Value>
```
