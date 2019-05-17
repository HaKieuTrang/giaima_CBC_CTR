Trong bài tập này, bạn sẽ cài đặt hai hệ mã/giải mã, một sử dụng AES với CBC mode và một sử dụng AES với counter mode (CTR). Trong cả hai trường hợp, IV đều là 16-byte và được chọn ngẫu nhiên, và được ghép vào bản mã. Với CBC mode bạn  sử dụng sơ đồ padding PKCS5.

Bạn có thể sử dụng cài đặt AES của thư viện như Pycrypto (Python) nhưng bạn bắt buộc phải tự cài đặt CBC và CTR mode.

Hãy dùng hàm giải mã vừa cài đặt để giải mã:
Test 1:
CBC key: 140b41b22a29beb4061bda66b6747e14
CBC Ciphertext 1: 4ca00ff4c898d61e1edbf1800618fb2828a226d160dad07883d04e008a7897ee2e4b7465d5290d0c0e6c6822236e1daafb94ffe0c5da05d9476be028ad7c1d81
Test 2:
CBC key: 140b41b22a29beb4061bda66b6747e14
CBC Ciphertext 2: 5b68629feb8606f9a6667670b75b38a5b4832d0f26e1ab7da33249de7d4afc48e713ac646ace36e872ad5fb8a512428a6e21364b0c374df45503473c5242a253
Test 3:
CTR key: 36f18357be4dbd77f050515c73fcf9f2
CTR Ciphertext 1: 69dda8455c7dd4254bf353b773304eec0ec7702330098ce7f7520d1cbbb20fc388d1b0adb5054dbd7370849dbf0b88d393f252e764f1f5f7ad97ef79d59ce29f5f51eeca32eabedd9afa9329


Test 4:

CTR key: 36f18357be4dbd77f050515c73fcf9f2
CTR Ciphertext 2: 770b80259ec33beb2561358a9f2dc617e46218c0a53cbeca695ae45faa8952aa0e311bde9d4e01726d3184c34451
