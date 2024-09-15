-_min-width_: độ rộng tối thiểu -_max-width_: độ rộng tối đa

- _flexbox_: áp dụng thuộc tính display flex vào phần tử mình muốn dàn layout
- _flex-direction_: hướng hiển thị , row(mặc định), column, row-reverse(hướng ngược lại của dòng- ngang), column-reverse
- _align-items_:stretch(mặc định- các cột độ cao bằng nhau theo hướng row ), còn column thì làm cho các cột có độ rộng bằng nhau

  - 'flex-start': phần trên đầu
  - 'flex-end': phần cuối
  - 'flex-center': phần giữa
  - 'baseline': căn theo đít chữ của dòng chữ đầu tiên

- _flex-wrap_: không cho phép rớt xuống hàng

  - 'nowrap': - mặc định ko cho phép rớt xuống hàng- ko tốt vì layout có thể linh động
  - 'wrap': cho phép rớt xuống hàng

- chia phần trăm để linh hoạt chứ không để width cố định
- khi dùng phần trăm phải nhớ phần trăm đó của ai

- _object-fit_: 'cover', vd: ảnh nhỏ khung to thì sẽ giúp scale ảnh full khung

_calc_ : hàm dùng để tính toán +, -, \* , /, lưu ý là phải có khoảng cách giữa các phép tính
\_ cách cài đặt pug và sass: Mở terminal -> npm install -g pug sass

- _component_: khối dùng để tái sử dụng , tùy chỉnh 1 chỗ để sử dụng nhiều nơi
  _pug_:https://pugjs.org/api/getting-started.html
  (link document pug)
  - link pug giúp chuyển đổi code (https://pughtml.com/)
    -mixins: nằm trong pug document , viết 1 lần sử dụng nhiều lần, tái sử dụng code
    - biến : sd =, #{biến}
      _sass_:
      _javascript_:
- _position_: có 5 giá trị chính static, relative, absolute, sticky, fixed
  khi sử dụng thuộc tính position này thì đi kèm sẽ có các thuộc tính khác như top right left bottom z-index

  - 'relative': khi sử dụng giá trị này thì phải lưu ý xem phần tử con của nó có sử dụng position là 'absolute' hay không, thì nó sẽ chạy theo class cha or ông nội > body sử dụng position absolute hoặc relative
  - 'absolute': khi sử dụng giá trị này thì phải lưu ý xem phần tử chứa nó gần nhất có sử dụng là position absolute hay relative không

  _column-gap_: khoảng trống theo chiều dọc
  _row-gap_: khoảng trống theo chiều ngang
  _gap_ : viết rút gọn, row trước , column sau. Sử dụng cho class cha

  - _justify-content_:

    - 'flex-start': toàn bộ phần tử dồn về phía bên trái- mặc định
    - 'flex-end': toàn bộ phần tử dồn về phía bên phải
    - 'center': phần tử nằm giữa
    - 'space between': chia đầu cuối, có 3 chỗ , mà chỉ chiếm 2 thì space between sẽ là 1 cái ở đầu, 1 cái ở cuối
      -'space-around': khoảng trống xung quanh, khoảng trống (kt giữa = kt trái + kt phải)
    - 'space-evenly': khoảng trống đều nhau

  - _word-break_: tách chữ để không bị tràn khỏi khoảng trống
    - 'break-all': tách chữ nhưng không có ý nghĩa
    - 'break-word': tách chữ có ý nghĩa, bị tràn hoặc dính chữ
      _whitle-space_: nowrap ko cho chữ rớt xuống hàng
  - \_text-overflow\_:ellipsis dấu ...
  - _overflow_: hidden , để khi mà chữ tràn ra ngoài thì nó sẽ cut đi
