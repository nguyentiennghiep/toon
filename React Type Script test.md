# Test
## Library name 
### Name
1. Chai , sinon 

## Sinon
1. Sinon.spy() => là giả lập 1 hàm để xem nó gọi với tham số nào và gọi bao nhiêu lần 
2. Sinon.stub() => cũng là giả lập hàm nhưng giả lập được cả kết quả trả về 

## Jest
1. toMatchInlineSnapshot => dùng để snapshot kết quả trả về , expect(func()).toMatchInlineSnapshot();
  - sau lần đầu chạy với toMatchInlineSnapshot() thì jest sẽ tự auto generate ra snapshoot mới .
