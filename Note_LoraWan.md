# Tổng quan về LoraWan 

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

**- Sức khỏe & Vệ sinh (Health & Hygiene)**

Giám sát nhiệt độ / độ ẩm  
Kiểm soát môi trường  
Quản lý chất thải (giám sát mức chất thải trong thùng chất thải)  


## MỘT SỐ TRƯỜNG HỢP SỬ DỤNG SỬ DỤNG CÔNG NGHỆ LORA(FEW USE CASES USING LORA TECHNOLOGY) 

**• Sự an toàn (Safety)**

Smart lightning    
Giám sát mực nước  
Giám sát mức độ phóng xạ  
Giám sát đê điều (ngăn đê bùn than bùn bị khô)  

**• Hiệu quả (Efficiency)**

Quản lý tài sản (ví dụ: theo dõi container, pallet, v.v.)  
Quản lý đội xe (ví dụ: theo dõi ô tô, xe tải, v.v.)  

**• Nông nghiệp (Agriculture)** 

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


## LORAWAN NETWORK 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/LoraWan_Network.png"></div> 

- LoRaWAN network architecture is deployed in a star topology.  
- The communication between the end node and gateway is bidirectional which means the end node can send data to the gateway but it can also receive data from the gateway.  


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
- 

## LORA PROTOCOL STACK 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/LoraWan_protocol.png"></div> 

## LORA ALLIANCE 

- Các giao thức LoRaWAN được xác định bởi LoRa Alliance. 
- Đây là một tổ chức phi lợi nhuận của hơn 500 công ty thành viên, cam kết cho phép triển khai LPWAN IoT trên quy mô lớn thông qua việc phát triển và quảng bá tiêu chuẩn mở LoRaWAN. 


## ISM BAND 

- LoRa hoạt động trong băng tần vô tuyến ISM (Industrial, Scientific and Medical) không được cấp phép có sẵn trên toàn thế giới. 

<div style="text-align:center"><img src="https://github.com/vuducthanh0115/LoraWan/blob/main/Image/ISM_Band.png"></div>

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















