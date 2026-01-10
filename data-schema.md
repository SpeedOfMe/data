### SpeedOf.Me Data Schema ###

| Name        | Data Type | SQL Type    | Description                                   | Example                            |
| ----------- | --------- | ----------- | --------------------------------------------- | -----------------------------------|
| id          | string    | char(32)    | Unique ID for the test                        | `ad52eb4b7a81362045189f0ee69bf9e9` |
| test_date   | string    | varchar(24) | Date/Time of the test - [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) | `2026-01-09T14:07:40.084Z` |
| test_year   | number    | int         | Year the test was taken                       | `2026` |
| test_month  | number    | int         | Month the test was taken                      | `1` |
| download    | number    | float       | Download speed in Megabits per second (Mbps)  | `157.15` |
| upload      | number    | float       | Upload speed in Megabits per second (Mbps)    | `92.16` |
| max_download | number   | float       | Maximum download speed during the test (Mbps) | `160.41` |
| max_upload  | number    | float       | Maximum upload speed during the test (Mbps)   | `147.64` |
| latency     | number    | int         | Latency (aka. ping) in milliseconds (ms)      | `13` |
| jitter      | number    | int         | [Jitter](https://speedofme.zendesk.com/hc/en-us/articles/224064067) in milliseconds (ms) | `4` |
| test_server | string    | varchar(30) | [Test Server](https://speedof.me/howitworks.html#testservers) that was used for the test  | `Dallas 1` |
| geo_continent_code | string | varchar(2)  | Continent code: `AF` (Africa), `AN` (Antarctica), `AS` (Asia), `EU` (Europe), `NA` (North America), `OC` (Oceania), `SA` (South America) | `NA` |
| geo_continent_name | string | varchar(20) | Continent name | `North America` |
| geo_country_iso_code | string | varchar(2) | Two-letter [ISO 3166-1](https://en.wikipedia.org/wiki/ISO_3166-1) country code | `US` |
| geo_country_name | string | varchar(60) | Country name | `United States` |
| geo_country_is_eu | boolean | int | Country is in the European Union (0,1) | `0` |
| geo_subdivision_1_iso_code | string | varchar(3) | Region portion of [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2) code (state/province) | `TX` |
| geo_subdivision_1_name | string | varchar(80) | State/province name | `Texas` |
| geo_subdivision_2_iso_code | string | varchar(3) | Region portion of [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2) code (county/district) | `453` |
| geo_subdivision_2_name | string | varchar(80) | County/district name | `Travis County` |
| geo_city_name | string | varchar(80) | City name | `Austin` |
| geo_postal_code | string | varchar(10) | Postal code | `78731` |
| timezone    | string    | varchar(40) | IANA timezone identifier | `America/Chicago` |
| net_isp | string | varchar(80) | ISP name | `Comcast Cable` |
| net_organization | string | varchar(80) | Organization name | `Comcast Cable Communications` |
| net_asn_org | string | varchar(80) | Autonomous System organization name | `Comcast Cable Communications, LLC` |
| net_host_name | string | varchar(255) | Reverse DNS hostname | `c-73-162-155-42.hsd1.tx.comcast.net` |
| net_connection_type | string | varchar(20) | Connection type: `Cable/DSL`, `Cellular`, `Corporate`, `Dialup` | `Cable/DSL` |
| net_user_type | string | varchar(20) | User type: `residential`, `business`, `hosting`, `isp`, `library`, `education`, `military`, `government` | `residential` |
| device_is_mobile | boolean | int | Mobile device (0,1) | `0` |
| device_type | string | varchar(255) | Hardware type: `mobile`, `computer`, `appliance`, `large-screen`, `server`, `vehicle` | `computer` |
| device_sub_type | string | varchar(255) | Sub-type. For `mobile`: `phone`, `tablet`, `phablet`, `ebook-reader`, `handheld-game`, `music-player`, `pda`, `wearable`. For `computer`: `desktop`, `portable` | `desktop` |
| device_software_full | string | varchar(255) | Software and OS description | `Chrome 131 on Windows 11` |
| device_software | string | varchar(255) | Software/browser name | `Chrome` |
| device_software_version | string | varchar(255) | Software/browser version | `131` |
| device_os | string | varchar(255) | Operating system name | `Windows` | 
| device_os_version | string | varchar(255) | Operating system version | `11` | 
| device_platform_full | string | varchar(255) | Hardware platform description | `Dell Desktop` |
| device_platform_vendor | string | varchar(255) | Device manufacturer | `Dell` |
| device_platform | string | varchar(255) | Device platform name | `Desktop` |
