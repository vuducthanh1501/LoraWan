# 1.Tổng quan lý thuyết về LoraWan 

## INTERNET OF THINGS 

- Internet of Things, hay IoT, là một mạng lưới các thiết bị vật lý được kết nối với Internet và có thể "nói chuyện" với nhau.  

- Dự đoán đến năm 2020 sẽ có trên 25 tỷ thiết bị kết nối Internet.  

- Có nhiều công nghệ không dây có thể sử dụng để kết nối các thiết bị này với Internet, chẳng hạn như:  

- Giao tiếp không dây tầm ngắn 
- Giao tiếp di động 
- Giao tiếp LPWA 

## LPWAN 

- LPWAN là viết tắt của Low Power Wide Area Network và loại giao tiếp không dây này được thiết kế để gửi các gói dữ liệu nhỏ ở khoảng cách xa, hoạt động bằng pin. 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/LPWAN.png"></div>  


## WIRELESS COMMUNICATION COMPARISON

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/Comparison.png"></div> 


## LORA RANGE 

- Phạm vi giữa người gửi và người nhận LoRa phụ thuộc vào môi trường thiết bị hoạt động. Phạm vi phủ sóng trong nhà phần lớn phụ thuộc vào loại vật liệu xây dựng được sử dụng. 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/Lora%20range.png"></div> 


- Một số kỷ lục đáng chú ý: 

Andreas Spiess, kết nối đất với mặt đất: 212 km (= 131,73 dặm) 

Kết nối khí cầu thời tiết với mặt đất: 702,67 km (= 436,61 dặm) 


## MỘT SỐ TRƯỜNG HỢP SỬ DỤNG NGHỆ LORA (FEW USE CASES USING LORA TECHNOLOGY)

**- Tiện ích thông minh (Smart utilities)**

Giám sát máy biến áp điện  
Giám sát mực nước  
Đồng hồ đo tiện ích  
Giám sát nhiên liệu (giám sát mức nhiên liệu trong thùng nhiên liệu để sưởi ấm nhà)  

**- Health & Hygiene**

Giám sát nhiệt độ / độ ẩm  
Kiểm soát môi trường  
Quản lý chất thải (giám sát mức chất thải trong thùng chất thải)  

**- Sự an toàn (Safety)**

Smart lightning    
Giám sát mực nước  
Giám sát mức độ phóng xạ  
Giám sát đê điều (ngăn đê bùn than bùn bị khô)  

**- Hiệu quả (Efficiency)**

Quản lý tài sản (ví dụ: theo dõi container, pallet, v.v.)  
Quản lý đội xe (ví dụ: theo dõi ô tô, xe tải, v.v.)  

**- Nông nghiệp (Agriculture)** 

Giám sát phúc lợi động vật  
Giám sát điều kiện phát triển của cây trồng  


## LORA 

- LoRa là từ viết tắt của Long Range và nó là một công nghệ không dây trong đó người gửi có công suất thấp truyền các gói dữ liệu nhỏ (0,3 kbps đến 5,5 kbps) đến người nhận trong một khoảng cách xa. 

- Một cổng có thể xử lý hàng trăm thiết bị cùng một lúc 

## LORA END NODE 

- Một nút kết thúc LoRa bao gồm 2 phần: 

• Một mô-đun radio với ăng-ten.  
• Một bộ vi xử lý để xử lý dữ liệu cảm biến chẳng hạn.  
• Các nút cuối thường được cấp nguồn bằng pin.  
• Thiết bị LoRa (nút cuối) có bộ thu phát không dây.  

Nếu thiết bị này cũng có cảm biến, thiết bị này hoạt động như một cảm biến từ xa.
Một thiết bị như vậy được gọi là remote. 

## LORA GATEWAY 

- Cổng LoRa bao gồm 2 phần:  

