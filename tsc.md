# Typescript
## Types
- Union Types : biến có thể là nhiều hơn một kiểu dữ liệu ví dụ let age:number | string = '25'
- Differences Between Type Aliases and Interfaces : Type và Interface đa phần là giôngs nhau và có thể thay thế cho nhau , nhưng interface có thể thêm thuộc tính bất cứ lúc nào , còn type thì không nếu thay đổi ở bất kỳ đâu sẽ báo lỗi .
- Type Assertions : từ khoá `as` giống như ép kiểu

## Classes
- super() cần được gọi trc khi access kw this trong contructor function
- Giống như toán tử var , let , const thì các properties của class cũng sẽ tự động đăng định nghĩa kiểu dữ liệu nếu bạn không định nghĩa nó
- overload contructor trong lập trình hướng đối tượng có thể viết nhiều hàm constructor và phân biệt bằng tham số đầu vào
- protected chỉ access được ở `trong` subclasses nghĩa là phải ở trong class đó , chứ ko thể gọi ở ngoài được
- reading in process ..... 

## Utility Types
- Awaited<Type> : kiểu dữ liệu khi await hay những biến có thể `.then()`
- Partial<Type> : tạo một kiểu mới từ `Type` mà tất cả các trường đều là optional
- Required<Type>: kiểu mới từ `Type` mà tất cả các trường đều là required
- Readonly<Type>: tất cả các trường đều là readonly nghĩa là không thể gán lại đc
- Record<Keys, Type> : tạo một kiểu ví dụ như một object có các key thuộc `Keys` và mỗi key sẽ chứa value là một object kiểu `Type`
- Pick<Type, Keys> : sẽ tạo ra một kiểu mới mà có các key là `Keys` nhưng nhóm key này sẽ được pick trong các key của `Type` ví dụ
- Omit<Type, Keys> : kiểu sẽ là lấy hết các key từ type trừ các key trong `Keys`
- Exclude<UnionType, ExcludedMembers> : tạo một kiểu từ UnionType loại bỏ các Type từ ExcludedMembers
  - ex
    ```typescript
    type Shape =
    | { kind: "circle"; radius: number }
    | { kind: "square"; x: number }
    | { kind: "triangle"; x: number; y: number };
 
    type T3 = Exclude<Shape, { kind: "circle" }>
     
    type T3 = {
    kind: "square";
    x: number;
    } | {
    kind: "triangle";
    x: number;
    y: number;
    }
    ```
- Extract<Type, Union> : ngược với Exclude<UnionType, ExcludedMembers>





