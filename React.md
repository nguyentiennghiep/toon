# React
## Hooks
### useEffect
-  Có thể tạo 1 custom hook ,chỉ cần chú ý bắt đầu bằng từ use , hãy nhớ là mỗi lần gọi hook sẽ là các hành động khác nhau dù có là dùng chung custom hooks
-  Return bên trong hook useEffect là 1 cleanUp optional function để cleanup những đăng ký để tránh leak memory  remove những eventListener gán đã gán trong userEfeect

### useRef
- tham chiếu đến một giá trị không cần hiển thị ???
- ví dụ trong lần đầu ta khai báo const num = useRef(0) , trong lần render đầu tiên nó sẽ trả về giá trị là num.current = 0; và trong lần tiếp theo render ta có thể tham chiếu đến giá trị lần trước render bằng cách num.current
- useRef hay được sử dụng để access vào DOM 