• Một mô-đun radio với ăng-ten.  
• Một bộ vi xử lý để xử lý dữ liệu.  
• Các cổng được cấp nguồn chính và kết nối với Internet.  
• Nhiều cổng có thể nhận dữ liệu từ cùng một nút kết thúc.  
• Các cổng có thể nghe nhiều tần số đồng thời,trong mọi hệ số lan truyền ở mỗi tần số.  

## LORAWAN

- Xác định giao thức truyền thông và kiến trúc hệ thống cho mạng lưới trong khi lớp vật lí Lora cho phép liên kết truyền thông tầm xa.  

- Là một giao thức kiểm soát truy cập phương tiện (MAC) cho các mạng diện rộng, được thiết kế để cho phép các thiết bị có công suất thấp giao tiếp với các ứng dụng kết nối Internet qua các kết nối không dây tầm xa.  


## LORAWAN NETWORK 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/LoraWan_Network.png"></div> 

- Kiến trúc mạng LoraWan đuwocj triển khai theo cấu trúc liên kết hình ngôi sao.   
- Các mạng LoraWan được đặt trong cấu trúc liên kết sao có các trạm cơ sở chuyển tiếp dữ liệu giữa các node cảm biến và Network Server. 
- Giao tiếp giữa các node cảm biến và các trạm cơ sở đi qua kênh không dây sử dụng lớp vật lý Lora, trong khi kết nối giữa các gateway và máy chủ trung tâm được xử lý qua mạng dựa trên IP. 
- End nodes truyền trực tiếp đến tất cả các Gateway trong phạm vi sử dụng Lora. 
- Gateway chuyển tiếp tin nhắn giữa các thiết bị dầu cuối và Network Server trung tâm sử dungj IP. 
- End nodes thương là cảm biến nhúng công nghệ Lora. Các node thường có: 
  + Các cảm biến : được sử dụng để phát hiện thông số thay đổi 
  + Lora transponder để truyền tín hiệu qua phương thức truyền vô tuyến được cấp bằng sáng chế của Lora. 
  + 1 bộ điều khiển vi mô(với bộ nhớ trên bo mạch) có thể có hoặc không 
Các cảm biến có thể kết nối với chip transponder Lora hoặc cảm biến có thể là 1 đơn vị tích hợp với chip transponder Lora được nhúng bên trong. 


## UPLINK AND DOWNLINK 

- When an end node transmits data to the gateway it is called an uplink. 
- When the gateway transmits data to the end node it is called a downlink. 

## LORAWAN HOẠT ĐỘNG NHƯ THẾ NÀO 

- Một nút cuối phát dữ liệu của nó tới mọi cổng trong vùng lân cận của nó. 
- Các cổng chuyển tiếp gói tin này đến máy chủ mạng. 
- Máy chủ mạng thu thập tin nhắn từ tất cả các cổng và lọc ra dữ liệu trùng lặp và xác định cổng có khả năng tiếp nhận tốt nhất. 
- Máy chủ mạng chuyển tiếp gói tin đến đúng máy chủ ứng dụng nơi người dùng cuối có thể xử lý dữ liệu cảm biến. 
- Tùy chọn máy chủ ứng dụng có thể gửi phản hồi trở lại nút cuối. 
Khi một phản hồi được gửi đi, máy chủ mạng sẽ nhận phản hồi và xác định cổng nào sẽ sử dụng để phát phản hồi trở lại nút cuối. 


## GIAO TIẾP TRỰC TIẾP GIỮA CÁC THIẾT BỊ LORA 

- Giao thức LoRaWAN không hỗ trợ giao tiếp trực tiếp giữa các nút cuối. 
- Nếu bạn muốn giao tiếp trực tiếp giữa các thiết bị LoRa mà không cần sử dụng cổng, hãy sử dụng thư viện RadioHead Packet Radio dành cho bộ vi xử lý nhúng. Nó cung cấp một thư viện hướng đối tượng hoàn chỉnh để gửi và nhận các tin nhắn có kích thước gói thông qua nhiều loại radio như LoRa trên một loạt các bộ vi xử lý nhúng. 


