#Cải thiện ReflexAgent
Một tác nhân phản xạ có khả năng sẽ phải xem xét cả vị trí thức ăn và vị trí ma để hoạt động tốt.
#minimax
Minimax là giải thuật là một thuật toán đệ quy lựa chọn bước đi kế tiếp trong một trò chơi có hai người bằng cách định giá trị cho các Node trên cây trò chơi sau đó tìm Node có giá trị phù hợp để đi bước tiếp theo.
Giải thuật Minimax Hai người chơi trong game được đại diện là MAX và MIN. MAX đại diện cho người chơi luôn muốn chiến thắng và cố gắng tối ưu hóa ưu thế của mình còn MIN đại diện cho người chơi cố gắng cho người MAX giành số điểm càng thấp càng tốt. Giải thuật Minimax thể hiện bằng cách định trị các Node trên cây trò chơi: Node thuộc lớp MAX thì gán cho nó giá trị lớn nhất của con Node đó. Node thuộc lớp MIN thì gán cho nó giá trị nhỏ nhất của con Node đó. Từ các giá trị này người chơi sẽ lựa chọn cho mình nước đi tiếp theo hợp lý nhất.
Đầu tiên chúng ta cần 1 hàm để biết trạng thái game hiện tại đã thắng, thua hay hòa. 
Tiếp theo là cần tìm nước tốt nhất cần đi.
Và tiếp đến là hàm tính giá trị minimax của các nước đó.
# Alpha beta pruning
Nút Max có một giá trị alpha (lớn hơn hoặc bằng alpha – luôn tăng), nút min có một giá trị beta (nhỏ hơn hoặc bằng beta – luôn giảm). Khi chưa có alpha và beta xác định thì thực hiện tìm kiếm sâu (depth-first) để xác định được alpha, beta, và truyền ngược lên các nút cha.

#Expectimax	
 hữu ích cho việc mô hình hóa hành vi có xác suất của các tác nhân có thể đưa ra các lựa chọn không tối ưu.
