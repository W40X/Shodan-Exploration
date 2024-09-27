---    

## Advanced Shodan Dorks for Deep Reconnaissance

| **1. Identify specific SSL certificates:**                 |              `ssl.cert.subject.cn:"target.com"<br>`               |
| :--------------------------------------------------------- | :---------------------------------------------------------------: |
| **2. Find web applications with login forms:**                 | `http.html:"Login" http.html:"username" http.html:"password"<br>` |
| **3. Locate admin panels:**                                    |                     `http.title:"Admin"<br>`                      |
| **4. Filter results by organization and product:**             | `ssl:"target.com" org:"Cloudflare, Inc." product:"nginx" 200<br>` |
| **5. Search for Kibana instances:**                            |            `kibana content-length:217 net:"cidr"<br>`             |
| **6. Find Amazon-related services with SSL:**                  |                  `org:"Amazon" ssl:"target"<br>`                  |
| **7. Identify instances with specific dashboard information:** |      `html:"Dashboard Jenkins" http.component:"jenkins"<br>`      |
| **8. Locate sites with specific redirect responses:**          |                   `http.title:"302 Found"<br>`                    |
| **9. Search for AWS S3 bucket information:**                   |                     `X-Amz-Bucket-Region<br>`                     |
| **10. Find Jenkins servers based on response codes:**          |                        `x-jenkins 200<br>`                        |
| **11. Search for sites using Drupal:**                         |                    `X-Generator: Drupal 7<br>`                    |
| **12. Locate Google-related SSL connections:**                 |                        `ssl:"Google"<br>`                         |
| **13. Find MongoDB servers with metrics:**                     |       `all:"mongodb server information" all:"metrics"<br>`        |
| **14. Identify MongoDB instances without authentication:**     |         `port:27017 -all:"partially" all:"fs.files"<br>`          |
| **15. Locate ElasticSearch indices:**                          |              `port:"9200" all:"elastic indices"<br>`              |
| **16. Find CouchDB servers:**                                  |                      `product:"CouchDB"<br>`                      |
| **17. Identify system dashboards related to JIRA:**            |             `title:"system dashboard" html:jira<br>`              |
| **18. Locate Apache Tomcat instances:**                        |                   `product:"apache tomcat"<br>`                   |
| **19. Search for Ruby applications on specific ports:**        |                `http.component:ruby port:3000<br>`                |
| **20. Find exposed secret keys:**                              |                   `html:"secret_key_base"<br>`                    |
| **21. Locate Rack applications with specific queries:**        |              `http.html:QUERY ssl:"domain.com"<br>`               |
| **22. Identify sites using specific favicon hashes:**          |               `http.favicon.hash:81586312 200<br>`                |
| **23. Search for Pulse Secure VPN exploits:**                  |           `html:/dana-na/ Pulse Secure VPN exploit<br>`           |
| **24. Identify MongoDB instances based on response:**          |   `"MongoDB Server Information" port:27017 -authentication<br>`   |
| **25. Search for successful login messages:**                  |            `"220" "230 Login successful." port:21<br>`            |
| **26. Locate ProFTPD servers:**                                |                       `proftpd port:21<br>`                       |
| **27. Find Exim mail servers:**                                |                  `port:"25" product:"exim"<br>`                   |
| **28. Identify Memcached servers:**                            |              `port:"11211" product:"Memcached"<br>`               |
| **29. Locate Jenkins dashboard cookies:**                      | `"X-Jenkins" "Set-Cookie: JSESSIONID" http.title:"Dashboard"<br>` |
| **30. Find DNS servers with recursion enabled:**               |                `"port: 53" Recursion: Enabled<br>`                |
| **31. Identify Microsoft IIS web servers:**                    |                `product:"Microsoft IIS httpd"<br>`                |
| **32. Search for expired SSL certificates:**                   |                    `ssl.cert.expired:true<br>`                    |
| **33. Locate services with disabled authentication:**          |             `"Authentication: disabled" port:445<br>`             |


---