## LORA PROTOCOL STACK 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/LoraWan_protocol.png"></div> 

## LORA ALLIANCE 

- Các giao thức LoRaWAN được xác định bởi LoRa Alliance. 
- Đây là một tổ chức phi lợi nhuận của hơn 500 công ty thành viên, cam kết cho phép triển khai LPWAN IoT trên quy mô lớn thông qua việc phát triển và quảng bá tiêu chuẩn mở LoRaWAN. 

## ISM BAND 

- LoRa hoạt động trong băng tần vô tuyến ISM (Industrial, Scientific and Medical) không được cấp phép có sẵn trên toàn thế giới. 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/ISM-Band.png"></div>

- Tại Hoa Kỳ, LoRaWAN hoạt động trong dải tần 902-928 MHz. 

- Các thiết bị như lò vi sóng, thiết bị y tế hoặc màn hình trẻ em đều sử dụng băng tần ISM. 

**Ưu điểm của băng tần ISM:** 

• Bất kỳ ai cũng được phép sử dụng các tần số này. 
• Không có lệ phí giấy phép được yêu cầu. 

**Nhược điểm của băng tần ISM:** 

• Tốc độ dữ liệu thấp. 
• Rất nhiều nhiễu vì bất kỳ ai cũng có thể sử dụng các tần số này. 

## ETSI VÀ FCC 

- Bởi vì băng tần ISM có thể được sử dụng bởi tất cả mọi người, phải có một số quy tắc được đặt ra nếu không băng tần này sẽ trở nên không sử dụng được. Hãy nghĩ đến nhiều tín hiệu gây nhiễu. 

- Có một số tổ chức quốc tế quản lý phổ tần vô tuyến để đảm bảo sự chung sống an toàn giữa tất cả các các công nghệ vô tuyến khác nhau. 

- Ở Châu Âu, Viện Tiêu chuẩn Viễn thông Châu Âu (ETSI) tạo ra các tiêu chuẩn được sử dụng bởi các cơ quan quản lý địa phương (= quốc gia). 

- Tại Hoa Kỳ, Ủy ban Truyền thông Liên bang (FCC) tạo ra các tiêu chuẩn này. 

- Tất cả các quốc gia khác đang sử dụng các bộ tiêu chuẩn của ETSI hoặc FCC.
Ngoại trừ Nhật Bản, họ có Trung tâm Kỹ thuật Viễn thông (TELEC) và Hàn Quốc họ có Ủy ban Truyền thông Hàn Quốc (KCC).  

- Ví dụ ở Hà Lan, cơ quan quản lý viễn thông của nó được gọi là Cơ quan Viễn thông (Tiếng Hà Lan: Agentschap Telecom), là một bộ phận của Bộ Kinh tế và Khí hậu (Tiếng Hà Lan: Bộ trưởng van Economische Zaken en Klimaat). 

- Cơ quan quản lý này đã ban hành các điều kiện và yêu cầu khi sử dụng LoRa ở Hà Lan và dựa trên các tiêu chuẩn do ETSI đặt ra.  

## ORGANISATIONS AND REGULATORY AUTHORITIES 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/Orangnisation.png"></div> 

## ISM BAND AND DUTY CYCLE 

- Ví dụ: ở Châu Âu khi sử dụng các tần số băng tần ISM (863 MHz - 870 MHz), người dùng phải tuân thủ các quy tắc sau: 

- Đối với đường lên, công suất truyền tối đa được giới hạn ở 25mW (14 dBm).Đối với đường xuống (cho 869,525MHz), công suất truyền tải tối đa được giới hạn ở 0,5W (27 dBm) 

- Có chu kỳ nhiệm vụ 0,1% và 1,0% mỗi ngày tùy thuộc vào kênh. 

- Bên cạnh các quy tắc về băng tần ISM này, nhà khai thác mạng (ví dụ: The Things Network) cũng có thể thêm các hạn chế bổ sung. 

