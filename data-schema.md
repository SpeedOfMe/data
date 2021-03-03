### SpeedOf.Me Data Schema ###

| Name        | Data Type | SQL Type    | Description                                   | Example                            |
| ----------- | --------- | ----------- | --------------------------------------------- | -----------------------------------|
| id          | string    | char(32)    | Unique ID for the test                        | `ad52eb4b7a81362045189f0ee69bf9e9` |
| test_date   | string    | varchar(24) | Date/Time of the test - [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) | `2020-03-11T14:07:40.084Z` |
| test_year   | number    | int         | Year the test was taken                       | `2020` |
| test_month  | number    | int         | Month the test was taken                      | `3` |
| download    | number    | float       | Download speed in Megabits per second (Mbps)  | `157.15` |
| upload      | number    | float       | Upload speed in Megabits per second (Mbps)    | `92.16` |
| max_download | number   | float       | Maximum download speed during the test (Mbps) | `160.41` |       
| max_upload  | number    | float       | Maximum upload speed during the test (Mbps)   | `147.64` |
| latency     | number    | int         | Latency (aka. ping) in milliseconds (ms)      | `13` |
| jitter      | number    | int         | [Jitter](https://speedofme.zendesk.com/hc/en-us/articles/224064067) in milliseconds (ms) | `14` |
| test_server | string    | varchar(30) | [Test Server](https://speedof.me/howitworks.html#testservers) that was used for the test  | `Dallas 1` | 
| geo_continent_code | string | varchar(2)  | `AF: Africa, AN: Antarctica, AS: Asia, EU: Europe, NA: North America, OC: Oceania, SA: South America` | `NA` |
| geo_continent_name | string | varchar(20) | Continent Name | `North America` |
| geo_country_iso_code | string | varchar(2) | A two-letter [ISO 3166-1](https://en.wikipedia.org/wiki/ISO_3166-1) country code | `US` |
| geo_country_name | string | varchar(60) | Country name | `United States` |
| geo_subdivision_1_iso_code | string | varchar(3) | A string of up to three characters containing the region-portion of the [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2) code (less specific) | `TX` |
| geo_subdivision_1_name | string | varchar(80) | Subdivision name (less specific) | `Texas` |
| geo_subdivision_2_iso_code | string | varchar(3) | A string of up to three characters containing the region-portion of the [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2) code (more specific) | `CZ` |
| geo_subdivision_2_name | string | varchar(80) | Subdivision name (more specific) | `Provincia di Catanzaro` |
| geo_city_name | string | varchar(80) | City name | `Austin` |
| geo_postal_code | string | varchar(10) | Postal code (US Zip code) | `78731` |
| net_organization | string | varchar(80) | Network - Organization name | `Whole Foods Market` | 
| net_isp | string | varchar(80) | Network - ISP name | `Level 3 Communications` |
| net_host_name | string | varchar(255) | Network - Server Hostname | `wholefoods.com` |
| net_connection_type | string | varchar(255) | Network - Connection type. One of the following values: `Dialup`, `Cable/DSL`, `Corporate`, or `Cellular` | `Cable/DSL` |
| device_is_mobile | boolean | int | Mobile device? (0,1) | `1`
| device_type | string | varchar(255) | Device hardware type: `mobile`, `computer`, `appliance`, `large-screen`, `server`, `vehicle` | `mobile` |
| device_sub_type | string | varchar(255) | Device sub-type based on the `device_type`. For `device_type = mobile`, the sub-type could be: `phone`, `tablet`, `phablet`, `ebook-reader`, `handheld-game`, `music-player`, `pda`, `wearable`. For `device_type = computer`, the sub-type could be: `desktop`, `portable` | `phone` |
| device_software_full | string | varchar(255) | A human-readable description of the Software and Operating System (or Platform - when possible and when there’s not also an Operating System). | `Chrome 86 on macOS (Catalina)` |
| device_software | string | varchar(255) | The name of the software on the device; Usually browser name | `Chrome` |
| device_software_version | string | varchar(255) | The version of the software on the device; Usually browser version | `86` |
| device_os | string | varchar(255) | The name of the device Operating System | `Mac OS X` | 
| device_os_version | string | varchar(255) | The version of the device Operating System | `Catalina` | 
| device_platform_full | string | varchar(255) | A human-readable description of whatever could be detected as the device hardware platform | `Apple iPhone` |
| device_platform_vendor | string | varchar(255) | The name of the vendor/manufacturer of the device platform | `Apple` |
| device_platform | string | varchar(255) | The name of the device platform | `iPhone` |
