## createAsyncThunk
- ví dụ : createAsyncThunk<
  DeleteItemApiOkData,
  DeleteItemApiPayload,
  CommonApiConfig<CheckoutState>
>('deleteItem', async (data, { rejectWithValue, getState }) => {})

-- create createAsyncThunk để tạo một action mới dùng trong extrabuider của createSlide toolkit 
-- param đầu là tên của action 
-- param 2 là 1 function với param 1 là payload , param2 là thunkAPi gômf có những hàm như getState ,... để support 

## unwrap()
-  dispatch(actionThunk).unwrap().then(()=>do some thing when fulfilled).catch(e=>// err)
  - dùng unwrap nghĩa là không nhất thiết phải xử lý catch , chỉ khi nào cần thiết mới cần catch và sẽ không gây ra lỗi 