## THE THINGS NETWORK (TTN) FAIR USE 

• Nếu bạn sử dụng The Things Network (mạng LoRaWAN cộng đồng công cộng miễn phí) chính sách sử dụng hợp lý sau sẽ được áp dụng: 
• Thời gian phát sóng của đường lên được giới hạn trong 30 giây mỗi ngày (24 giờ) cho mỗi nút. 
• Các thông báo đường xuống được giới hạn ở 10 thông báo mỗi ngày (24 giờ) cho mỗi nút. 

## TIME ON AIR 

• Thời gian trực tuyến (ToA) là khoảng thời gian ăng-ten của máy phát được cấp năng lượng và truyền dữ liệu. 
Lưu ý: ToA là không phải thời gian từTx đến Rx.  

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/Time_on_air.png"></div> 

## DUTY CYCLE 

• Chu kỳ làm việc là tỷ lệ thời gian trong đó một bộ phận, thiết bị hoặc hệ thống được vận hành. Chu kỳ làm việc có thể được biểu thị dưới dạng tỷ lệ hoặc phần trăm. 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/duty%20cycle.png"></div> 

## LORAWAN DEVICE CLASSES 

• The LoRaWAN specification [4] defines three device classes: 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/Class.png"></div>

### CLASS A 

- Tại bất kỳ thời điểm nào, một nút kết thúc có thể phát tín hiệu. Sau quá trình truyền uplink 
(tx), nút cuối sẽ lắng nghe phản hồi từ cổng kết nối. 
- Nút cuối mở 2 khe nhận tại t1 và t2 vài giây sau khi truyền tải đường lên. Cổng có thể phản hồi trong khe nhận đầu tiên hoặc khe nhận thứ hai, nhưng không phải cả hai. 
- Class B và C cũng phải hỗ trợ chức năng class A. 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/class%20A.png"></div> 

### CLASS B 

- Ngoài các slot nhận Class A, các thiết bị Class B mở thêm các slot nhận vào các thời điểm đã lên lịch. 
- Nút cuối nhận được một báo hiệu được đồng bộ hóa thời gian từ gateway, cho phép cổng kết nối biết khi nào nút đang lắng nghe. 
- Class B không hỗ trợ chức năng của thiết bị C. 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/Class%20B.png"></div> 

### CLASS C 

- Ngoài các khe nhận class A, một thiết bị class C sẽ lắng nghe liên tục các phản hồi từ gateway. 
- Thiết bị class C không hỗ trợ chức năng của thiết bị B. 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/class%20C.png"></div>


### PROPAGATION

• Sự lan truyền là cách sóng vô tuyến truyền qua không gian tự do (còn được gọi là phương tiện).Cách mà những sóng này truyền đi có thể ảnh hưởng đến cường độ tín hiệu của nó.  

• Sự lan truyền đường nhìn  
Sóng vô tuyến truyền trực tiếp từ người gửi đến người nhận mà không gặp bất kỳ trở ngại nào. Nếu khoảng cách giữa người gửi và người nhận càng lớn thì tín hiệu sẽ yếu đi. Mất mát này được gọi là mất dung lượng trống. 

• Nếu có trở ngại gần đường đi của nó (trong vùng Fresnel), sóng vô tuyến phản xạ từ những vật thể đó có thể đến lệch pha với tín hiệu truyền trực tiếp và làm giảm công suất của tín hiệu nhận được. 

• Truyền qua chướng ngại vật
Sóng vô tuyến có thể xuyên qua các chướng ngại vật xuất hiện trên đường đi của nó. Sóng vô tuyến mất sức mạnh nếu nó đi qua chướng ngại vật làm bằng vật liệu dẫn điện hơn.  

• Sự lan truyền thông qua sự phản chiếu  
Sóng vô tuyến có thể bị phản xạ bởi các tòa nhà gây nhiễu tín hiệu trực tiếp của nó. 

• Sự lan truyền thông qua sự nhiễu xạ
Nhiễu xạ là nơi sóng vô tuyến bị bẻ cong xung quanh các cạnh sắc. Cổng vào có thể nhận được tín hiệu từ một máy phát mặc dù nó có thể bị “che khuất” bởi một chướng ngại vật lớn. 

### Lora Terminologies 

#### Chirp: 
-  Up-chirp: Tần số tăng dần theo thời gian. 
-  Down-Chirp: Tần số giảm dần theo thời gian. 

### Dữ liệu trong 1 radio packet của LoRa, bao gồm:

- Preamble: Là chuỗi binary để bộ nhận detect được tín hiệu của LoRa packet trong không khí 
- Header: chứa thông tin về size của Payload cũng như có PayloadCRC  hay không. Giá trị của Header cũng được check CRC kèm theo 
- Payload: là dữ liệu ứng dụng truyền qua LoRa 
- Payload: giá trị CRC của Payload. Nếu có PayloadCRC, LoRa chip sẽ tự kiểm tra dữ liệu trong Payload và báo lên nếu CRC OK hay không 

## Lora chip 

Semtech SX1278: Single channel Lora chip 

- Available in Ra01, Ra02 and RFM96 

Semtech SX1301: 8-channel Lora chip 
- Fully compatible with LoraWan 

## Lora ModuleSPI

Lora module = MCU + Lora chip  
MCU : STM8, STM32, ESP8266, ESP32, ARM, ...  
MCU and Lora chip are connected using SPI interface.  

### Lora Module - UART 

UART Lora Module: E32(better) and AS32  
- SX 1278 + STM8 . Connected via UART TX and RX 
- Has GUI tool to configure. Hide important Lora settings 

### SPI(Serial Peripheral Interface) or UART Lora Module? 

- UART module 
  + Pro: Simple for point to point Lora connection. 
  + Cons: Slower in bandwidth due to UART speed and MCU polling. 

- SPI module 
  + Pro: Faster. Can control every Lora settings to suit the purpose. 
  + Cons: Need to do everything yourself. Hence, make it easy and open source. 

## CÁCH KẾT NỐI LORAWAN GATEWAY VÀO LORAWAN SERVER 

Hai cách thức chính: Packet Forwarder và Bridge.  

**1. PACKET FORWARDER** 

- Packet Forwarder do chính Semtech (hãng sản xuất chip LoRa) tạo ra và vẫn còn được code thêm / bảo trì.  
- Ưu điểm: Nguồn mở, đơn giản và dễ quay bài code cho các nền tảng khác nhau.  
- Nhược điểm: Bảo mặt kém hơn và UDP thì dễ mất gói hơn TCP.  
- Kiểu kết nối này hay gặp ở các LoRaWAN gateway 1 kênh.  

**2. BRIDGE** 

- Kiểu kết nối Bridge là do các hãng LoRaWAN server tạo ra và hỗ trợ cho các LoRaWAN gateway phổ biến.  
- Thường nó bao gồm cả Packet forwarder (UDP/1700) bên trong gateway. Và gateway tự đọc UDP/1700 và giao tiếp với LoRaWAN server qua MQTT/MQTTS.  
- Ưu điểm: Bao gồm mọi ưu điểm của MQTT/MQTTS. Bảo mật tốt hơn do có authentication (user/password) và có mã hóa nếu dùng MQTTS.  
- Nhược kiểm: Cồng kềnh, phức tạp hơn. Nên không phải gateway nào cũng hỗ trợ.  
- Kiểu kết nối này hay gặp ở các LoRaWAN gateway 8 kênh trở lên (Kerlink, Dragino 8 kênh...)  

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/Conected.jpg"></div>

### LORAWAN GATEWAY: DATA FORWARDER GIỮA NODE VÀ NETWORK SERVER

**1. Chức năng**  
- LoRaWAN gateway nằm ở giữa LoRaWAN node và LoRaWAN network server.  
- Là một thành phần bắt buộc cần có. Buộc phải chạy giao thức LoRaWAN.
- Làm nhiệm vụ gứi dữ liệu từ node lên server (uplink) và gửi dữ liệu từ server về node (downlink)
- Không can thiệp vào dữ liệu giữa node và server.
- Có thể dùng chung bởi nhiều LoRaWAN node. 

**2. Thành phần**  
- Thành phần chính bao gồm:
+ MCU: Chip xử lý như Arduino, STM32, ESP32...
+ Ethernet / WiFi / 3G: Dùng để kết nối với network server qua giao thức TCP/IP thông thường.
+ LoRaWAN module: Semtech SX123x (8 kênh) hoặc SX126x/127x (1 kênh). Dùng để kết nối với LoRaWAN node. 

**Note** : LoRaWAN gateway về nguyên tắc nó chỉ kết nối với LoRaWAN Network server.Kết nối với hệ thống MQTT ngoài hay HASS ngoài thông qua LoRaWAN Network server hoặc IoT server. LoRaWAN gateway không giải mã (decrypt) và không đọc được dữ liệu giữa node và server. Dữ liệu giữa node và server được mã hóa.  

### LORAWAN NODE: CẢM BIẾN VÀ LORAWAN 

**1. CHỨC NĂNG** 

- Trong 3 thành phần chuẩn LoRaWAN node, gateway và network server thì LoRaWAN node là thành phần quan trọng nhất.
- Kết nối trực tiếp với vô vàn cảm biến từ dân dụng / công nghiệp / nông nghiệp.
- Kết nối đến relay để đóng cắt nguồn điện.
- Gửi dữ liệu đã mã hóa về network server thông qua LoRaWAN gateway.
- Vì được kết nối với nhiều loại cảm biến, nên LoRaWAN node rất đa dạng.
- Tuy nhiên, nếu dùng chuẩn LoRaWAN thì mọi LoRaWAN node đều hoạt động với mọi loại LoRaWAN gateway và network server.

**2. THÀNH PHẦN**  

- LoRaWAN Sensor = LoRaWAN Node + Sensor. 
+ LoRaWAN Sensor là LoRaWAN Node gắn thêm cảm biến. 

- LoRaWAN node = MCU + SX126x / SX127x 
+ MCU: ESP32, Arduino, STM32....  
+ Semtech LoRa SX126x / SX127x: Đa phần là chip single channel SX126x / 127x. 


# 2. Các vấn đề nghiên cứu phát triển, triển khai 

- Nghiên cứu, tìm hiểu về LoRaWAN, phân biệt LoRa spi và LoRa uart. Đi sâu vào tìm hiểu LoRa spi. 
- Nghiên cứu tìm hiểu về phần cứng để build 1 bộ.  
- Mục tiêu đầu tiên nghiên cứu kết nối 2 máy  

### Raspberry pi 

Raspberry Pi gồm có 6 khối liên kết lại với nhau : Ram, CPU/GPU, I/O, USB hub, Ethernet, 2x USB. 

Raspberry model B bao gồm:
- SoC 700MHz với 512MB RAM.
- 1 cổng HDMI cho đầu ra âm thanh/video số.
- 1 cổng video RCA cho đầu ra video Analog.
- 02 cổng USB.
- 01 cổng Ethernet LAN.
- 01 đầu đọc thẻ nhớ SD để tải hệ điều hành.
- 01 giao diện GPIO (General Purpose Input/Output).
- Jack Headphone Stereo 3.5mm cho đầu ra âm thanh Analog.

<div style="text-align:center"><img src="https://github.com/vuducthanh1501/LoraWan/blob/main/Image/Rasp.png"></div> 

### Arduino 

Arduino là một bo mạch vi điều khiển do một nhóm giáo sư và sinh viên nước Ý thiết kế và đưa ra đầu tiên vào năm 2005. Mạch Arduino được sử dụng để cảm nhận và điều khiển nhiều đối tượng khác nhau. Nó có thể thực hiện nhiều nhiệm vụ lấy tín hiệu từ cảm biến đến điều khiển đèn, động cơ, và nhiều đối tượng khác. Ngoài ra mạch còn có khả năng liên kết với nhiều module khác nhau như module đọc thẻ từ, ethernet shield, sim900A, ….để tăng khả ứng dụng của mạch.  

Phần cứng bao gồm một board mạch nguồn mở được thiết kế trên nền tảng vi xử lý AVR Atmel 8bit, hoặc ARM, Atmel 32-bit,…. Hiện phần cứng của Arduino có tất cả 6 phiên bản, Tuy nhiên phiên bản thường được sử dụng nhiều nhất là Arduino Uno và Arduino Mega.  

Phần mềm để lập trình cho mạch Arduino là phần mềm IDE.  

#### Các loại Board Arduino phổ biến 

1. Arduino Uno  
Đây chính là loại board đơn giản nhất nên rất phù hợp với những người mới bắt đầu tìm hiểu về lĩnh vực này. Dữ liệu số bao gồm 14 chân, đầu vào gồm 6 chân 5V, khả năng phân giải là 1024 mức, tốc độ 16MHz, điện áp từ 7V đến 12V. Kích thước của Board này là 5,5x7cm.  

2. Arduino Micro  
Bao gồm có đến 20 chân, trong đó có 7 chân có thể phát PWM. Loại này có thiết kế khá nhỏ gọn, kích thước chỉ 5x2cm.  

3. Arduino Nano  
Có thể nói đây chính là loại board có kích thước nhỏ nhất chỉ 2x4cm, việc lắp đặt được thực hiện dễ dàng.  

4. Arduino Pro  
Đây là một thiết kế mới mẻ khi chân số không có sẵn, tùy vào số chân bạn sử dụng để gắn trực tiếp và giúp tiết kiệm được khoảng không lớn, ta thường thấy hai loại có nguồn 3.3V và 5V.  

5. Arduino Mega  
Chân số lên đến 64, 14 chân có thể phát PWM, 4 cổng truyền tiếp cùng kích thước khá lớn 5x10cm.  

6. Arduino Leonardo  
Là board không có cổng nối USB dùng lập trình. Được thiết kế tại một chip nhỏ điều khiển. Kết nối qua COM ảo và có thể kết nối với chuột và bàn phím.  
  
7. Arduino LilyPad  
Board mạch Lily Pad Arduino là một công nghệ dệt điện tử có thể đeo được được mở rộng bởi Leah Sang Buechley, và được thiết kế một cách cẩn thận bởi dòng Lea Leah và SparkFun. Mỗi board được thiết kế một cách tưởng tượng với các miếng kết nối khổng lồ & một mặt sau mịn màng để cho chúng được khâu vào quần áo bằng chỉ . Arduino này cũng bao gồm I / O, nguồn và cả board cảm biến được chế tạo đặc biệt cho hàng dệt may điện tử.  

8. Arduino RedBoard  
Board mạch RedBoard Arduino có thể được lập trình bằng cáp USB Mini-B bằng Arduino IDE. Nó sẽ hoạt động trên Windows 8 mà không phải sửa đổi cài đặt bảo mật của bạn. Nó không đổi do chip USB hoặc FTDI chúng tôi sử dụng và nó hoàn toàn phẳng ở mặt sau. Tạo nó rất đơn giản để sử dụng trong thiết kế dự án. Chỉ cần cắm board, chọn tùy chọn menu để chọn Arduino UNO và bạn đã sẵn sàng để tải lên chương trình. Bạn có thể điều khiển RedBoard qua cáp USB bằng giắc cắm thùng.  

# 3. Kết quả thu được


# Các kiến thức được tìm hiểu tại group: [Easy LoRa - IoTThinks.com](https://www.facebook.com/groups/iotthinks)





